<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `varnish`

-	[`varnish:6.0`](#varnish60)
-	[`varnish:6.0.8`](#varnish608)
-	[`varnish:6.6`](#varnish66)
-	[`varnish:6.6-alpine`](#varnish66-alpine)
-	[`varnish:6.6.1`](#varnish661)
-	[`varnish:6.6.1-alpine`](#varnish661-alpine)
-	[`varnish:7.0`](#varnish70)
-	[`varnish:7.0-alpine`](#varnish70-alpine)
-	[`varnish:7.0.1`](#varnish701)
-	[`varnish:7.0.1-alpine`](#varnish701-alpine)
-	[`varnish:alpine`](#varnishalpine)
-	[`varnish:fresh`](#varnishfresh)
-	[`varnish:fresh-alpine`](#varnishfresh-alpine)
-	[`varnish:latest`](#varnishlatest)
-	[`varnish:old`](#varnishold)
-	[`varnish:old-alpine`](#varnishold-alpine)
-	[`varnish:stable`](#varnishstable)

## `varnish:6.0`

```console
$ docker pull varnish@sha256:786e9bd61f197b2720853007c7c507c6bdc71f4e3236e03d35da367a01e2d116
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
$ docker pull varnish@sha256:a21d8beb55aa8f902b55a6f773c581dcd6537a8883d0d24b5d32c18f1b662bdb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100572918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58725732895fe16eebccbad29fc67442778d35629b74e64b49b44538eaa3dcfe`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 02:48:20 GMT
ADD file:ece5ff85ca549f0b1e9139d29dcb43a52af672d0591c423e28180f6d8d700ad7 in / 
# Thu, 02 Dec 2021 02:48:21 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 17:48:20 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 17:58:16 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.0.8.tgz -o $tmpdir/orig.tgz;     echo "73ed2f465ba3b11680b20a70633fc78da9b3eac68395f927b7ff02f4106b6cc92a2b395db2813a0605da2771530e5c4fc594eaf5a9a32bf2e42181b6dd90cf3f  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.8|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 17:58:17 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 17:58:17 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 02 Dec 2021 17:58:17 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 17:58:17 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 17:58:18 GMT
CMD []
```

-	Layers:
	-	`sha256:e5ae68f740265288a4888db98d2999a638fdcb6d725f427678814538d253aa4d`  
		Last Modified: Thu, 02 Dec 2021 02:53:46 GMT  
		Size: 31.4 MB (31370221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3cfaf0bcb14454b543ce0498ecb01e3e93089900b28fb13ae862bb38a29a84`  
		Last Modified: Thu, 02 Dec 2021 17:59:42 GMT  
		Size: 69.2 MB (69201997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c37ac8a55c4f5f4a2cb6e64b5198e81377fdfa11ec23d4000d7c90e35edb37`  
		Last Modified: Thu, 02 Dec 2021 17:59:29 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; arm variant v7

```console
$ docker pull varnish@sha256:78c279b4c10a6687be3db34d347f867a234def120a1e06dc418c7f7e44a9c727
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77216753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57d84c4c56a5deeba196ae1f0a545651321f1381d4f6bc472f4495ce898ecfdf`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 09:05:17 GMT
ADD file:97ce5af9ff4fb4002733d5c402ddc01a13e765d31b85bb6525a7fa797b698e10 in / 
# Thu, 02 Dec 2021 09:05:17 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 17:16:05 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 17:34:44 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.0.8.tgz -o $tmpdir/orig.tgz;     echo "73ed2f465ba3b11680b20a70633fc78da9b3eac68395f927b7ff02f4106b6cc92a2b395db2813a0605da2771530e5c4fc594eaf5a9a32bf2e42181b6dd90cf3f  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.8|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 17:34:45 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 17:34:45 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 02 Dec 2021 17:34:46 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 17:34:46 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 17:34:47 GMT
CMD []
```

-	Layers:
	-	`sha256:ba82a1312e1efdcd1cc6eb31cd40358dcec180da31779dac399cba31bf3dc206`  
		Last Modified: Thu, 02 Dec 2021 09:21:03 GMT  
		Size: 26.6 MB (26573192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a26aabdc4af6fcc2f87ffedefcd2035994ad7c44dbfc8ca07bcc82b1fd49ac0`  
		Last Modified: Thu, 02 Dec 2021 17:38:18 GMT  
		Size: 50.6 MB (50642860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2885c8aa3ff49bada1b1b2038107980ee649083c64c42d6534df3bf77cbf35`  
		Last Modified: Thu, 02 Dec 2021 17:37:55 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:ac60c1e4761cc40d24baa103506086f6f415a4b67f72d02a4342ee7208300669
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94686680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:967bad5c1de22c86008e49361e2caf5e5e47e81271b94caf94047c037d70e1aa`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Dec 2021 01:42:23 GMT
ADD file:986f91febed4aa8e2072081ff8419d52ba2060510822e717086d3b3d9469e4d7 in / 
# Tue, 21 Dec 2021 01:42:24 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:28:06 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Dec 2021 10:35:31 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.0.8.tgz -o $tmpdir/orig.tgz;     echo "73ed2f465ba3b11680b20a70633fc78da9b3eac68395f927b7ff02f4106b6cc92a2b395db2813a0605da2771530e5c4fc594eaf5a9a32bf2e42181b6dd90cf3f  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.8|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 21 Dec 2021 10:35:31 GMT
WORKDIR /etc/varnish
# Tue, 21 Dec 2021 10:35:33 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 21 Dec 2021 10:35:33 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Dec 2021 10:35:34 GMT
EXPOSE 80 8443
# Tue, 21 Dec 2021 10:35:35 GMT
CMD []
```

-	Layers:
	-	`sha256:927a35006d93ea08499b57046904046d7926cd76fb17be193e3e74f56d634a08`  
		Last Modified: Tue, 21 Dec 2021 01:48:54 GMT  
		Size: 30.0 MB (30043793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2fa237057a545eaaa1d2005ed3acdefbf217c0e1186f5bc68ca4c0c5a311d6`  
		Last Modified: Tue, 21 Dec 2021 10:37:27 GMT  
		Size: 64.6 MB (64642186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d3a2610175a2cea7772fba94f24c41446ac559e3d93f920dce10b8975fdc34`  
		Last Modified: Tue, 21 Dec 2021 10:37:16 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; 386

```console
$ docker pull varnish@sha256:5ad40751894382694f868022af125c7b5b4bd737d339d465b4a1c175cd41bb2b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102062918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fc599f425f815d23bedac0d4d540e4a345932db7bc20035e03ccea8ee192045`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 02:39:54 GMT
ADD file:0284c10b06ba22560408e1e14c1147887f4302c79dba143277ece2e333d6dcbc in / 
# Thu, 02 Dec 2021 02:39:55 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 14:41:26 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 14:52:24 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.0.8.tgz -o $tmpdir/orig.tgz;     echo "73ed2f465ba3b11680b20a70633fc78da9b3eac68395f927b7ff02f4106b6cc92a2b395db2813a0605da2771530e5c4fc594eaf5a9a32bf2e42181b6dd90cf3f  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.8|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 14:52:25 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 14:52:25 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 02 Dec 2021 14:52:25 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 14:52:26 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 14:52:26 GMT
CMD []
```

-	Layers:
	-	`sha256:2df7932f17d752876c686aa22054692a38e88e182dd7b6a5cca7ffce4ffe6f84`  
		Last Modified: Thu, 02 Dec 2021 02:47:59 GMT  
		Size: 32.4 MB (32380814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6f8f5993208760bfd785dee6370007dde3e7837d9dc7e3cc74206ad6e54b6f`  
		Last Modified: Thu, 02 Dec 2021 14:55:16 GMT  
		Size: 69.7 MB (69681403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1900d954ea8bc8ac629ec212ad0ff3da652ff5189d2138156bb2445aefc20179`  
		Last Modified: Thu, 02 Dec 2021 14:55:01 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; ppc64le

```console
$ docker pull varnish@sha256:85b85d37828bb1349bc6dffa742f97d110d48b08ade48b00e4614db87669821b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.8 MB (99776391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:477f13d57ec581eb6568aee6dc2eaad1148d9fcc2e856cb9a237f5adc4c27574`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 07:21:21 GMT
ADD file:81a93de7f5dcdbb9397c05b9b6bb7dc5a4742119d46faf929b4c6277b02be7a5 in / 
# Thu, 02 Dec 2021 07:21:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 20:55:25 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 21:58:15 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.0.8.tgz -o $tmpdir/orig.tgz;     echo "73ed2f465ba3b11680b20a70633fc78da9b3eac68395f927b7ff02f4106b6cc92a2b395db2813a0605da2771530e5c4fc594eaf5a9a32bf2e42181b6dd90cf3f  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.8|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 21:58:21 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 21:58:22 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 02 Dec 2021 21:58:24 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 21:58:26 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 21:58:28 GMT
CMD []
```

-	Layers:
	-	`sha256:8d46978b233ccedeaa1cbef7248b214991469fa922cc4fbf9916f9d0711d2d2e`  
		Last Modified: Thu, 02 Dec 2021 07:31:43 GMT  
		Size: 35.3 MB (35271379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07dc89dd1f6108b0a247a91d91d5167422d9f447169268fc11f4d289a75f70a6`  
		Last Modified: Thu, 02 Dec 2021 22:00:40 GMT  
		Size: 64.5 MB (64504309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90804dc475998e237ff6f2f044f47b7bca1ae4d009676626f1761c1b44556496`  
		Last Modified: Thu, 02 Dec 2021 22:00:26 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; s390x

```console
$ docker pull varnish@sha256:1a58eec42888f09f1a1c33c632b474197658d4e07d04aa36f581a0254a457ed0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.0 MB (80994821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd2857448b98a5e632f673a99702a81e5cf9f880873cb813e97c3534237fb56b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 07:19:07 GMT
ADD file:9303def035f391c14bdca007751c5061f36fe929d5b3f4d725ce376e25f7dd36 in / 
# Thu, 02 Dec 2021 07:19:09 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 12:47:34 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 12:52:13 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.0.8.tgz -o $tmpdir/orig.tgz;     echo "73ed2f465ba3b11680b20a70633fc78da9b3eac68395f927b7ff02f4106b6cc92a2b395db2813a0605da2771530e5c4fc594eaf5a9a32bf2e42181b6dd90cf3f  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.8|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 12:52:15 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 12:52:15 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 02 Dec 2021 12:52:15 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 12:52:15 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 12:52:15 GMT
CMD []
```

-	Layers:
	-	`sha256:bf2c280d82ca10801fb58bfc3f73029eef17592cbe00e94875cb189bdbac0c5f`  
		Last Modified: Thu, 02 Dec 2021 07:25:12 GMT  
		Size: 29.7 MB (29650954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b1cead4f753add4eee5c4fa71deb8b75b67a36d59deb9b760aa7bc95189a11`  
		Last Modified: Thu, 02 Dec 2021 12:53:33 GMT  
		Size: 51.3 MB (51343165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd72e0b5d5556153d85da35fb2538e849772bf4fdfa087a050284b761e28953`  
		Last Modified: Thu, 02 Dec 2021 12:53:26 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0.8`

```console
$ docker pull varnish@sha256:786e9bd61f197b2720853007c7c507c6bdc71f4e3236e03d35da367a01e2d116
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:6.0.8` - linux; amd64

```console
$ docker pull varnish@sha256:a21d8beb55aa8f902b55a6f773c581dcd6537a8883d0d24b5d32c18f1b662bdb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100572918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58725732895fe16eebccbad29fc67442778d35629b74e64b49b44538eaa3dcfe`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 02:48:20 GMT
ADD file:ece5ff85ca549f0b1e9139d29dcb43a52af672d0591c423e28180f6d8d700ad7 in / 
# Thu, 02 Dec 2021 02:48:21 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 17:48:20 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 17:58:16 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.0.8.tgz -o $tmpdir/orig.tgz;     echo "73ed2f465ba3b11680b20a70633fc78da9b3eac68395f927b7ff02f4106b6cc92a2b395db2813a0605da2771530e5c4fc594eaf5a9a32bf2e42181b6dd90cf3f  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.8|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 17:58:17 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 17:58:17 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 02 Dec 2021 17:58:17 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 17:58:17 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 17:58:18 GMT
CMD []
```

-	Layers:
	-	`sha256:e5ae68f740265288a4888db98d2999a638fdcb6d725f427678814538d253aa4d`  
		Last Modified: Thu, 02 Dec 2021 02:53:46 GMT  
		Size: 31.4 MB (31370221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3cfaf0bcb14454b543ce0498ecb01e3e93089900b28fb13ae862bb38a29a84`  
		Last Modified: Thu, 02 Dec 2021 17:59:42 GMT  
		Size: 69.2 MB (69201997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c37ac8a55c4f5f4a2cb6e64b5198e81377fdfa11ec23d4000d7c90e35edb37`  
		Last Modified: Thu, 02 Dec 2021 17:59:29 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.8` - linux; arm variant v7

```console
$ docker pull varnish@sha256:78c279b4c10a6687be3db34d347f867a234def120a1e06dc418c7f7e44a9c727
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77216753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57d84c4c56a5deeba196ae1f0a545651321f1381d4f6bc472f4495ce898ecfdf`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 09:05:17 GMT
ADD file:97ce5af9ff4fb4002733d5c402ddc01a13e765d31b85bb6525a7fa797b698e10 in / 
# Thu, 02 Dec 2021 09:05:17 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 17:16:05 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 17:34:44 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.0.8.tgz -o $tmpdir/orig.tgz;     echo "73ed2f465ba3b11680b20a70633fc78da9b3eac68395f927b7ff02f4106b6cc92a2b395db2813a0605da2771530e5c4fc594eaf5a9a32bf2e42181b6dd90cf3f  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.8|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 17:34:45 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 17:34:45 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 02 Dec 2021 17:34:46 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 17:34:46 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 17:34:47 GMT
CMD []
```

-	Layers:
	-	`sha256:ba82a1312e1efdcd1cc6eb31cd40358dcec180da31779dac399cba31bf3dc206`  
		Last Modified: Thu, 02 Dec 2021 09:21:03 GMT  
		Size: 26.6 MB (26573192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a26aabdc4af6fcc2f87ffedefcd2035994ad7c44dbfc8ca07bcc82b1fd49ac0`  
		Last Modified: Thu, 02 Dec 2021 17:38:18 GMT  
		Size: 50.6 MB (50642860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2885c8aa3ff49bada1b1b2038107980ee649083c64c42d6534df3bf77cbf35`  
		Last Modified: Thu, 02 Dec 2021 17:37:55 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.8` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:ac60c1e4761cc40d24baa103506086f6f415a4b67f72d02a4342ee7208300669
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94686680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:967bad5c1de22c86008e49361e2caf5e5e47e81271b94caf94047c037d70e1aa`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Dec 2021 01:42:23 GMT
ADD file:986f91febed4aa8e2072081ff8419d52ba2060510822e717086d3b3d9469e4d7 in / 
# Tue, 21 Dec 2021 01:42:24 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:28:06 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Dec 2021 10:35:31 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.0.8.tgz -o $tmpdir/orig.tgz;     echo "73ed2f465ba3b11680b20a70633fc78da9b3eac68395f927b7ff02f4106b6cc92a2b395db2813a0605da2771530e5c4fc594eaf5a9a32bf2e42181b6dd90cf3f  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.8|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 21 Dec 2021 10:35:31 GMT
WORKDIR /etc/varnish
# Tue, 21 Dec 2021 10:35:33 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 21 Dec 2021 10:35:33 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Dec 2021 10:35:34 GMT
EXPOSE 80 8443
# Tue, 21 Dec 2021 10:35:35 GMT
CMD []
```

-	Layers:
	-	`sha256:927a35006d93ea08499b57046904046d7926cd76fb17be193e3e74f56d634a08`  
		Last Modified: Tue, 21 Dec 2021 01:48:54 GMT  
		Size: 30.0 MB (30043793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2fa237057a545eaaa1d2005ed3acdefbf217c0e1186f5bc68ca4c0c5a311d6`  
		Last Modified: Tue, 21 Dec 2021 10:37:27 GMT  
		Size: 64.6 MB (64642186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d3a2610175a2cea7772fba94f24c41446ac559e3d93f920dce10b8975fdc34`  
		Last Modified: Tue, 21 Dec 2021 10:37:16 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.8` - linux; 386

```console
$ docker pull varnish@sha256:5ad40751894382694f868022af125c7b5b4bd737d339d465b4a1c175cd41bb2b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102062918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fc599f425f815d23bedac0d4d540e4a345932db7bc20035e03ccea8ee192045`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 02:39:54 GMT
ADD file:0284c10b06ba22560408e1e14c1147887f4302c79dba143277ece2e333d6dcbc in / 
# Thu, 02 Dec 2021 02:39:55 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 14:41:26 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 14:52:24 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.0.8.tgz -o $tmpdir/orig.tgz;     echo "73ed2f465ba3b11680b20a70633fc78da9b3eac68395f927b7ff02f4106b6cc92a2b395db2813a0605da2771530e5c4fc594eaf5a9a32bf2e42181b6dd90cf3f  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.8|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 14:52:25 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 14:52:25 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 02 Dec 2021 14:52:25 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 14:52:26 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 14:52:26 GMT
CMD []
```

-	Layers:
	-	`sha256:2df7932f17d752876c686aa22054692a38e88e182dd7b6a5cca7ffce4ffe6f84`  
		Last Modified: Thu, 02 Dec 2021 02:47:59 GMT  
		Size: 32.4 MB (32380814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6f8f5993208760bfd785dee6370007dde3e7837d9dc7e3cc74206ad6e54b6f`  
		Last Modified: Thu, 02 Dec 2021 14:55:16 GMT  
		Size: 69.7 MB (69681403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1900d954ea8bc8ac629ec212ad0ff3da652ff5189d2138156bb2445aefc20179`  
		Last Modified: Thu, 02 Dec 2021 14:55:01 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.8` - linux; ppc64le

```console
$ docker pull varnish@sha256:85b85d37828bb1349bc6dffa742f97d110d48b08ade48b00e4614db87669821b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.8 MB (99776391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:477f13d57ec581eb6568aee6dc2eaad1148d9fcc2e856cb9a237f5adc4c27574`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 07:21:21 GMT
ADD file:81a93de7f5dcdbb9397c05b9b6bb7dc5a4742119d46faf929b4c6277b02be7a5 in / 
# Thu, 02 Dec 2021 07:21:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 20:55:25 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 21:58:15 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.0.8.tgz -o $tmpdir/orig.tgz;     echo "73ed2f465ba3b11680b20a70633fc78da9b3eac68395f927b7ff02f4106b6cc92a2b395db2813a0605da2771530e5c4fc594eaf5a9a32bf2e42181b6dd90cf3f  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.8|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 21:58:21 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 21:58:22 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 02 Dec 2021 21:58:24 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 21:58:26 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 21:58:28 GMT
CMD []
```

-	Layers:
	-	`sha256:8d46978b233ccedeaa1cbef7248b214991469fa922cc4fbf9916f9d0711d2d2e`  
		Last Modified: Thu, 02 Dec 2021 07:31:43 GMT  
		Size: 35.3 MB (35271379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07dc89dd1f6108b0a247a91d91d5167422d9f447169268fc11f4d289a75f70a6`  
		Last Modified: Thu, 02 Dec 2021 22:00:40 GMT  
		Size: 64.5 MB (64504309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90804dc475998e237ff6f2f044f47b7bca1ae4d009676626f1761c1b44556496`  
		Last Modified: Thu, 02 Dec 2021 22:00:26 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.8` - linux; s390x

```console
$ docker pull varnish@sha256:1a58eec42888f09f1a1c33c632b474197658d4e07d04aa36f581a0254a457ed0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.0 MB (80994821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd2857448b98a5e632f673a99702a81e5cf9f880873cb813e97c3534237fb56b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 07:19:07 GMT
ADD file:9303def035f391c14bdca007751c5061f36fe929d5b3f4d725ce376e25f7dd36 in / 
# Thu, 02 Dec 2021 07:19:09 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 12:47:34 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 12:52:13 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.0.8.tgz -o $tmpdir/orig.tgz;     echo "73ed2f465ba3b11680b20a70633fc78da9b3eac68395f927b7ff02f4106b6cc92a2b395db2813a0605da2771530e5c4fc594eaf5a9a32bf2e42181b6dd90cf3f  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.8|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 12:52:15 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 12:52:15 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 02 Dec 2021 12:52:15 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 12:52:15 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 12:52:15 GMT
CMD []
```

-	Layers:
	-	`sha256:bf2c280d82ca10801fb58bfc3f73029eef17592cbe00e94875cb189bdbac0c5f`  
		Last Modified: Thu, 02 Dec 2021 07:25:12 GMT  
		Size: 29.7 MB (29650954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b1cead4f753add4eee5c4fa71deb8b75b67a36d59deb9b760aa7bc95189a11`  
		Last Modified: Thu, 02 Dec 2021 12:53:33 GMT  
		Size: 51.3 MB (51343165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd72e0b5d5556153d85da35fb2538e849772bf4fdfa087a050284b761e28953`  
		Last Modified: Thu, 02 Dec 2021 12:53:26 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.6`

```console
$ docker pull varnish@sha256:0e299ff5c2b04a608dd4333c430a8f4e6c78104248bbc413606c45b1e7f804c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:6.6` - linux; amd64

```console
$ docker pull varnish@sha256:4e9a31f9cd3768e94409465bc6a147521426447a500d4cc02b085771f94ceab1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.1 MB (101111892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73d4575ed5fdcfe4eae8cdad180dcc1b6ff651a9fbe51f640ae291cb22eb75c4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 02:48:20 GMT
ADD file:ece5ff85ca549f0b1e9139d29dcb43a52af672d0591c423e28180f6d8d700ad7 in / 
# Thu, 02 Dec 2021 02:48:21 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 17:48:20 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 17:54:45 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.6.1.tgz -o $tmpdir/orig.tgz;     echo "af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.6.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 17:54:46 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 17:54:46 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 02 Dec 2021 17:54:46 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 17:54:47 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 17:54:47 GMT
CMD []
```

-	Layers:
	-	`sha256:e5ae68f740265288a4888db98d2999a638fdcb6d725f427678814538d253aa4d`  
		Last Modified: Thu, 02 Dec 2021 02:53:46 GMT  
		Size: 31.4 MB (31370221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54aafcbd42918f75407dff1904fed8191a04453c65ebc1bb390a504f95dd9b48`  
		Last Modified: Thu, 02 Dec 2021 17:59:15 GMT  
		Size: 69.7 MB (69740968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef06e7e4e4e50154e65169fb5a1998f8896a9269d468dc69292eec6b4d54227`  
		Last Modified: Thu, 02 Dec 2021 17:59:04 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.6` - linux; arm variant v7

```console
$ docker pull varnish@sha256:f05c268f8e8bb687fe1f4f8e8acdb51a3227ed4be5bf83fc697910f0fa90dfb0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.7 MB (77727488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01fcc14c5839bed7878b09ad08adf90226d16a47e2096669fb230457233dd4a2`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 09:05:17 GMT
ADD file:97ce5af9ff4fb4002733d5c402ddc01a13e765d31b85bb6525a7fa797b698e10 in / 
# Thu, 02 Dec 2021 09:05:17 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 17:16:05 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 17:27:59 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.6.1.tgz -o $tmpdir/orig.tgz;     echo "af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.6.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 17:28:00 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 17:28:00 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 02 Dec 2021 17:28:01 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 17:28:01 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 17:28:01 GMT
CMD []
```

-	Layers:
	-	`sha256:ba82a1312e1efdcd1cc6eb31cd40358dcec180da31779dac399cba31bf3dc206`  
		Last Modified: Thu, 02 Dec 2021 09:21:03 GMT  
		Size: 26.6 MB (26573192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85dad9248f0b6f379b3fc0581d83af70ba00e2ad83b7b9fea210fe9e71180748`  
		Last Modified: Thu, 02 Dec 2021 17:37:34 GMT  
		Size: 51.2 MB (51153596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e1f08afc9c3f5a7595f71bd9cddb3790098261476e2001bfa8f056a25fdf73`  
		Last Modified: Thu, 02 Dec 2021 17:37:10 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.6` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:3f5c0ade9623076b6f70af0f9c2e8ed1c5e05e8a26132cbcb69ab332c79d8874
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.2 MB (95201957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c878a4677639eae79f1dc7bdc929e5a01023d410f3a82d7af12be91839296a9`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Dec 2021 01:42:23 GMT
ADD file:986f91febed4aa8e2072081ff8419d52ba2060510822e717086d3b3d9469e4d7 in / 
# Tue, 21 Dec 2021 01:42:24 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:28:06 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Dec 2021 10:33:04 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.6.1.tgz -o $tmpdir/orig.tgz;     echo "af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.6.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 21 Dec 2021 10:33:05 GMT
WORKDIR /etc/varnish
# Tue, 21 Dec 2021 10:33:06 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 21 Dec 2021 10:33:06 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Dec 2021 10:33:07 GMT
EXPOSE 80 8443
# Tue, 21 Dec 2021 10:33:08 GMT
CMD []
```

-	Layers:
	-	`sha256:927a35006d93ea08499b57046904046d7926cd76fb17be193e3e74f56d634a08`  
		Last Modified: Tue, 21 Dec 2021 01:48:54 GMT  
		Size: 30.0 MB (30043793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3132324cb63ca845b64354090627b56cb213f682412e616569edcfff411b0063`  
		Last Modified: Tue, 21 Dec 2021 10:37:01 GMT  
		Size: 65.2 MB (65157463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcddc6003e0c38e0f6b53aa00f16f05a3b2091aadd404eb735e08d104e94fe03`  
		Last Modified: Tue, 21 Dec 2021 10:36:51 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.6` - linux; 386

```console
$ docker pull varnish@sha256:2c1144b3aa8bbebe4de0b386c82cd8c17f34aa8da1a41118f48972ee8c0776b1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.5 MB (102504588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ac112a00fa98d1392dc812b6fa5446c417c8b4f80819896a9e8035ad476aba1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 02:39:54 GMT
ADD file:0284c10b06ba22560408e1e14c1147887f4302c79dba143277ece2e333d6dcbc in / 
# Thu, 02 Dec 2021 02:39:55 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 14:41:26 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 14:48:54 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.6.1.tgz -o $tmpdir/orig.tgz;     echo "af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.6.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 14:48:55 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 14:48:55 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 02 Dec 2021 14:48:55 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 14:48:56 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 14:48:56 GMT
CMD []
```

-	Layers:
	-	`sha256:2df7932f17d752876c686aa22054692a38e88e182dd7b6a5cca7ffce4ffe6f84`  
		Last Modified: Thu, 02 Dec 2021 02:47:59 GMT  
		Size: 32.4 MB (32380814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922c816d4d3f0946beac2d08f5eb0190ec5a80682dc209f8d0329c89b27638d4`  
		Last Modified: Thu, 02 Dec 2021 14:54:43 GMT  
		Size: 70.1 MB (70123075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95fa0cd2f6a540ad99fc42899f545670eebe17aba545ebaed16e3dc88c2e4ba8`  
		Last Modified: Thu, 02 Dec 2021 14:54:22 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.6` - linux; ppc64le

```console
$ docker pull varnish@sha256:5b4892ab3461ddbe3e005f0743fd108f23bd2b5e29ad535ec8eca7ebea149ce7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.3 MB (100286361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9c2cd2e73557a8406f2bef10afbf10709762c0d5ef19fbc0a95de11ae26cd0d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 07:21:21 GMT
ADD file:81a93de7f5dcdbb9397c05b9b6bb7dc5a4742119d46faf929b4c6277b02be7a5 in / 
# Thu, 02 Dec 2021 07:21:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 20:55:25 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 21:40:19 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.6.1.tgz -o $tmpdir/orig.tgz;     echo "af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.6.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 21:40:24 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 21:40:25 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 02 Dec 2021 21:40:28 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 21:40:31 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 21:40:38 GMT
CMD []
```

-	Layers:
	-	`sha256:8d46978b233ccedeaa1cbef7248b214991469fa922cc4fbf9916f9d0711d2d2e`  
		Last Modified: Thu, 02 Dec 2021 07:31:43 GMT  
		Size: 35.3 MB (35271379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0776e5e25a1d33dcf0ac0200fe69c70a222da6eed40bceb51e7425843833e789`  
		Last Modified: Thu, 02 Dec 2021 22:00:09 GMT  
		Size: 65.0 MB (65014280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dd010c4033bde0051434329ac0374d3261fd87e5d9a4dadfe64a52366740e66`  
		Last Modified: Thu, 02 Dec 2021 21:59:55 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.6` - linux; s390x

```console
$ docker pull varnish@sha256:14e377f6877ce74f254ed9ed95d31b7a40d16d4a62a987c4019e65d1d069301d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.7 MB (84737666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b27da94164283f11e04b01eaa1c5e0d71358b3249f3d1448574059b8cd14c53`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 17 Nov 2021 02:42:27 GMT
ADD file:42f73dac307a6a5232e3100f3d3b36e8125f73a4ca504b106e60e2b66d242b2f in / 
# Wed, 17 Nov 2021 02:42:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 12:09:56 GMT
ENV VARNISH_SIZE=100M
# Fri, 19 Nov 2021 02:11:05 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.6.1.tgz -o $tmpdir/orig.tgz;     echo "af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.6.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Fri, 19 Nov 2021 02:11:07 GMT
WORKDIR /etc/varnish
# Fri, 19 Nov 2021 02:11:07 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Fri, 19 Nov 2021 02:11:07 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 19 Nov 2021 02:11:07 GMT
EXPOSE 80 8443
# Fri, 19 Nov 2021 02:11:08 GMT
CMD []
```

-	Layers:
	-	`sha256:8d71e885edf612b507bbdcc48a970548d436b8709eeedfc2c98f6843a214b5e2`  
		Last Modified: Wed, 17 Nov 2021 02:48:25 GMT  
		Size: 29.7 MB (29650960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cbe324e886d9ee47afe369fd7b2c3c3e223f8213f286df5daa395bba36d378f`  
		Last Modified: Fri, 19 Nov 2021 02:12:35 GMT  
		Size: 55.1 MB (55086007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607c8fd5302cec2fa184d34ed2873b257df7dac3ba972aee15614765f9ffa43a`  
		Last Modified: Fri, 19 Nov 2021 02:12:28 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.6-alpine`

```console
$ docker pull varnish@sha256:4c1836081996430a23b736e66ceaa37221580d97ecd0683a47a16ff0e3f09aa6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:6.6-alpine` - linux; amd64

```console
$ docker pull varnish@sha256:452898ec4382082c43e9aad4ad2313939833ac757ed3eedf122dd4107a060862
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.0 MB (57989509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9452c96edc1e2f1f4f52a9471093a1f653d6266bd8a9fae81849688342d1dfcd`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 07:25:45 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 18:27:11 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=6.6.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 18:27:11 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 18:27:11 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Mon, 29 Nov 2021 18:27:12 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 18:27:12 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 18:27:12 GMT
CMD []
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153ae6d73742ceecdf942d8913c25adacffcf7590c180c52467774aae45fbdf8`  
		Last Modified: Mon, 29 Nov 2021 18:31:17 GMT  
		Size: 55.2 MB (55165820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47da88759d700deda407b20295e1fa1b16669b41d326a6ec602f1764725eb339`  
		Last Modified: Mon, 29 Nov 2021 18:31:09 GMT  
		Size: 708.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.6-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:c73adc94b1b1fbee8b0d00ecc03446cbe553ec30d20c232bd24ce69ebb15595c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.8 MB (43831597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6f764f7171682d32f568bcc7a144616e93a442db165eee0f50c65b69b4ebc3d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:41:33 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 21:27:56 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=6.6.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 21:27:57 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 21:27:58 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Mon, 29 Nov 2021 21:27:58 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 21:27:59 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 21:27:59 GMT
CMD []
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45906a707d1a67dd18797169bbfe25bac52a1b464e7f990698da21fddd7475c0`  
		Last Modified: Mon, 29 Nov 2021 21:37:33 GMT  
		Size: 41.4 MB (41392271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740d9723635b34441b27b262933bd4b8418b26b67f4045cc9f64ec89bc227fd3`  
		Last Modified: Mon, 29 Nov 2021 21:37:11 GMT  
		Size: 708.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.6-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:2a37d0c77875b555f8ca6eb95423051dccd662fc043139f3ca0c454b3297c3d0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50731977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97f125861bc75731dc461286c1d1b0a2b17c8e0f205c97df4543729f7a8b7352`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:02:27 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 20:48:16 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=6.6.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 20:48:17 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 20:48:19 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Mon, 29 Nov 2021 20:48:19 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 20:48:20 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 20:48:21 GMT
CMD []
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9a5a9eecb648d857587d324062b4f87bb9dc62e6a4cb827c9e4464961c2e59`  
		Last Modified: Mon, 29 Nov 2021 20:52:51 GMT  
		Size: 48.0 MB (48013567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e736777a13cbd6c9e14db297a5c4bbb132c234eeeff9c10b17cd5452cd362216`  
		Last Modified: Mon, 29 Nov 2021 20:52:44 GMT  
		Size: 710.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.6-alpine` - linux; 386

```console
$ docker pull varnish@sha256:8d0d547249a14cde7e3bd5e01c2a40ddf1ba74cb90d66f5a093034cfff3e55c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58199339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0336cd46aeafd4ae83b0b6dc96d0f1f1614ec9ba408969822994a117199191bc`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:38:42 GMT
ADD file:403428c2903dd9dea10d069185873cb2c2c3149c553797807c69f22aa3d12fe3 in / 
# Fri, 12 Nov 2021 16:38:42 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 20:27:36 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 20:01:00 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=6.6.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 20:01:01 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 20:01:01 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Mon, 29 Nov 2021 20:01:01 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 20:01:01 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 20:01:02 GMT
CMD []
```

-	Layers:
	-	`sha256:5420e0d28c84ecb16748cb90cc6acf8e2a81dab10cb1f674f3eee8533e53c62a`  
		Last Modified: Fri, 12 Nov 2021 16:39:36 GMT  
		Size: 2.8 MB (2830948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d909c7ab2ae0be7fc0e4ae7aa02aa06a2e44ad53f3cff2268bfeed6937c499c3`  
		Last Modified: Mon, 29 Nov 2021 20:02:44 GMT  
		Size: 55.4 MB (55367685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19722b94f50ff8a0a17e55d0b2919cf221589ab013ad66a822669ae094c020de`  
		Last Modified: Mon, 29 Nov 2021 20:02:34 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.6-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:377e24a918f548a09f38a533afdcdecf4d9a30f2286434bce625df8260f06411
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47836328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fdc983240c36081b8a4d544f472904fa029137f9e87f69d41b24b43d0a16ca7`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 21:18:00 GMT
ADD file:4d45063079cb28a34f1e382fddb22f156ac99d5449aa05ed37cb653c1f7b80f2 in / 
# Fri, 12 Nov 2021 21:18:01 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:52:07 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 19:56:23 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=6.6.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 19:56:29 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 19:56:32 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Mon, 29 Nov 2021 19:56:34 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 19:56:35 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 19:56:36 GMT
CMD []
```

-	Layers:
	-	`sha256:72940440c1ab65eca4d38846164719ffde4b147543cc658d041407a925b13368`  
		Last Modified: Fri, 12 Nov 2021 21:19:32 GMT  
		Size: 2.8 MB (2817467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e0a28c63680f4f963ab893db97224b8d2b5ff2d6e06ea1e743d9c3731ebc85`  
		Last Modified: Mon, 29 Nov 2021 20:15:27 GMT  
		Size: 45.0 MB (45018158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7d4295e98da2f81183f70ef0dc76d1d3490a26ffcbf6354434e1651d44ae3c`  
		Last Modified: Mon, 29 Nov 2021 20:15:19 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.6-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:e1001918850b37c9a482e47544f06bfb1808f199cd9d7bf5e33d35c132ba702a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.4 MB (46372307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5888cbaa2a9d39840aedcdd59b0feb27f3687cbcd2be29caff8898de3799d2a6`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:41:35 GMT
ADD file:7e0cf02b3f015b1a0f867c03b2902b85f2140be1cee7af63c23f367a487e4577 in / 
# Fri, 12 Nov 2021 16:41:36 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 22:10:22 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 20:08:19 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=6.6.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 20:08:20 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 20:08:20 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Mon, 29 Nov 2021 20:08:20 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 20:08:21 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 20:08:21 GMT
CMD []
```

-	Layers:
	-	`sha256:817a13b0e05928f7491adbf1d2cf261ec35079112247bd03469bbe31156aca7c`  
		Last Modified: Fri, 12 Nov 2021 16:42:44 GMT  
		Size: 2.6 MB (2609278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2b2b1073e64d39da57603b96e9b9171e48a505e0e09a02cfd3e29658a2a58a`  
		Last Modified: Mon, 29 Nov 2021 20:11:46 GMT  
		Size: 43.8 MB (43762322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35ef3ae417d6531198e3ab2b6a00ef57d1474d0dde453fff48250ed6cf22703`  
		Last Modified: Mon, 29 Nov 2021 20:11:40 GMT  
		Size: 707.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.6.1`

```console
$ docker pull varnish@sha256:0e299ff5c2b04a608dd4333c430a8f4e6c78104248bbc413606c45b1e7f804c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:6.6.1` - linux; amd64

```console
$ docker pull varnish@sha256:4e9a31f9cd3768e94409465bc6a147521426447a500d4cc02b085771f94ceab1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.1 MB (101111892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73d4575ed5fdcfe4eae8cdad180dcc1b6ff651a9fbe51f640ae291cb22eb75c4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 02:48:20 GMT
ADD file:ece5ff85ca549f0b1e9139d29dcb43a52af672d0591c423e28180f6d8d700ad7 in / 
# Thu, 02 Dec 2021 02:48:21 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 17:48:20 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 17:54:45 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.6.1.tgz -o $tmpdir/orig.tgz;     echo "af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.6.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 17:54:46 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 17:54:46 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 02 Dec 2021 17:54:46 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 17:54:47 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 17:54:47 GMT
CMD []
```

-	Layers:
	-	`sha256:e5ae68f740265288a4888db98d2999a638fdcb6d725f427678814538d253aa4d`  
		Last Modified: Thu, 02 Dec 2021 02:53:46 GMT  
		Size: 31.4 MB (31370221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54aafcbd42918f75407dff1904fed8191a04453c65ebc1bb390a504f95dd9b48`  
		Last Modified: Thu, 02 Dec 2021 17:59:15 GMT  
		Size: 69.7 MB (69740968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef06e7e4e4e50154e65169fb5a1998f8896a9269d468dc69292eec6b4d54227`  
		Last Modified: Thu, 02 Dec 2021 17:59:04 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.6.1` - linux; arm variant v7

```console
$ docker pull varnish@sha256:f05c268f8e8bb687fe1f4f8e8acdb51a3227ed4be5bf83fc697910f0fa90dfb0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.7 MB (77727488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01fcc14c5839bed7878b09ad08adf90226d16a47e2096669fb230457233dd4a2`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 09:05:17 GMT
ADD file:97ce5af9ff4fb4002733d5c402ddc01a13e765d31b85bb6525a7fa797b698e10 in / 
# Thu, 02 Dec 2021 09:05:17 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 17:16:05 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 17:27:59 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.6.1.tgz -o $tmpdir/orig.tgz;     echo "af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.6.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 17:28:00 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 17:28:00 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 02 Dec 2021 17:28:01 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 17:28:01 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 17:28:01 GMT
CMD []
```

-	Layers:
	-	`sha256:ba82a1312e1efdcd1cc6eb31cd40358dcec180da31779dac399cba31bf3dc206`  
		Last Modified: Thu, 02 Dec 2021 09:21:03 GMT  
		Size: 26.6 MB (26573192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85dad9248f0b6f379b3fc0581d83af70ba00e2ad83b7b9fea210fe9e71180748`  
		Last Modified: Thu, 02 Dec 2021 17:37:34 GMT  
		Size: 51.2 MB (51153596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e1f08afc9c3f5a7595f71bd9cddb3790098261476e2001bfa8f056a25fdf73`  
		Last Modified: Thu, 02 Dec 2021 17:37:10 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.6.1` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:3f5c0ade9623076b6f70af0f9c2e8ed1c5e05e8a26132cbcb69ab332c79d8874
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.2 MB (95201957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c878a4677639eae79f1dc7bdc929e5a01023d410f3a82d7af12be91839296a9`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Dec 2021 01:42:23 GMT
ADD file:986f91febed4aa8e2072081ff8419d52ba2060510822e717086d3b3d9469e4d7 in / 
# Tue, 21 Dec 2021 01:42:24 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:28:06 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Dec 2021 10:33:04 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.6.1.tgz -o $tmpdir/orig.tgz;     echo "af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.6.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 21 Dec 2021 10:33:05 GMT
WORKDIR /etc/varnish
# Tue, 21 Dec 2021 10:33:06 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 21 Dec 2021 10:33:06 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Dec 2021 10:33:07 GMT
EXPOSE 80 8443
# Tue, 21 Dec 2021 10:33:08 GMT
CMD []
```

-	Layers:
	-	`sha256:927a35006d93ea08499b57046904046d7926cd76fb17be193e3e74f56d634a08`  
		Last Modified: Tue, 21 Dec 2021 01:48:54 GMT  
		Size: 30.0 MB (30043793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3132324cb63ca845b64354090627b56cb213f682412e616569edcfff411b0063`  
		Last Modified: Tue, 21 Dec 2021 10:37:01 GMT  
		Size: 65.2 MB (65157463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcddc6003e0c38e0f6b53aa00f16f05a3b2091aadd404eb735e08d104e94fe03`  
		Last Modified: Tue, 21 Dec 2021 10:36:51 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.6.1` - linux; 386

```console
$ docker pull varnish@sha256:2c1144b3aa8bbebe4de0b386c82cd8c17f34aa8da1a41118f48972ee8c0776b1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.5 MB (102504588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ac112a00fa98d1392dc812b6fa5446c417c8b4f80819896a9e8035ad476aba1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 02:39:54 GMT
ADD file:0284c10b06ba22560408e1e14c1147887f4302c79dba143277ece2e333d6dcbc in / 
# Thu, 02 Dec 2021 02:39:55 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 14:41:26 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 14:48:54 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.6.1.tgz -o $tmpdir/orig.tgz;     echo "af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.6.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 14:48:55 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 14:48:55 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 02 Dec 2021 14:48:55 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 14:48:56 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 14:48:56 GMT
CMD []
```

-	Layers:
	-	`sha256:2df7932f17d752876c686aa22054692a38e88e182dd7b6a5cca7ffce4ffe6f84`  
		Last Modified: Thu, 02 Dec 2021 02:47:59 GMT  
		Size: 32.4 MB (32380814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922c816d4d3f0946beac2d08f5eb0190ec5a80682dc209f8d0329c89b27638d4`  
		Last Modified: Thu, 02 Dec 2021 14:54:43 GMT  
		Size: 70.1 MB (70123075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95fa0cd2f6a540ad99fc42899f545670eebe17aba545ebaed16e3dc88c2e4ba8`  
		Last Modified: Thu, 02 Dec 2021 14:54:22 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.6.1` - linux; ppc64le

```console
$ docker pull varnish@sha256:5b4892ab3461ddbe3e005f0743fd108f23bd2b5e29ad535ec8eca7ebea149ce7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.3 MB (100286361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9c2cd2e73557a8406f2bef10afbf10709762c0d5ef19fbc0a95de11ae26cd0d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 07:21:21 GMT
ADD file:81a93de7f5dcdbb9397c05b9b6bb7dc5a4742119d46faf929b4c6277b02be7a5 in / 
# Thu, 02 Dec 2021 07:21:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 20:55:25 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 21:40:19 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.6.1.tgz -o $tmpdir/orig.tgz;     echo "af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.6.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 21:40:24 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 21:40:25 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 02 Dec 2021 21:40:28 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 21:40:31 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 21:40:38 GMT
CMD []
```

-	Layers:
	-	`sha256:8d46978b233ccedeaa1cbef7248b214991469fa922cc4fbf9916f9d0711d2d2e`  
		Last Modified: Thu, 02 Dec 2021 07:31:43 GMT  
		Size: 35.3 MB (35271379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0776e5e25a1d33dcf0ac0200fe69c70a222da6eed40bceb51e7425843833e789`  
		Last Modified: Thu, 02 Dec 2021 22:00:09 GMT  
		Size: 65.0 MB (65014280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dd010c4033bde0051434329ac0374d3261fd87e5d9a4dadfe64a52366740e66`  
		Last Modified: Thu, 02 Dec 2021 21:59:55 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.6.1` - linux; s390x

```console
$ docker pull varnish@sha256:14e377f6877ce74f254ed9ed95d31b7a40d16d4a62a987c4019e65d1d069301d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.7 MB (84737666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b27da94164283f11e04b01eaa1c5e0d71358b3249f3d1448574059b8cd14c53`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 17 Nov 2021 02:42:27 GMT
ADD file:42f73dac307a6a5232e3100f3d3b36e8125f73a4ca504b106e60e2b66d242b2f in / 
# Wed, 17 Nov 2021 02:42:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 12:09:56 GMT
ENV VARNISH_SIZE=100M
# Fri, 19 Nov 2021 02:11:05 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.6.1.tgz -o $tmpdir/orig.tgz;     echo "af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.6.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Fri, 19 Nov 2021 02:11:07 GMT
WORKDIR /etc/varnish
# Fri, 19 Nov 2021 02:11:07 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Fri, 19 Nov 2021 02:11:07 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 19 Nov 2021 02:11:07 GMT
EXPOSE 80 8443
# Fri, 19 Nov 2021 02:11:08 GMT
CMD []
```

-	Layers:
	-	`sha256:8d71e885edf612b507bbdcc48a970548d436b8709eeedfc2c98f6843a214b5e2`  
		Last Modified: Wed, 17 Nov 2021 02:48:25 GMT  
		Size: 29.7 MB (29650960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cbe324e886d9ee47afe369fd7b2c3c3e223f8213f286df5daa395bba36d378f`  
		Last Modified: Fri, 19 Nov 2021 02:12:35 GMT  
		Size: 55.1 MB (55086007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607c8fd5302cec2fa184d34ed2873b257df7dac3ba972aee15614765f9ffa43a`  
		Last Modified: Fri, 19 Nov 2021 02:12:28 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.6.1-alpine`

```console
$ docker pull varnish@sha256:4c1836081996430a23b736e66ceaa37221580d97ecd0683a47a16ff0e3f09aa6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:6.6.1-alpine` - linux; amd64

```console
$ docker pull varnish@sha256:452898ec4382082c43e9aad4ad2313939833ac757ed3eedf122dd4107a060862
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.0 MB (57989509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9452c96edc1e2f1f4f52a9471093a1f653d6266bd8a9fae81849688342d1dfcd`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 07:25:45 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 18:27:11 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=6.6.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 18:27:11 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 18:27:11 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Mon, 29 Nov 2021 18:27:12 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 18:27:12 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 18:27:12 GMT
CMD []
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153ae6d73742ceecdf942d8913c25adacffcf7590c180c52467774aae45fbdf8`  
		Last Modified: Mon, 29 Nov 2021 18:31:17 GMT  
		Size: 55.2 MB (55165820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47da88759d700deda407b20295e1fa1b16669b41d326a6ec602f1764725eb339`  
		Last Modified: Mon, 29 Nov 2021 18:31:09 GMT  
		Size: 708.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.6.1-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:c73adc94b1b1fbee8b0d00ecc03446cbe553ec30d20c232bd24ce69ebb15595c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.8 MB (43831597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6f764f7171682d32f568bcc7a144616e93a442db165eee0f50c65b69b4ebc3d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:41:33 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 21:27:56 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=6.6.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 21:27:57 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 21:27:58 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Mon, 29 Nov 2021 21:27:58 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 21:27:59 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 21:27:59 GMT
CMD []
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45906a707d1a67dd18797169bbfe25bac52a1b464e7f990698da21fddd7475c0`  
		Last Modified: Mon, 29 Nov 2021 21:37:33 GMT  
		Size: 41.4 MB (41392271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740d9723635b34441b27b262933bd4b8418b26b67f4045cc9f64ec89bc227fd3`  
		Last Modified: Mon, 29 Nov 2021 21:37:11 GMT  
		Size: 708.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:2a37d0c77875b555f8ca6eb95423051dccd662fc043139f3ca0c454b3297c3d0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50731977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97f125861bc75731dc461286c1d1b0a2b17c8e0f205c97df4543729f7a8b7352`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:02:27 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 20:48:16 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=6.6.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 20:48:17 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 20:48:19 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Mon, 29 Nov 2021 20:48:19 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 20:48:20 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 20:48:21 GMT
CMD []
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9a5a9eecb648d857587d324062b4f87bb9dc62e6a4cb827c9e4464961c2e59`  
		Last Modified: Mon, 29 Nov 2021 20:52:51 GMT  
		Size: 48.0 MB (48013567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e736777a13cbd6c9e14db297a5c4bbb132c234eeeff9c10b17cd5452cd362216`  
		Last Modified: Mon, 29 Nov 2021 20:52:44 GMT  
		Size: 710.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.6.1-alpine` - linux; 386

```console
$ docker pull varnish@sha256:8d0d547249a14cde7e3bd5e01c2a40ddf1ba74cb90d66f5a093034cfff3e55c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58199339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0336cd46aeafd4ae83b0b6dc96d0f1f1614ec9ba408969822994a117199191bc`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:38:42 GMT
ADD file:403428c2903dd9dea10d069185873cb2c2c3149c553797807c69f22aa3d12fe3 in / 
# Fri, 12 Nov 2021 16:38:42 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 20:27:36 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 20:01:00 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=6.6.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 20:01:01 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 20:01:01 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Mon, 29 Nov 2021 20:01:01 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 20:01:01 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 20:01:02 GMT
CMD []
```

-	Layers:
	-	`sha256:5420e0d28c84ecb16748cb90cc6acf8e2a81dab10cb1f674f3eee8533e53c62a`  
		Last Modified: Fri, 12 Nov 2021 16:39:36 GMT  
		Size: 2.8 MB (2830948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d909c7ab2ae0be7fc0e4ae7aa02aa06a2e44ad53f3cff2268bfeed6937c499c3`  
		Last Modified: Mon, 29 Nov 2021 20:02:44 GMT  
		Size: 55.4 MB (55367685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19722b94f50ff8a0a17e55d0b2919cf221589ab013ad66a822669ae094c020de`  
		Last Modified: Mon, 29 Nov 2021 20:02:34 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.6.1-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:377e24a918f548a09f38a533afdcdecf4d9a30f2286434bce625df8260f06411
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47836328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fdc983240c36081b8a4d544f472904fa029137f9e87f69d41b24b43d0a16ca7`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 21:18:00 GMT
ADD file:4d45063079cb28a34f1e382fddb22f156ac99d5449aa05ed37cb653c1f7b80f2 in / 
# Fri, 12 Nov 2021 21:18:01 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:52:07 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 19:56:23 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=6.6.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 19:56:29 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 19:56:32 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Mon, 29 Nov 2021 19:56:34 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 19:56:35 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 19:56:36 GMT
CMD []
```

-	Layers:
	-	`sha256:72940440c1ab65eca4d38846164719ffde4b147543cc658d041407a925b13368`  
		Last Modified: Fri, 12 Nov 2021 21:19:32 GMT  
		Size: 2.8 MB (2817467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e0a28c63680f4f963ab893db97224b8d2b5ff2d6e06ea1e743d9c3731ebc85`  
		Last Modified: Mon, 29 Nov 2021 20:15:27 GMT  
		Size: 45.0 MB (45018158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7d4295e98da2f81183f70ef0dc76d1d3490a26ffcbf6354434e1651d44ae3c`  
		Last Modified: Mon, 29 Nov 2021 20:15:19 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.6.1-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:e1001918850b37c9a482e47544f06bfb1808f199cd9d7bf5e33d35c132ba702a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.4 MB (46372307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5888cbaa2a9d39840aedcdd59b0feb27f3687cbcd2be29caff8898de3799d2a6`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:41:35 GMT
ADD file:7e0cf02b3f015b1a0f867c03b2902b85f2140be1cee7af63c23f367a487e4577 in / 
# Fri, 12 Nov 2021 16:41:36 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 22:10:22 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 20:08:19 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=6.6.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 20:08:20 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 20:08:20 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Mon, 29 Nov 2021 20:08:20 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 20:08:21 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 20:08:21 GMT
CMD []
```

-	Layers:
	-	`sha256:817a13b0e05928f7491adbf1d2cf261ec35079112247bd03469bbe31156aca7c`  
		Last Modified: Fri, 12 Nov 2021 16:42:44 GMT  
		Size: 2.6 MB (2609278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2b2b1073e64d39da57603b96e9b9171e48a505e0e09a02cfd3e29658a2a58a`  
		Last Modified: Mon, 29 Nov 2021 20:11:46 GMT  
		Size: 43.8 MB (43762322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35ef3ae417d6531198e3ab2b6a00ef57d1474d0dde453fff48250ed6cf22703`  
		Last Modified: Mon, 29 Nov 2021 20:11:40 GMT  
		Size: 707.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.0`

```console
$ docker pull varnish@sha256:d81f3e0cb09821ee06c6e1c3dde09adda1db842bb97548c6431e98f3f770d927
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:7.0` - linux; amd64

```console
$ docker pull varnish@sha256:ae959bdd6bb300bdf4ab4667d40b0a3bd7805cb398668446c619b484d0538c69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101191056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a30574a32f9387bfb3e1de6a5a9bf2f8c747befabc15268836a09bba431edc30`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 02:48:20 GMT
ADD file:ece5ff85ca549f0b1e9139d29dcb43a52af672d0591c423e28180f6d8d700ad7 in / 
# Thu, 02 Dec 2021 02:48:21 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 17:48:20 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 17:51:31 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-7.0.1.tgz -o $tmpdir/orig.tgz;     echo "7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 17:51:32 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 17:51:32 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 02 Dec 2021 17:51:33 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 17:51:33 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 17:51:33 GMT
CMD []
```

-	Layers:
	-	`sha256:e5ae68f740265288a4888db98d2999a638fdcb6d725f427678814538d253aa4d`  
		Last Modified: Thu, 02 Dec 2021 02:53:46 GMT  
		Size: 31.4 MB (31370221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12826beb2fa2a9fd22ca8cf0048dc3d9e93dda923855bbf2f9edc2eac7d2db7`  
		Last Modified: Thu, 02 Dec 2021 17:58:48 GMT  
		Size: 69.8 MB (69820363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25909d0f31444a52569da07a6ce274b76d41f6bf139bb4a55291c544ad04705a`  
		Last Modified: Thu, 02 Dec 2021 17:58:37 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0` - linux; arm variant v7

```console
$ docker pull varnish@sha256:ed282cf2f85b7f88b869454bd6ce98f50ea8c4aa216a79f14665af7de24c47eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.8 MB (77812722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbda4c98640add6594c969787d60f2ff0737148b1126e295c7550b48fd59887d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 09:05:17 GMT
ADD file:97ce5af9ff4fb4002733d5c402ddc01a13e765d31b85bb6525a7fa797b698e10 in / 
# Thu, 02 Dec 2021 09:05:17 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 17:16:05 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 17:21:51 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-7.0.1.tgz -o $tmpdir/orig.tgz;     echo "7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 17:21:52 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 17:21:53 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 02 Dec 2021 17:21:53 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 17:21:54 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 17:21:54 GMT
CMD []
```

-	Layers:
	-	`sha256:ba82a1312e1efdcd1cc6eb31cd40358dcec180da31779dac399cba31bf3dc206`  
		Last Modified: Thu, 02 Dec 2021 09:21:03 GMT  
		Size: 26.6 MB (26573192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a7af23f33d5037abbe717474bce6f137fdf6db1852beb948bcff91135ffabc`  
		Last Modified: Thu, 02 Dec 2021 17:36:44 GMT  
		Size: 51.2 MB (51239056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9fda28a9f74fe318d52ac4025f63aefdb4ff683eaed6debe26e8af22606f7d`  
		Last Modified: Thu, 02 Dec 2021 17:36:16 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:61956ab15ae49e1d6900db09c616e4a5359341846205221fec7f6c0920cd3d74
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 MB (95289331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4b5de96371e693462f2885e1598467d53e46b15f8feb3d1e582f425e794d011`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Dec 2021 01:42:23 GMT
ADD file:986f91febed4aa8e2072081ff8419d52ba2060510822e717086d3b3d9469e4d7 in / 
# Tue, 21 Dec 2021 01:42:24 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:28:06 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Dec 2021 10:30:29 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-7.0.1.tgz -o $tmpdir/orig.tgz;     echo "7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 21 Dec 2021 10:30:29 GMT
WORKDIR /etc/varnish
# Tue, 21 Dec 2021 10:30:31 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 21 Dec 2021 10:30:31 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Dec 2021 10:30:32 GMT
EXPOSE 80 8443
# Tue, 21 Dec 2021 10:30:33 GMT
CMD []
```

-	Layers:
	-	`sha256:927a35006d93ea08499b57046904046d7926cd76fb17be193e3e74f56d634a08`  
		Last Modified: Tue, 21 Dec 2021 01:48:54 GMT  
		Size: 30.0 MB (30043793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7879c8db25efa15fd67c52352319b5decba8751ce82fc464e491208b56b6126c`  
		Last Modified: Tue, 21 Dec 2021 10:36:33 GMT  
		Size: 65.2 MB (65245064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3969df205cd59ced08fbbf1f1648394f1c621bfe1511d5ae8601239a07be49ed`  
		Last Modified: Tue, 21 Dec 2021 10:36:24 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0` - linux; 386

```console
$ docker pull varnish@sha256:b5711e2756437ce78ea84aa10ad810b1efc436055e26685ad1f8fd2d7b6917e2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.6 MB (102578231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c0cdb20dcbf11013ece2af89e3a9fa6a032513d1fbbc32e25388779c199b545`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 02:39:54 GMT
ADD file:0284c10b06ba22560408e1e14c1147887f4302c79dba143277ece2e333d6dcbc in / 
# Thu, 02 Dec 2021 02:39:55 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 14:41:26 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 14:45:23 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-7.0.1.tgz -o $tmpdir/orig.tgz;     echo "7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 14:45:24 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 14:45:25 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 02 Dec 2021 14:45:25 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 14:45:25 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 14:45:26 GMT
CMD []
```

-	Layers:
	-	`sha256:2df7932f17d752876c686aa22054692a38e88e182dd7b6a5cca7ffce4ffe6f84`  
		Last Modified: Thu, 02 Dec 2021 02:47:59 GMT  
		Size: 32.4 MB (32380814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4532a2822b9d5322c71f3791db81585df1f7fd7698d94c628b4a89789ab06d`  
		Last Modified: Thu, 02 Dec 2021 14:53:57 GMT  
		Size: 70.2 MB (70196944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43edf33f023e899d92eb9fb6d8b922f9e55ccaaf71daf98d429b3cd9a22610aa`  
		Last Modified: Thu, 02 Dec 2021 14:53:37 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0` - linux; ppc64le

```console
$ docker pull varnish@sha256:2c6433bcdfb8f6840987b269f0befb55f24b50e4d16512c54018fd26ef2c4117
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.4 MB (100360511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f76b57f61628753fe997c625800c5f45636b443a164d95dc38a46ac6b3730f1b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 07:21:21 GMT
ADD file:81a93de7f5dcdbb9397c05b9b6bb7dc5a4742119d46faf929b4c6277b02be7a5 in / 
# Thu, 02 Dec 2021 07:21:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 20:55:25 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 21:22:29 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-7.0.1.tgz -o $tmpdir/orig.tgz;     echo "7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 21:22:37 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 21:22:39 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 02 Dec 2021 21:22:41 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 21:22:43 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 21:22:45 GMT
CMD []
```

-	Layers:
	-	`sha256:8d46978b233ccedeaa1cbef7248b214991469fa922cc4fbf9916f9d0711d2d2e`  
		Last Modified: Thu, 02 Dec 2021 07:31:43 GMT  
		Size: 35.3 MB (35271379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a877f42cdd8c7663f7ff10b41702a657bf404827b4ecad08e33487a7b8879b`  
		Last Modified: Thu, 02 Dec 2021 21:59:36 GMT  
		Size: 65.1 MB (65088657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad6570cd65bc0a559262f22219716908f7b28ffd1cbd93d9bcdcde970371752`  
		Last Modified: Thu, 02 Dec 2021 21:59:22 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0` - linux; s390x

```console
$ docker pull varnish@sha256:de1bbc824a6aacfadb8414d3273e4a1ab2c2b49a7b4a880de6e64558266db2f7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.6 MB (81633677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9872cee508e48131bb3424959486542cd81d0eaec0d7c9747e58c90b16c4cb4f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 07:19:07 GMT
ADD file:9303def035f391c14bdca007751c5061f36fe929d5b3f4d725ce376e25f7dd36 in / 
# Thu, 02 Dec 2021 07:19:09 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 12:47:34 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 12:49:19 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-7.0.1.tgz -o $tmpdir/orig.tgz;     echo "7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 12:49:21 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 12:49:21 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 02 Dec 2021 12:49:21 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 12:49:21 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 12:49:21 GMT
CMD []
```

-	Layers:
	-	`sha256:bf2c280d82ca10801fb58bfc3f73029eef17592cbe00e94875cb189bdbac0c5f`  
		Last Modified: Thu, 02 Dec 2021 07:25:12 GMT  
		Size: 29.7 MB (29650954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea009950cddf65d0ad4b52a5ae1891b850f677718911376605822e794733ced`  
		Last Modified: Thu, 02 Dec 2021 12:53:09 GMT  
		Size: 52.0 MB (51982250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0bbe1910546c0494957b3da3bf63782f4d3786641b32c0c54d8ff8607ecfb5`  
		Last Modified: Thu, 02 Dec 2021 12:53:02 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.0-alpine`

```console
$ docker pull varnish@sha256:f87e507197e30345d94738e81eb3724707c42fc2629881019066d37028019f7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:7.0-alpine` - linux; amd64

```console
$ docker pull varnish@sha256:e6f6804aecc2fb6b091c54021c1773b77968d798293d41ab3ee46f5c00a58bb1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.4 MB (58362658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e7e9599575e47151d14b79975fd45baf80559233e36487f2ce8bbe0a941ce68`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 07:25:45 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 18:23:42 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 18:23:42 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 18:23:42 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Mon, 29 Nov 2021 18:23:42 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 18:23:43 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 18:23:43 GMT
CMD []
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf619492e89f6485a3ba5e7cb6807f6f35a59e5715d4bffcb692cfecddeefbd8`  
		Last Modified: Mon, 29 Nov 2021 18:30:34 GMT  
		Size: 55.5 MB (55539197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a667c3f673f5f288f2ff0a45cd4743280d929515d6979127e0cb9f843854d03`  
		Last Modified: Mon, 29 Nov 2021 18:30:26 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:0a8a4359542a0d380e8caff6957abd147ba3e0d4d0f81291a2680f915fc4418e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44177096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efb40b53aee89e6abc8b6707b45a06124ad2bda4a6ce63c73b8c54ff9f4f310b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:41:33 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 21:25:11 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 21:25:12 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 21:25:13 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Mon, 29 Nov 2021 21:25:13 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 21:25:13 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 21:25:14 GMT
CMD []
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ba0a88317201e7b894f07e0179e31e58105e7f86b5716079c72f20d505e90d`  
		Last Modified: Mon, 29 Nov 2021 21:36:51 GMT  
		Size: 41.7 MB (41737996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d68e43dcc838fa62cef86b564038a9ebf4b4511e841577b9ad44a6a40e653e56`  
		Last Modified: Mon, 29 Nov 2021 21:36:29 GMT  
		Size: 482.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:33a0b3a7ab60e096fee91372231b338f2256b92e1030b6e40c1cd0046b72841e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51095315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7cd53e93e2c30ec59c3d576f21316d000c835291752add2060586a1047d3f85`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:02:27 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 20:44:40 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 20:44:40 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 20:44:42 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Mon, 29 Nov 2021 20:44:42 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 20:44:43 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 20:44:44 GMT
CMD []
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed53609c137cea4c70e37bf852c4b51b6baa5e8d2a5d4f6dd5fff316ab310f78`  
		Last Modified: Mon, 29 Nov 2021 20:52:04 GMT  
		Size: 48.4 MB (48377136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99915de3f6477a815b3567ff58bc0b27f2c926cff1dbd04685aa00135003ea0`  
		Last Modified: Mon, 29 Nov 2021 20:51:57 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0-alpine` - linux; 386

```console
$ docker pull varnish@sha256:41415e58f6a0abfb75fc6d924cd4b8e695be23e29697990bd1b5652c50c38125
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.6 MB (58572214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a0be743f31821cf8c667a0bbda63169351f08c76d76f119573bdf4366721063`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:38:42 GMT
ADD file:403428c2903dd9dea10d069185873cb2c2c3149c553797807c69f22aa3d12fe3 in / 
# Fri, 12 Nov 2021 16:38:42 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 20:27:36 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 19:59:18 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 19:59:19 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 19:59:19 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Mon, 29 Nov 2021 19:59:19 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 19:59:20 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 19:59:20 GMT
CMD []
```

-	Layers:
	-	`sha256:5420e0d28c84ecb16748cb90cc6acf8e2a81dab10cb1f674f3eee8533e53c62a`  
		Last Modified: Fri, 12 Nov 2021 16:39:36 GMT  
		Size: 2.8 MB (2830948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a847bbc8f41c777fb2d9bb80d681e74aff97c1d7b641dc784f50d2f15e65878`  
		Last Modified: Mon, 29 Nov 2021 20:02:17 GMT  
		Size: 55.7 MB (55740787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de19c3037a0843a385ef2b761144a16e7b2928588ad15b9d3c8a55e4271c7d49`  
		Last Modified: Mon, 29 Nov 2021 20:02:07 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:3dbc09408d5de96ed2e1da8ee6839b6d2d27d2a6b61461af2dfd979800c96ae4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48217424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf9c543a6c0fc8cebf02f61bc86908cdfd0336e14d49f4585f0b66516aeb8824`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 21:18:00 GMT
ADD file:4d45063079cb28a34f1e382fddb22f156ac99d5449aa05ed37cb653c1f7b80f2 in / 
# Fri, 12 Nov 2021 21:18:01 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:52:07 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 19:33:01 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 19:33:14 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 19:33:16 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Mon, 29 Nov 2021 19:33:20 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 19:33:24 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 19:33:26 GMT
CMD []
```

-	Layers:
	-	`sha256:72940440c1ab65eca4d38846164719ffde4b147543cc658d041407a925b13368`  
		Last Modified: Fri, 12 Nov 2021 21:19:32 GMT  
		Size: 2.8 MB (2817467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fee0663614f072189bcfe90801176e82e4b095b43d6669338848e513113a6b`  
		Last Modified: Mon, 29 Nov 2021 20:14:35 GMT  
		Size: 45.4 MB (45399475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415be876b654e4417228f66afdf87a6f7fb9eb42f7b4c56e20a48c5cf82e155b`  
		Last Modified: Mon, 29 Nov 2021 20:14:24 GMT  
		Size: 482.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:fc3bcee94e4ebed0aeb20e8452bf251168c054aba104ec73cfe2eef09f4e8493
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46683739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94b29bebe019d754443456933a8ab78ec41609ba82475054712204df54da7729`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:41:35 GMT
ADD file:7e0cf02b3f015b1a0f867c03b2902b85f2140be1cee7af63c23f367a487e4577 in / 
# Fri, 12 Nov 2021 16:41:36 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 22:10:22 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 20:07:02 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 20:07:03 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 20:07:03 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Mon, 29 Nov 2021 20:07:03 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 20:07:03 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 20:07:04 GMT
CMD []
```

-	Layers:
	-	`sha256:817a13b0e05928f7491adbf1d2cf261ec35079112247bd03469bbe31156aca7c`  
		Last Modified: Fri, 12 Nov 2021 16:42:44 GMT  
		Size: 2.6 MB (2609278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd4ecc3a23e099fd1b2190632241b2eb90449a80f21c20aea2dc403e49b660e`  
		Last Modified: Mon, 29 Nov 2021 20:11:28 GMT  
		Size: 44.1 MB (44073983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5949a7063bbe02e339a90c74121063f6f7d783927a93059408bbb4112f6d86de`  
		Last Modified: Mon, 29 Nov 2021 20:11:23 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.0.1`

```console
$ docker pull varnish@sha256:d81f3e0cb09821ee06c6e1c3dde09adda1db842bb97548c6431e98f3f770d927
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:7.0.1` - linux; amd64

```console
$ docker pull varnish@sha256:ae959bdd6bb300bdf4ab4667d40b0a3bd7805cb398668446c619b484d0538c69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101191056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a30574a32f9387bfb3e1de6a5a9bf2f8c747befabc15268836a09bba431edc30`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 02:48:20 GMT
ADD file:ece5ff85ca549f0b1e9139d29dcb43a52af672d0591c423e28180f6d8d700ad7 in / 
# Thu, 02 Dec 2021 02:48:21 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 17:48:20 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 17:51:31 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-7.0.1.tgz -o $tmpdir/orig.tgz;     echo "7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 17:51:32 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 17:51:32 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 02 Dec 2021 17:51:33 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 17:51:33 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 17:51:33 GMT
CMD []
```

-	Layers:
	-	`sha256:e5ae68f740265288a4888db98d2999a638fdcb6d725f427678814538d253aa4d`  
		Last Modified: Thu, 02 Dec 2021 02:53:46 GMT  
		Size: 31.4 MB (31370221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12826beb2fa2a9fd22ca8cf0048dc3d9e93dda923855bbf2f9edc2eac7d2db7`  
		Last Modified: Thu, 02 Dec 2021 17:58:48 GMT  
		Size: 69.8 MB (69820363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25909d0f31444a52569da07a6ce274b76d41f6bf139bb4a55291c544ad04705a`  
		Last Modified: Thu, 02 Dec 2021 17:58:37 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0.1` - linux; arm variant v7

```console
$ docker pull varnish@sha256:ed282cf2f85b7f88b869454bd6ce98f50ea8c4aa216a79f14665af7de24c47eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.8 MB (77812722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbda4c98640add6594c969787d60f2ff0737148b1126e295c7550b48fd59887d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 09:05:17 GMT
ADD file:97ce5af9ff4fb4002733d5c402ddc01a13e765d31b85bb6525a7fa797b698e10 in / 
# Thu, 02 Dec 2021 09:05:17 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 17:16:05 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 17:21:51 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-7.0.1.tgz -o $tmpdir/orig.tgz;     echo "7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 17:21:52 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 17:21:53 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 02 Dec 2021 17:21:53 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 17:21:54 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 17:21:54 GMT
CMD []
```

-	Layers:
	-	`sha256:ba82a1312e1efdcd1cc6eb31cd40358dcec180da31779dac399cba31bf3dc206`  
		Last Modified: Thu, 02 Dec 2021 09:21:03 GMT  
		Size: 26.6 MB (26573192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a7af23f33d5037abbe717474bce6f137fdf6db1852beb948bcff91135ffabc`  
		Last Modified: Thu, 02 Dec 2021 17:36:44 GMT  
		Size: 51.2 MB (51239056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9fda28a9f74fe318d52ac4025f63aefdb4ff683eaed6debe26e8af22606f7d`  
		Last Modified: Thu, 02 Dec 2021 17:36:16 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0.1` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:61956ab15ae49e1d6900db09c616e4a5359341846205221fec7f6c0920cd3d74
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 MB (95289331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4b5de96371e693462f2885e1598467d53e46b15f8feb3d1e582f425e794d011`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Dec 2021 01:42:23 GMT
ADD file:986f91febed4aa8e2072081ff8419d52ba2060510822e717086d3b3d9469e4d7 in / 
# Tue, 21 Dec 2021 01:42:24 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:28:06 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Dec 2021 10:30:29 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-7.0.1.tgz -o $tmpdir/orig.tgz;     echo "7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 21 Dec 2021 10:30:29 GMT
WORKDIR /etc/varnish
# Tue, 21 Dec 2021 10:30:31 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 21 Dec 2021 10:30:31 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Dec 2021 10:30:32 GMT
EXPOSE 80 8443
# Tue, 21 Dec 2021 10:30:33 GMT
CMD []
```

-	Layers:
	-	`sha256:927a35006d93ea08499b57046904046d7926cd76fb17be193e3e74f56d634a08`  
		Last Modified: Tue, 21 Dec 2021 01:48:54 GMT  
		Size: 30.0 MB (30043793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7879c8db25efa15fd67c52352319b5decba8751ce82fc464e491208b56b6126c`  
		Last Modified: Tue, 21 Dec 2021 10:36:33 GMT  
		Size: 65.2 MB (65245064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3969df205cd59ced08fbbf1f1648394f1c621bfe1511d5ae8601239a07be49ed`  
		Last Modified: Tue, 21 Dec 2021 10:36:24 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0.1` - linux; 386

```console
$ docker pull varnish@sha256:b5711e2756437ce78ea84aa10ad810b1efc436055e26685ad1f8fd2d7b6917e2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.6 MB (102578231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c0cdb20dcbf11013ece2af89e3a9fa6a032513d1fbbc32e25388779c199b545`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 02:39:54 GMT
ADD file:0284c10b06ba22560408e1e14c1147887f4302c79dba143277ece2e333d6dcbc in / 
# Thu, 02 Dec 2021 02:39:55 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 14:41:26 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 14:45:23 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-7.0.1.tgz -o $tmpdir/orig.tgz;     echo "7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 14:45:24 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 14:45:25 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 02 Dec 2021 14:45:25 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 14:45:25 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 14:45:26 GMT
CMD []
```

-	Layers:
	-	`sha256:2df7932f17d752876c686aa22054692a38e88e182dd7b6a5cca7ffce4ffe6f84`  
		Last Modified: Thu, 02 Dec 2021 02:47:59 GMT  
		Size: 32.4 MB (32380814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4532a2822b9d5322c71f3791db81585df1f7fd7698d94c628b4a89789ab06d`  
		Last Modified: Thu, 02 Dec 2021 14:53:57 GMT  
		Size: 70.2 MB (70196944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43edf33f023e899d92eb9fb6d8b922f9e55ccaaf71daf98d429b3cd9a22610aa`  
		Last Modified: Thu, 02 Dec 2021 14:53:37 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0.1` - linux; ppc64le

```console
$ docker pull varnish@sha256:2c6433bcdfb8f6840987b269f0befb55f24b50e4d16512c54018fd26ef2c4117
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.4 MB (100360511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f76b57f61628753fe997c625800c5f45636b443a164d95dc38a46ac6b3730f1b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 07:21:21 GMT
ADD file:81a93de7f5dcdbb9397c05b9b6bb7dc5a4742119d46faf929b4c6277b02be7a5 in / 
# Thu, 02 Dec 2021 07:21:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 20:55:25 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 21:22:29 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-7.0.1.tgz -o $tmpdir/orig.tgz;     echo "7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 21:22:37 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 21:22:39 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 02 Dec 2021 21:22:41 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 21:22:43 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 21:22:45 GMT
CMD []
```

-	Layers:
	-	`sha256:8d46978b233ccedeaa1cbef7248b214991469fa922cc4fbf9916f9d0711d2d2e`  
		Last Modified: Thu, 02 Dec 2021 07:31:43 GMT  
		Size: 35.3 MB (35271379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a877f42cdd8c7663f7ff10b41702a657bf404827b4ecad08e33487a7b8879b`  
		Last Modified: Thu, 02 Dec 2021 21:59:36 GMT  
		Size: 65.1 MB (65088657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad6570cd65bc0a559262f22219716908f7b28ffd1cbd93d9bcdcde970371752`  
		Last Modified: Thu, 02 Dec 2021 21:59:22 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0.1` - linux; s390x

```console
$ docker pull varnish@sha256:de1bbc824a6aacfadb8414d3273e4a1ab2c2b49a7b4a880de6e64558266db2f7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.6 MB (81633677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9872cee508e48131bb3424959486542cd81d0eaec0d7c9747e58c90b16c4cb4f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 07:19:07 GMT
ADD file:9303def035f391c14bdca007751c5061f36fe929d5b3f4d725ce376e25f7dd36 in / 
# Thu, 02 Dec 2021 07:19:09 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 12:47:34 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 12:49:19 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-7.0.1.tgz -o $tmpdir/orig.tgz;     echo "7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 12:49:21 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 12:49:21 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 02 Dec 2021 12:49:21 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 12:49:21 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 12:49:21 GMT
CMD []
```

-	Layers:
	-	`sha256:bf2c280d82ca10801fb58bfc3f73029eef17592cbe00e94875cb189bdbac0c5f`  
		Last Modified: Thu, 02 Dec 2021 07:25:12 GMT  
		Size: 29.7 MB (29650954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea009950cddf65d0ad4b52a5ae1891b850f677718911376605822e794733ced`  
		Last Modified: Thu, 02 Dec 2021 12:53:09 GMT  
		Size: 52.0 MB (51982250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0bbe1910546c0494957b3da3bf63782f4d3786641b32c0c54d8ff8607ecfb5`  
		Last Modified: Thu, 02 Dec 2021 12:53:02 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.0.1-alpine`

```console
$ docker pull varnish@sha256:f87e507197e30345d94738e81eb3724707c42fc2629881019066d37028019f7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:7.0.1-alpine` - linux; amd64

```console
$ docker pull varnish@sha256:e6f6804aecc2fb6b091c54021c1773b77968d798293d41ab3ee46f5c00a58bb1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.4 MB (58362658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e7e9599575e47151d14b79975fd45baf80559233e36487f2ce8bbe0a941ce68`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 07:25:45 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 18:23:42 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 18:23:42 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 18:23:42 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Mon, 29 Nov 2021 18:23:42 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 18:23:43 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 18:23:43 GMT
CMD []
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf619492e89f6485a3ba5e7cb6807f6f35a59e5715d4bffcb692cfecddeefbd8`  
		Last Modified: Mon, 29 Nov 2021 18:30:34 GMT  
		Size: 55.5 MB (55539197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a667c3f673f5f288f2ff0a45cd4743280d929515d6979127e0cb9f843854d03`  
		Last Modified: Mon, 29 Nov 2021 18:30:26 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0.1-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:0a8a4359542a0d380e8caff6957abd147ba3e0d4d0f81291a2680f915fc4418e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44177096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efb40b53aee89e6abc8b6707b45a06124ad2bda4a6ce63c73b8c54ff9f4f310b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:41:33 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 21:25:11 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 21:25:12 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 21:25:13 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Mon, 29 Nov 2021 21:25:13 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 21:25:13 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 21:25:14 GMT
CMD []
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ba0a88317201e7b894f07e0179e31e58105e7f86b5716079c72f20d505e90d`  
		Last Modified: Mon, 29 Nov 2021 21:36:51 GMT  
		Size: 41.7 MB (41737996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d68e43dcc838fa62cef86b564038a9ebf4b4511e841577b9ad44a6a40e653e56`  
		Last Modified: Mon, 29 Nov 2021 21:36:29 GMT  
		Size: 482.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0.1-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:33a0b3a7ab60e096fee91372231b338f2256b92e1030b6e40c1cd0046b72841e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51095315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7cd53e93e2c30ec59c3d576f21316d000c835291752add2060586a1047d3f85`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:02:27 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 20:44:40 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 20:44:40 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 20:44:42 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Mon, 29 Nov 2021 20:44:42 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 20:44:43 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 20:44:44 GMT
CMD []
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed53609c137cea4c70e37bf852c4b51b6baa5e8d2a5d4f6dd5fff316ab310f78`  
		Last Modified: Mon, 29 Nov 2021 20:52:04 GMT  
		Size: 48.4 MB (48377136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99915de3f6477a815b3567ff58bc0b27f2c926cff1dbd04685aa00135003ea0`  
		Last Modified: Mon, 29 Nov 2021 20:51:57 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0.1-alpine` - linux; 386

```console
$ docker pull varnish@sha256:41415e58f6a0abfb75fc6d924cd4b8e695be23e29697990bd1b5652c50c38125
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.6 MB (58572214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a0be743f31821cf8c667a0bbda63169351f08c76d76f119573bdf4366721063`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:38:42 GMT
ADD file:403428c2903dd9dea10d069185873cb2c2c3149c553797807c69f22aa3d12fe3 in / 
# Fri, 12 Nov 2021 16:38:42 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 20:27:36 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 19:59:18 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 19:59:19 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 19:59:19 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Mon, 29 Nov 2021 19:59:19 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 19:59:20 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 19:59:20 GMT
CMD []
```

-	Layers:
	-	`sha256:5420e0d28c84ecb16748cb90cc6acf8e2a81dab10cb1f674f3eee8533e53c62a`  
		Last Modified: Fri, 12 Nov 2021 16:39:36 GMT  
		Size: 2.8 MB (2830948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a847bbc8f41c777fb2d9bb80d681e74aff97c1d7b641dc784f50d2f15e65878`  
		Last Modified: Mon, 29 Nov 2021 20:02:17 GMT  
		Size: 55.7 MB (55740787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de19c3037a0843a385ef2b761144a16e7b2928588ad15b9d3c8a55e4271c7d49`  
		Last Modified: Mon, 29 Nov 2021 20:02:07 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0.1-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:3dbc09408d5de96ed2e1da8ee6839b6d2d27d2a6b61461af2dfd979800c96ae4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48217424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf9c543a6c0fc8cebf02f61bc86908cdfd0336e14d49f4585f0b66516aeb8824`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 21:18:00 GMT
ADD file:4d45063079cb28a34f1e382fddb22f156ac99d5449aa05ed37cb653c1f7b80f2 in / 
# Fri, 12 Nov 2021 21:18:01 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:52:07 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 19:33:01 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 19:33:14 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 19:33:16 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Mon, 29 Nov 2021 19:33:20 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 19:33:24 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 19:33:26 GMT
CMD []
```

-	Layers:
	-	`sha256:72940440c1ab65eca4d38846164719ffde4b147543cc658d041407a925b13368`  
		Last Modified: Fri, 12 Nov 2021 21:19:32 GMT  
		Size: 2.8 MB (2817467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fee0663614f072189bcfe90801176e82e4b095b43d6669338848e513113a6b`  
		Last Modified: Mon, 29 Nov 2021 20:14:35 GMT  
		Size: 45.4 MB (45399475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415be876b654e4417228f66afdf87a6f7fb9eb42f7b4c56e20a48c5cf82e155b`  
		Last Modified: Mon, 29 Nov 2021 20:14:24 GMT  
		Size: 482.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0.1-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:fc3bcee94e4ebed0aeb20e8452bf251168c054aba104ec73cfe2eef09f4e8493
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46683739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94b29bebe019d754443456933a8ab78ec41609ba82475054712204df54da7729`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:41:35 GMT
ADD file:7e0cf02b3f015b1a0f867c03b2902b85f2140be1cee7af63c23f367a487e4577 in / 
# Fri, 12 Nov 2021 16:41:36 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 22:10:22 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 20:07:02 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 20:07:03 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 20:07:03 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Mon, 29 Nov 2021 20:07:03 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 20:07:03 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 20:07:04 GMT
CMD []
```

-	Layers:
	-	`sha256:817a13b0e05928f7491adbf1d2cf261ec35079112247bd03469bbe31156aca7c`  
		Last Modified: Fri, 12 Nov 2021 16:42:44 GMT  
		Size: 2.6 MB (2609278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd4ecc3a23e099fd1b2190632241b2eb90449a80f21c20aea2dc403e49b660e`  
		Last Modified: Mon, 29 Nov 2021 20:11:28 GMT  
		Size: 44.1 MB (44073983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5949a7063bbe02e339a90c74121063f6f7d783927a93059408bbb4112f6d86de`  
		Last Modified: Mon, 29 Nov 2021 20:11:23 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:alpine`

```console
$ docker pull varnish@sha256:f87e507197e30345d94738e81eb3724707c42fc2629881019066d37028019f7b
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
$ docker pull varnish@sha256:e6f6804aecc2fb6b091c54021c1773b77968d798293d41ab3ee46f5c00a58bb1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.4 MB (58362658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e7e9599575e47151d14b79975fd45baf80559233e36487f2ce8bbe0a941ce68`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 07:25:45 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 18:23:42 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 18:23:42 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 18:23:42 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Mon, 29 Nov 2021 18:23:42 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 18:23:43 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 18:23:43 GMT
CMD []
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf619492e89f6485a3ba5e7cb6807f6f35a59e5715d4bffcb692cfecddeefbd8`  
		Last Modified: Mon, 29 Nov 2021 18:30:34 GMT  
		Size: 55.5 MB (55539197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a667c3f673f5f288f2ff0a45cd4743280d929515d6979127e0cb9f843854d03`  
		Last Modified: Mon, 29 Nov 2021 18:30:26 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:0a8a4359542a0d380e8caff6957abd147ba3e0d4d0f81291a2680f915fc4418e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44177096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efb40b53aee89e6abc8b6707b45a06124ad2bda4a6ce63c73b8c54ff9f4f310b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:41:33 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 21:25:11 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 21:25:12 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 21:25:13 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Mon, 29 Nov 2021 21:25:13 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 21:25:13 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 21:25:14 GMT
CMD []
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ba0a88317201e7b894f07e0179e31e58105e7f86b5716079c72f20d505e90d`  
		Last Modified: Mon, 29 Nov 2021 21:36:51 GMT  
		Size: 41.7 MB (41737996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d68e43dcc838fa62cef86b564038a9ebf4b4511e841577b9ad44a6a40e653e56`  
		Last Modified: Mon, 29 Nov 2021 21:36:29 GMT  
		Size: 482.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:33a0b3a7ab60e096fee91372231b338f2256b92e1030b6e40c1cd0046b72841e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51095315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7cd53e93e2c30ec59c3d576f21316d000c835291752add2060586a1047d3f85`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:02:27 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 20:44:40 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 20:44:40 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 20:44:42 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Mon, 29 Nov 2021 20:44:42 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 20:44:43 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 20:44:44 GMT
CMD []
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed53609c137cea4c70e37bf852c4b51b6baa5e8d2a5d4f6dd5fff316ab310f78`  
		Last Modified: Mon, 29 Nov 2021 20:52:04 GMT  
		Size: 48.4 MB (48377136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99915de3f6477a815b3567ff58bc0b27f2c926cff1dbd04685aa00135003ea0`  
		Last Modified: Mon, 29 Nov 2021 20:51:57 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; 386

```console
$ docker pull varnish@sha256:41415e58f6a0abfb75fc6d924cd4b8e695be23e29697990bd1b5652c50c38125
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.6 MB (58572214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a0be743f31821cf8c667a0bbda63169351f08c76d76f119573bdf4366721063`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:38:42 GMT
ADD file:403428c2903dd9dea10d069185873cb2c2c3149c553797807c69f22aa3d12fe3 in / 
# Fri, 12 Nov 2021 16:38:42 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 20:27:36 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 19:59:18 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 19:59:19 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 19:59:19 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Mon, 29 Nov 2021 19:59:19 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 19:59:20 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 19:59:20 GMT
CMD []
```

-	Layers:
	-	`sha256:5420e0d28c84ecb16748cb90cc6acf8e2a81dab10cb1f674f3eee8533e53c62a`  
		Last Modified: Fri, 12 Nov 2021 16:39:36 GMT  
		Size: 2.8 MB (2830948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a847bbc8f41c777fb2d9bb80d681e74aff97c1d7b641dc784f50d2f15e65878`  
		Last Modified: Mon, 29 Nov 2021 20:02:17 GMT  
		Size: 55.7 MB (55740787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de19c3037a0843a385ef2b761144a16e7b2928588ad15b9d3c8a55e4271c7d49`  
		Last Modified: Mon, 29 Nov 2021 20:02:07 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:3dbc09408d5de96ed2e1da8ee6839b6d2d27d2a6b61461af2dfd979800c96ae4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48217424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf9c543a6c0fc8cebf02f61bc86908cdfd0336e14d49f4585f0b66516aeb8824`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 21:18:00 GMT
ADD file:4d45063079cb28a34f1e382fddb22f156ac99d5449aa05ed37cb653c1f7b80f2 in / 
# Fri, 12 Nov 2021 21:18:01 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:52:07 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 19:33:01 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 19:33:14 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 19:33:16 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Mon, 29 Nov 2021 19:33:20 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 19:33:24 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 19:33:26 GMT
CMD []
```

-	Layers:
	-	`sha256:72940440c1ab65eca4d38846164719ffde4b147543cc658d041407a925b13368`  
		Last Modified: Fri, 12 Nov 2021 21:19:32 GMT  
		Size: 2.8 MB (2817467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fee0663614f072189bcfe90801176e82e4b095b43d6669338848e513113a6b`  
		Last Modified: Mon, 29 Nov 2021 20:14:35 GMT  
		Size: 45.4 MB (45399475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415be876b654e4417228f66afdf87a6f7fb9eb42f7b4c56e20a48c5cf82e155b`  
		Last Modified: Mon, 29 Nov 2021 20:14:24 GMT  
		Size: 482.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; s390x

```console
$ docker pull varnish@sha256:fc3bcee94e4ebed0aeb20e8452bf251168c054aba104ec73cfe2eef09f4e8493
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46683739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94b29bebe019d754443456933a8ab78ec41609ba82475054712204df54da7729`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:41:35 GMT
ADD file:7e0cf02b3f015b1a0f867c03b2902b85f2140be1cee7af63c23f367a487e4577 in / 
# Fri, 12 Nov 2021 16:41:36 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 22:10:22 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 20:07:02 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 20:07:03 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 20:07:03 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Mon, 29 Nov 2021 20:07:03 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 20:07:03 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 20:07:04 GMT
CMD []
```

-	Layers:
	-	`sha256:817a13b0e05928f7491adbf1d2cf261ec35079112247bd03469bbe31156aca7c`  
		Last Modified: Fri, 12 Nov 2021 16:42:44 GMT  
		Size: 2.6 MB (2609278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd4ecc3a23e099fd1b2190632241b2eb90449a80f21c20aea2dc403e49b660e`  
		Last Modified: Mon, 29 Nov 2021 20:11:28 GMT  
		Size: 44.1 MB (44073983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5949a7063bbe02e339a90c74121063f6f7d783927a93059408bbb4112f6d86de`  
		Last Modified: Mon, 29 Nov 2021 20:11:23 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:fresh`

```console
$ docker pull varnish@sha256:d81f3e0cb09821ee06c6e1c3dde09adda1db842bb97548c6431e98f3f770d927
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
$ docker pull varnish@sha256:ae959bdd6bb300bdf4ab4667d40b0a3bd7805cb398668446c619b484d0538c69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101191056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a30574a32f9387bfb3e1de6a5a9bf2f8c747befabc15268836a09bba431edc30`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 02:48:20 GMT
ADD file:ece5ff85ca549f0b1e9139d29dcb43a52af672d0591c423e28180f6d8d700ad7 in / 
# Thu, 02 Dec 2021 02:48:21 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 17:48:20 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 17:51:31 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-7.0.1.tgz -o $tmpdir/orig.tgz;     echo "7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 17:51:32 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 17:51:32 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 02 Dec 2021 17:51:33 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 17:51:33 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 17:51:33 GMT
CMD []
```

-	Layers:
	-	`sha256:e5ae68f740265288a4888db98d2999a638fdcb6d725f427678814538d253aa4d`  
		Last Modified: Thu, 02 Dec 2021 02:53:46 GMT  
		Size: 31.4 MB (31370221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12826beb2fa2a9fd22ca8cf0048dc3d9e93dda923855bbf2f9edc2eac7d2db7`  
		Last Modified: Thu, 02 Dec 2021 17:58:48 GMT  
		Size: 69.8 MB (69820363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25909d0f31444a52569da07a6ce274b76d41f6bf139bb4a55291c544ad04705a`  
		Last Modified: Thu, 02 Dec 2021 17:58:37 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; arm variant v7

```console
$ docker pull varnish@sha256:ed282cf2f85b7f88b869454bd6ce98f50ea8c4aa216a79f14665af7de24c47eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.8 MB (77812722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbda4c98640add6594c969787d60f2ff0737148b1126e295c7550b48fd59887d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 09:05:17 GMT
ADD file:97ce5af9ff4fb4002733d5c402ddc01a13e765d31b85bb6525a7fa797b698e10 in / 
# Thu, 02 Dec 2021 09:05:17 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 17:16:05 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 17:21:51 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-7.0.1.tgz -o $tmpdir/orig.tgz;     echo "7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 17:21:52 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 17:21:53 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 02 Dec 2021 17:21:53 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 17:21:54 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 17:21:54 GMT
CMD []
```

-	Layers:
	-	`sha256:ba82a1312e1efdcd1cc6eb31cd40358dcec180da31779dac399cba31bf3dc206`  
		Last Modified: Thu, 02 Dec 2021 09:21:03 GMT  
		Size: 26.6 MB (26573192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a7af23f33d5037abbe717474bce6f137fdf6db1852beb948bcff91135ffabc`  
		Last Modified: Thu, 02 Dec 2021 17:36:44 GMT  
		Size: 51.2 MB (51239056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9fda28a9f74fe318d52ac4025f63aefdb4ff683eaed6debe26e8af22606f7d`  
		Last Modified: Thu, 02 Dec 2021 17:36:16 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:61956ab15ae49e1d6900db09c616e4a5359341846205221fec7f6c0920cd3d74
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 MB (95289331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4b5de96371e693462f2885e1598467d53e46b15f8feb3d1e582f425e794d011`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Dec 2021 01:42:23 GMT
ADD file:986f91febed4aa8e2072081ff8419d52ba2060510822e717086d3b3d9469e4d7 in / 
# Tue, 21 Dec 2021 01:42:24 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:28:06 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Dec 2021 10:30:29 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-7.0.1.tgz -o $tmpdir/orig.tgz;     echo "7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 21 Dec 2021 10:30:29 GMT
WORKDIR /etc/varnish
# Tue, 21 Dec 2021 10:30:31 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 21 Dec 2021 10:30:31 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Dec 2021 10:30:32 GMT
EXPOSE 80 8443
# Tue, 21 Dec 2021 10:30:33 GMT
CMD []
```

-	Layers:
	-	`sha256:927a35006d93ea08499b57046904046d7926cd76fb17be193e3e74f56d634a08`  
		Last Modified: Tue, 21 Dec 2021 01:48:54 GMT  
		Size: 30.0 MB (30043793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7879c8db25efa15fd67c52352319b5decba8751ce82fc464e491208b56b6126c`  
		Last Modified: Tue, 21 Dec 2021 10:36:33 GMT  
		Size: 65.2 MB (65245064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3969df205cd59ced08fbbf1f1648394f1c621bfe1511d5ae8601239a07be49ed`  
		Last Modified: Tue, 21 Dec 2021 10:36:24 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; 386

```console
$ docker pull varnish@sha256:b5711e2756437ce78ea84aa10ad810b1efc436055e26685ad1f8fd2d7b6917e2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.6 MB (102578231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c0cdb20dcbf11013ece2af89e3a9fa6a032513d1fbbc32e25388779c199b545`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 02:39:54 GMT
ADD file:0284c10b06ba22560408e1e14c1147887f4302c79dba143277ece2e333d6dcbc in / 
# Thu, 02 Dec 2021 02:39:55 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 14:41:26 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 14:45:23 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-7.0.1.tgz -o $tmpdir/orig.tgz;     echo "7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 14:45:24 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 14:45:25 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 02 Dec 2021 14:45:25 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 14:45:25 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 14:45:26 GMT
CMD []
```

-	Layers:
	-	`sha256:2df7932f17d752876c686aa22054692a38e88e182dd7b6a5cca7ffce4ffe6f84`  
		Last Modified: Thu, 02 Dec 2021 02:47:59 GMT  
		Size: 32.4 MB (32380814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4532a2822b9d5322c71f3791db81585df1f7fd7698d94c628b4a89789ab06d`  
		Last Modified: Thu, 02 Dec 2021 14:53:57 GMT  
		Size: 70.2 MB (70196944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43edf33f023e899d92eb9fb6d8b922f9e55ccaaf71daf98d429b3cd9a22610aa`  
		Last Modified: Thu, 02 Dec 2021 14:53:37 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; ppc64le

```console
$ docker pull varnish@sha256:2c6433bcdfb8f6840987b269f0befb55f24b50e4d16512c54018fd26ef2c4117
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.4 MB (100360511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f76b57f61628753fe997c625800c5f45636b443a164d95dc38a46ac6b3730f1b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 07:21:21 GMT
ADD file:81a93de7f5dcdbb9397c05b9b6bb7dc5a4742119d46faf929b4c6277b02be7a5 in / 
# Thu, 02 Dec 2021 07:21:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 20:55:25 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 21:22:29 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-7.0.1.tgz -o $tmpdir/orig.tgz;     echo "7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 21:22:37 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 21:22:39 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 02 Dec 2021 21:22:41 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 21:22:43 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 21:22:45 GMT
CMD []
```

-	Layers:
	-	`sha256:8d46978b233ccedeaa1cbef7248b214991469fa922cc4fbf9916f9d0711d2d2e`  
		Last Modified: Thu, 02 Dec 2021 07:31:43 GMT  
		Size: 35.3 MB (35271379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a877f42cdd8c7663f7ff10b41702a657bf404827b4ecad08e33487a7b8879b`  
		Last Modified: Thu, 02 Dec 2021 21:59:36 GMT  
		Size: 65.1 MB (65088657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad6570cd65bc0a559262f22219716908f7b28ffd1cbd93d9bcdcde970371752`  
		Last Modified: Thu, 02 Dec 2021 21:59:22 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; s390x

```console
$ docker pull varnish@sha256:de1bbc824a6aacfadb8414d3273e4a1ab2c2b49a7b4a880de6e64558266db2f7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.6 MB (81633677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9872cee508e48131bb3424959486542cd81d0eaec0d7c9747e58c90b16c4cb4f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 07:19:07 GMT
ADD file:9303def035f391c14bdca007751c5061f36fe929d5b3f4d725ce376e25f7dd36 in / 
# Thu, 02 Dec 2021 07:19:09 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 12:47:34 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 12:49:19 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-7.0.1.tgz -o $tmpdir/orig.tgz;     echo "7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 12:49:21 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 12:49:21 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 02 Dec 2021 12:49:21 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 12:49:21 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 12:49:21 GMT
CMD []
```

-	Layers:
	-	`sha256:bf2c280d82ca10801fb58bfc3f73029eef17592cbe00e94875cb189bdbac0c5f`  
		Last Modified: Thu, 02 Dec 2021 07:25:12 GMT  
		Size: 29.7 MB (29650954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea009950cddf65d0ad4b52a5ae1891b850f677718911376605822e794733ced`  
		Last Modified: Thu, 02 Dec 2021 12:53:09 GMT  
		Size: 52.0 MB (51982250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0bbe1910546c0494957b3da3bf63782f4d3786641b32c0c54d8ff8607ecfb5`  
		Last Modified: Thu, 02 Dec 2021 12:53:02 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:fresh-alpine`

```console
$ docker pull varnish@sha256:f87e507197e30345d94738e81eb3724707c42fc2629881019066d37028019f7b
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
$ docker pull varnish@sha256:e6f6804aecc2fb6b091c54021c1773b77968d798293d41ab3ee46f5c00a58bb1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.4 MB (58362658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e7e9599575e47151d14b79975fd45baf80559233e36487f2ce8bbe0a941ce68`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 07:25:45 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 18:23:42 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 18:23:42 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 18:23:42 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Mon, 29 Nov 2021 18:23:42 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 18:23:43 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 18:23:43 GMT
CMD []
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf619492e89f6485a3ba5e7cb6807f6f35a59e5715d4bffcb692cfecddeefbd8`  
		Last Modified: Mon, 29 Nov 2021 18:30:34 GMT  
		Size: 55.5 MB (55539197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a667c3f673f5f288f2ff0a45cd4743280d929515d6979127e0cb9f843854d03`  
		Last Modified: Mon, 29 Nov 2021 18:30:26 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:0a8a4359542a0d380e8caff6957abd147ba3e0d4d0f81291a2680f915fc4418e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44177096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efb40b53aee89e6abc8b6707b45a06124ad2bda4a6ce63c73b8c54ff9f4f310b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:41:33 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 21:25:11 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 21:25:12 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 21:25:13 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Mon, 29 Nov 2021 21:25:13 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 21:25:13 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 21:25:14 GMT
CMD []
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ba0a88317201e7b894f07e0179e31e58105e7f86b5716079c72f20d505e90d`  
		Last Modified: Mon, 29 Nov 2021 21:36:51 GMT  
		Size: 41.7 MB (41737996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d68e43dcc838fa62cef86b564038a9ebf4b4511e841577b9ad44a6a40e653e56`  
		Last Modified: Mon, 29 Nov 2021 21:36:29 GMT  
		Size: 482.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:33a0b3a7ab60e096fee91372231b338f2256b92e1030b6e40c1cd0046b72841e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51095315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7cd53e93e2c30ec59c3d576f21316d000c835291752add2060586a1047d3f85`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:02:27 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 20:44:40 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 20:44:40 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 20:44:42 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Mon, 29 Nov 2021 20:44:42 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 20:44:43 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 20:44:44 GMT
CMD []
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed53609c137cea4c70e37bf852c4b51b6baa5e8d2a5d4f6dd5fff316ab310f78`  
		Last Modified: Mon, 29 Nov 2021 20:52:04 GMT  
		Size: 48.4 MB (48377136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99915de3f6477a815b3567ff58bc0b27f2c926cff1dbd04685aa00135003ea0`  
		Last Modified: Mon, 29 Nov 2021 20:51:57 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; 386

```console
$ docker pull varnish@sha256:41415e58f6a0abfb75fc6d924cd4b8e695be23e29697990bd1b5652c50c38125
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.6 MB (58572214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a0be743f31821cf8c667a0bbda63169351f08c76d76f119573bdf4366721063`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:38:42 GMT
ADD file:403428c2903dd9dea10d069185873cb2c2c3149c553797807c69f22aa3d12fe3 in / 
# Fri, 12 Nov 2021 16:38:42 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 20:27:36 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 19:59:18 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 19:59:19 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 19:59:19 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Mon, 29 Nov 2021 19:59:19 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 19:59:20 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 19:59:20 GMT
CMD []
```

-	Layers:
	-	`sha256:5420e0d28c84ecb16748cb90cc6acf8e2a81dab10cb1f674f3eee8533e53c62a`  
		Last Modified: Fri, 12 Nov 2021 16:39:36 GMT  
		Size: 2.8 MB (2830948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a847bbc8f41c777fb2d9bb80d681e74aff97c1d7b641dc784f50d2f15e65878`  
		Last Modified: Mon, 29 Nov 2021 20:02:17 GMT  
		Size: 55.7 MB (55740787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de19c3037a0843a385ef2b761144a16e7b2928588ad15b9d3c8a55e4271c7d49`  
		Last Modified: Mon, 29 Nov 2021 20:02:07 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:3dbc09408d5de96ed2e1da8ee6839b6d2d27d2a6b61461af2dfd979800c96ae4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48217424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf9c543a6c0fc8cebf02f61bc86908cdfd0336e14d49f4585f0b66516aeb8824`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 21:18:00 GMT
ADD file:4d45063079cb28a34f1e382fddb22f156ac99d5449aa05ed37cb653c1f7b80f2 in / 
# Fri, 12 Nov 2021 21:18:01 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:52:07 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 19:33:01 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 19:33:14 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 19:33:16 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Mon, 29 Nov 2021 19:33:20 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 19:33:24 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 19:33:26 GMT
CMD []
```

-	Layers:
	-	`sha256:72940440c1ab65eca4d38846164719ffde4b147543cc658d041407a925b13368`  
		Last Modified: Fri, 12 Nov 2021 21:19:32 GMT  
		Size: 2.8 MB (2817467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fee0663614f072189bcfe90801176e82e4b095b43d6669338848e513113a6b`  
		Last Modified: Mon, 29 Nov 2021 20:14:35 GMT  
		Size: 45.4 MB (45399475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415be876b654e4417228f66afdf87a6f7fb9eb42f7b4c56e20a48c5cf82e155b`  
		Last Modified: Mon, 29 Nov 2021 20:14:24 GMT  
		Size: 482.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:fc3bcee94e4ebed0aeb20e8452bf251168c054aba104ec73cfe2eef09f4e8493
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46683739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94b29bebe019d754443456933a8ab78ec41609ba82475054712204df54da7729`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:41:35 GMT
ADD file:7e0cf02b3f015b1a0f867c03b2902b85f2140be1cee7af63c23f367a487e4577 in / 
# Fri, 12 Nov 2021 16:41:36 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 22:10:22 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 20:07:02 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 20:07:03 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 20:07:03 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Mon, 29 Nov 2021 20:07:03 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 20:07:03 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 20:07:04 GMT
CMD []
```

-	Layers:
	-	`sha256:817a13b0e05928f7491adbf1d2cf261ec35079112247bd03469bbe31156aca7c`  
		Last Modified: Fri, 12 Nov 2021 16:42:44 GMT  
		Size: 2.6 MB (2609278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd4ecc3a23e099fd1b2190632241b2eb90449a80f21c20aea2dc403e49b660e`  
		Last Modified: Mon, 29 Nov 2021 20:11:28 GMT  
		Size: 44.1 MB (44073983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5949a7063bbe02e339a90c74121063f6f7d783927a93059408bbb4112f6d86de`  
		Last Modified: Mon, 29 Nov 2021 20:11:23 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:latest`

```console
$ docker pull varnish@sha256:d81f3e0cb09821ee06c6e1c3dde09adda1db842bb97548c6431e98f3f770d927
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
$ docker pull varnish@sha256:ae959bdd6bb300bdf4ab4667d40b0a3bd7805cb398668446c619b484d0538c69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101191056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a30574a32f9387bfb3e1de6a5a9bf2f8c747befabc15268836a09bba431edc30`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 02:48:20 GMT
ADD file:ece5ff85ca549f0b1e9139d29dcb43a52af672d0591c423e28180f6d8d700ad7 in / 
# Thu, 02 Dec 2021 02:48:21 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 17:48:20 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 17:51:31 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-7.0.1.tgz -o $tmpdir/orig.tgz;     echo "7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 17:51:32 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 17:51:32 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 02 Dec 2021 17:51:33 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 17:51:33 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 17:51:33 GMT
CMD []
```

-	Layers:
	-	`sha256:e5ae68f740265288a4888db98d2999a638fdcb6d725f427678814538d253aa4d`  
		Last Modified: Thu, 02 Dec 2021 02:53:46 GMT  
		Size: 31.4 MB (31370221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12826beb2fa2a9fd22ca8cf0048dc3d9e93dda923855bbf2f9edc2eac7d2db7`  
		Last Modified: Thu, 02 Dec 2021 17:58:48 GMT  
		Size: 69.8 MB (69820363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25909d0f31444a52569da07a6ce274b76d41f6bf139bb4a55291c544ad04705a`  
		Last Modified: Thu, 02 Dec 2021 17:58:37 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; arm variant v7

```console
$ docker pull varnish@sha256:ed282cf2f85b7f88b869454bd6ce98f50ea8c4aa216a79f14665af7de24c47eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.8 MB (77812722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbda4c98640add6594c969787d60f2ff0737148b1126e295c7550b48fd59887d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 09:05:17 GMT
ADD file:97ce5af9ff4fb4002733d5c402ddc01a13e765d31b85bb6525a7fa797b698e10 in / 
# Thu, 02 Dec 2021 09:05:17 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 17:16:05 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 17:21:51 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-7.0.1.tgz -o $tmpdir/orig.tgz;     echo "7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 17:21:52 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 17:21:53 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 02 Dec 2021 17:21:53 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 17:21:54 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 17:21:54 GMT
CMD []
```

-	Layers:
	-	`sha256:ba82a1312e1efdcd1cc6eb31cd40358dcec180da31779dac399cba31bf3dc206`  
		Last Modified: Thu, 02 Dec 2021 09:21:03 GMT  
		Size: 26.6 MB (26573192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a7af23f33d5037abbe717474bce6f137fdf6db1852beb948bcff91135ffabc`  
		Last Modified: Thu, 02 Dec 2021 17:36:44 GMT  
		Size: 51.2 MB (51239056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9fda28a9f74fe318d52ac4025f63aefdb4ff683eaed6debe26e8af22606f7d`  
		Last Modified: Thu, 02 Dec 2021 17:36:16 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:61956ab15ae49e1d6900db09c616e4a5359341846205221fec7f6c0920cd3d74
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 MB (95289331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4b5de96371e693462f2885e1598467d53e46b15f8feb3d1e582f425e794d011`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Dec 2021 01:42:23 GMT
ADD file:986f91febed4aa8e2072081ff8419d52ba2060510822e717086d3b3d9469e4d7 in / 
# Tue, 21 Dec 2021 01:42:24 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:28:06 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Dec 2021 10:30:29 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-7.0.1.tgz -o $tmpdir/orig.tgz;     echo "7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 21 Dec 2021 10:30:29 GMT
WORKDIR /etc/varnish
# Tue, 21 Dec 2021 10:30:31 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 21 Dec 2021 10:30:31 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Dec 2021 10:30:32 GMT
EXPOSE 80 8443
# Tue, 21 Dec 2021 10:30:33 GMT
CMD []
```

-	Layers:
	-	`sha256:927a35006d93ea08499b57046904046d7926cd76fb17be193e3e74f56d634a08`  
		Last Modified: Tue, 21 Dec 2021 01:48:54 GMT  
		Size: 30.0 MB (30043793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7879c8db25efa15fd67c52352319b5decba8751ce82fc464e491208b56b6126c`  
		Last Modified: Tue, 21 Dec 2021 10:36:33 GMT  
		Size: 65.2 MB (65245064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3969df205cd59ced08fbbf1f1648394f1c621bfe1511d5ae8601239a07be49ed`  
		Last Modified: Tue, 21 Dec 2021 10:36:24 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; 386

```console
$ docker pull varnish@sha256:b5711e2756437ce78ea84aa10ad810b1efc436055e26685ad1f8fd2d7b6917e2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.6 MB (102578231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c0cdb20dcbf11013ece2af89e3a9fa6a032513d1fbbc32e25388779c199b545`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 02:39:54 GMT
ADD file:0284c10b06ba22560408e1e14c1147887f4302c79dba143277ece2e333d6dcbc in / 
# Thu, 02 Dec 2021 02:39:55 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 14:41:26 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 14:45:23 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-7.0.1.tgz -o $tmpdir/orig.tgz;     echo "7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 14:45:24 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 14:45:25 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 02 Dec 2021 14:45:25 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 14:45:25 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 14:45:26 GMT
CMD []
```

-	Layers:
	-	`sha256:2df7932f17d752876c686aa22054692a38e88e182dd7b6a5cca7ffce4ffe6f84`  
		Last Modified: Thu, 02 Dec 2021 02:47:59 GMT  
		Size: 32.4 MB (32380814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4532a2822b9d5322c71f3791db81585df1f7fd7698d94c628b4a89789ab06d`  
		Last Modified: Thu, 02 Dec 2021 14:53:57 GMT  
		Size: 70.2 MB (70196944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43edf33f023e899d92eb9fb6d8b922f9e55ccaaf71daf98d429b3cd9a22610aa`  
		Last Modified: Thu, 02 Dec 2021 14:53:37 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; ppc64le

```console
$ docker pull varnish@sha256:2c6433bcdfb8f6840987b269f0befb55f24b50e4d16512c54018fd26ef2c4117
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.4 MB (100360511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f76b57f61628753fe997c625800c5f45636b443a164d95dc38a46ac6b3730f1b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 07:21:21 GMT
ADD file:81a93de7f5dcdbb9397c05b9b6bb7dc5a4742119d46faf929b4c6277b02be7a5 in / 
# Thu, 02 Dec 2021 07:21:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 20:55:25 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 21:22:29 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-7.0.1.tgz -o $tmpdir/orig.tgz;     echo "7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 21:22:37 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 21:22:39 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 02 Dec 2021 21:22:41 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 21:22:43 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 21:22:45 GMT
CMD []
```

-	Layers:
	-	`sha256:8d46978b233ccedeaa1cbef7248b214991469fa922cc4fbf9916f9d0711d2d2e`  
		Last Modified: Thu, 02 Dec 2021 07:31:43 GMT  
		Size: 35.3 MB (35271379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a877f42cdd8c7663f7ff10b41702a657bf404827b4ecad08e33487a7b8879b`  
		Last Modified: Thu, 02 Dec 2021 21:59:36 GMT  
		Size: 65.1 MB (65088657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad6570cd65bc0a559262f22219716908f7b28ffd1cbd93d9bcdcde970371752`  
		Last Modified: Thu, 02 Dec 2021 21:59:22 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; s390x

```console
$ docker pull varnish@sha256:de1bbc824a6aacfadb8414d3273e4a1ab2c2b49a7b4a880de6e64558266db2f7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.6 MB (81633677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9872cee508e48131bb3424959486542cd81d0eaec0d7c9747e58c90b16c4cb4f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 07:19:07 GMT
ADD file:9303def035f391c14bdca007751c5061f36fe929d5b3f4d725ce376e25f7dd36 in / 
# Thu, 02 Dec 2021 07:19:09 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 12:47:34 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 12:49:19 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-7.0.1.tgz -o $tmpdir/orig.tgz;     echo "7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 12:49:21 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 12:49:21 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 02 Dec 2021 12:49:21 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 12:49:21 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 12:49:21 GMT
CMD []
```

-	Layers:
	-	`sha256:bf2c280d82ca10801fb58bfc3f73029eef17592cbe00e94875cb189bdbac0c5f`  
		Last Modified: Thu, 02 Dec 2021 07:25:12 GMT  
		Size: 29.7 MB (29650954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea009950cddf65d0ad4b52a5ae1891b850f677718911376605822e794733ced`  
		Last Modified: Thu, 02 Dec 2021 12:53:09 GMT  
		Size: 52.0 MB (51982250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0bbe1910546c0494957b3da3bf63782f4d3786641b32c0c54d8ff8607ecfb5`  
		Last Modified: Thu, 02 Dec 2021 12:53:02 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:old`

```console
$ docker pull varnish@sha256:0e299ff5c2b04a608dd4333c430a8f4e6c78104248bbc413606c45b1e7f804c8
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
$ docker pull varnish@sha256:4e9a31f9cd3768e94409465bc6a147521426447a500d4cc02b085771f94ceab1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.1 MB (101111892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73d4575ed5fdcfe4eae8cdad180dcc1b6ff651a9fbe51f640ae291cb22eb75c4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 02:48:20 GMT
ADD file:ece5ff85ca549f0b1e9139d29dcb43a52af672d0591c423e28180f6d8d700ad7 in / 
# Thu, 02 Dec 2021 02:48:21 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 17:48:20 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 17:54:45 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.6.1.tgz -o $tmpdir/orig.tgz;     echo "af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.6.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 17:54:46 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 17:54:46 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 02 Dec 2021 17:54:46 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 17:54:47 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 17:54:47 GMT
CMD []
```

-	Layers:
	-	`sha256:e5ae68f740265288a4888db98d2999a638fdcb6d725f427678814538d253aa4d`  
		Last Modified: Thu, 02 Dec 2021 02:53:46 GMT  
		Size: 31.4 MB (31370221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54aafcbd42918f75407dff1904fed8191a04453c65ebc1bb390a504f95dd9b48`  
		Last Modified: Thu, 02 Dec 2021 17:59:15 GMT  
		Size: 69.7 MB (69740968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef06e7e4e4e50154e65169fb5a1998f8896a9269d468dc69292eec6b4d54227`  
		Last Modified: Thu, 02 Dec 2021 17:59:04 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; arm variant v7

```console
$ docker pull varnish@sha256:f05c268f8e8bb687fe1f4f8e8acdb51a3227ed4be5bf83fc697910f0fa90dfb0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.7 MB (77727488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01fcc14c5839bed7878b09ad08adf90226d16a47e2096669fb230457233dd4a2`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 09:05:17 GMT
ADD file:97ce5af9ff4fb4002733d5c402ddc01a13e765d31b85bb6525a7fa797b698e10 in / 
# Thu, 02 Dec 2021 09:05:17 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 17:16:05 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 17:27:59 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.6.1.tgz -o $tmpdir/orig.tgz;     echo "af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.6.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 17:28:00 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 17:28:00 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 02 Dec 2021 17:28:01 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 17:28:01 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 17:28:01 GMT
CMD []
```

-	Layers:
	-	`sha256:ba82a1312e1efdcd1cc6eb31cd40358dcec180da31779dac399cba31bf3dc206`  
		Last Modified: Thu, 02 Dec 2021 09:21:03 GMT  
		Size: 26.6 MB (26573192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85dad9248f0b6f379b3fc0581d83af70ba00e2ad83b7b9fea210fe9e71180748`  
		Last Modified: Thu, 02 Dec 2021 17:37:34 GMT  
		Size: 51.2 MB (51153596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e1f08afc9c3f5a7595f71bd9cddb3790098261476e2001bfa8f056a25fdf73`  
		Last Modified: Thu, 02 Dec 2021 17:37:10 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:3f5c0ade9623076b6f70af0f9c2e8ed1c5e05e8a26132cbcb69ab332c79d8874
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.2 MB (95201957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c878a4677639eae79f1dc7bdc929e5a01023d410f3a82d7af12be91839296a9`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Dec 2021 01:42:23 GMT
ADD file:986f91febed4aa8e2072081ff8419d52ba2060510822e717086d3b3d9469e4d7 in / 
# Tue, 21 Dec 2021 01:42:24 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:28:06 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Dec 2021 10:33:04 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.6.1.tgz -o $tmpdir/orig.tgz;     echo "af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.6.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 21 Dec 2021 10:33:05 GMT
WORKDIR /etc/varnish
# Tue, 21 Dec 2021 10:33:06 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 21 Dec 2021 10:33:06 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Dec 2021 10:33:07 GMT
EXPOSE 80 8443
# Tue, 21 Dec 2021 10:33:08 GMT
CMD []
```

-	Layers:
	-	`sha256:927a35006d93ea08499b57046904046d7926cd76fb17be193e3e74f56d634a08`  
		Last Modified: Tue, 21 Dec 2021 01:48:54 GMT  
		Size: 30.0 MB (30043793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3132324cb63ca845b64354090627b56cb213f682412e616569edcfff411b0063`  
		Last Modified: Tue, 21 Dec 2021 10:37:01 GMT  
		Size: 65.2 MB (65157463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcddc6003e0c38e0f6b53aa00f16f05a3b2091aadd404eb735e08d104e94fe03`  
		Last Modified: Tue, 21 Dec 2021 10:36:51 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; 386

```console
$ docker pull varnish@sha256:2c1144b3aa8bbebe4de0b386c82cd8c17f34aa8da1a41118f48972ee8c0776b1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.5 MB (102504588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ac112a00fa98d1392dc812b6fa5446c417c8b4f80819896a9e8035ad476aba1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 02:39:54 GMT
ADD file:0284c10b06ba22560408e1e14c1147887f4302c79dba143277ece2e333d6dcbc in / 
# Thu, 02 Dec 2021 02:39:55 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 14:41:26 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 14:48:54 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.6.1.tgz -o $tmpdir/orig.tgz;     echo "af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.6.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 14:48:55 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 14:48:55 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 02 Dec 2021 14:48:55 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 14:48:56 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 14:48:56 GMT
CMD []
```

-	Layers:
	-	`sha256:2df7932f17d752876c686aa22054692a38e88e182dd7b6a5cca7ffce4ffe6f84`  
		Last Modified: Thu, 02 Dec 2021 02:47:59 GMT  
		Size: 32.4 MB (32380814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922c816d4d3f0946beac2d08f5eb0190ec5a80682dc209f8d0329c89b27638d4`  
		Last Modified: Thu, 02 Dec 2021 14:54:43 GMT  
		Size: 70.1 MB (70123075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95fa0cd2f6a540ad99fc42899f545670eebe17aba545ebaed16e3dc88c2e4ba8`  
		Last Modified: Thu, 02 Dec 2021 14:54:22 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; ppc64le

```console
$ docker pull varnish@sha256:5b4892ab3461ddbe3e005f0743fd108f23bd2b5e29ad535ec8eca7ebea149ce7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.3 MB (100286361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9c2cd2e73557a8406f2bef10afbf10709762c0d5ef19fbc0a95de11ae26cd0d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 07:21:21 GMT
ADD file:81a93de7f5dcdbb9397c05b9b6bb7dc5a4742119d46faf929b4c6277b02be7a5 in / 
# Thu, 02 Dec 2021 07:21:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 20:55:25 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 21:40:19 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.6.1.tgz -o $tmpdir/orig.tgz;     echo "af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.6.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 21:40:24 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 21:40:25 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 02 Dec 2021 21:40:28 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 21:40:31 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 21:40:38 GMT
CMD []
```

-	Layers:
	-	`sha256:8d46978b233ccedeaa1cbef7248b214991469fa922cc4fbf9916f9d0711d2d2e`  
		Last Modified: Thu, 02 Dec 2021 07:31:43 GMT  
		Size: 35.3 MB (35271379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0776e5e25a1d33dcf0ac0200fe69c70a222da6eed40bceb51e7425843833e789`  
		Last Modified: Thu, 02 Dec 2021 22:00:09 GMT  
		Size: 65.0 MB (65014280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dd010c4033bde0051434329ac0374d3261fd87e5d9a4dadfe64a52366740e66`  
		Last Modified: Thu, 02 Dec 2021 21:59:55 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; s390x

```console
$ docker pull varnish@sha256:14e377f6877ce74f254ed9ed95d31b7a40d16d4a62a987c4019e65d1d069301d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.7 MB (84737666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b27da94164283f11e04b01eaa1c5e0d71358b3249f3d1448574059b8cd14c53`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 17 Nov 2021 02:42:27 GMT
ADD file:42f73dac307a6a5232e3100f3d3b36e8125f73a4ca504b106e60e2b66d242b2f in / 
# Wed, 17 Nov 2021 02:42:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 12:09:56 GMT
ENV VARNISH_SIZE=100M
# Fri, 19 Nov 2021 02:11:05 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.6.1.tgz -o $tmpdir/orig.tgz;     echo "af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.6.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Fri, 19 Nov 2021 02:11:07 GMT
WORKDIR /etc/varnish
# Fri, 19 Nov 2021 02:11:07 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Fri, 19 Nov 2021 02:11:07 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 19 Nov 2021 02:11:07 GMT
EXPOSE 80 8443
# Fri, 19 Nov 2021 02:11:08 GMT
CMD []
```

-	Layers:
	-	`sha256:8d71e885edf612b507bbdcc48a970548d436b8709eeedfc2c98f6843a214b5e2`  
		Last Modified: Wed, 17 Nov 2021 02:48:25 GMT  
		Size: 29.7 MB (29650960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cbe324e886d9ee47afe369fd7b2c3c3e223f8213f286df5daa395bba36d378f`  
		Last Modified: Fri, 19 Nov 2021 02:12:35 GMT  
		Size: 55.1 MB (55086007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607c8fd5302cec2fa184d34ed2873b257df7dac3ba972aee15614765f9ffa43a`  
		Last Modified: Fri, 19 Nov 2021 02:12:28 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:old-alpine`

```console
$ docker pull varnish@sha256:4c1836081996430a23b736e66ceaa37221580d97ecd0683a47a16ff0e3f09aa6
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
$ docker pull varnish@sha256:452898ec4382082c43e9aad4ad2313939833ac757ed3eedf122dd4107a060862
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.0 MB (57989509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9452c96edc1e2f1f4f52a9471093a1f653d6266bd8a9fae81849688342d1dfcd`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 07:25:45 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 18:27:11 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=6.6.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 18:27:11 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 18:27:11 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Mon, 29 Nov 2021 18:27:12 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 18:27:12 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 18:27:12 GMT
CMD []
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153ae6d73742ceecdf942d8913c25adacffcf7590c180c52467774aae45fbdf8`  
		Last Modified: Mon, 29 Nov 2021 18:31:17 GMT  
		Size: 55.2 MB (55165820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47da88759d700deda407b20295e1fa1b16669b41d326a6ec602f1764725eb339`  
		Last Modified: Mon, 29 Nov 2021 18:31:09 GMT  
		Size: 708.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:c73adc94b1b1fbee8b0d00ecc03446cbe553ec30d20c232bd24ce69ebb15595c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.8 MB (43831597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6f764f7171682d32f568bcc7a144616e93a442db165eee0f50c65b69b4ebc3d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:41:33 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 21:27:56 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=6.6.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 21:27:57 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 21:27:58 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Mon, 29 Nov 2021 21:27:58 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 21:27:59 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 21:27:59 GMT
CMD []
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45906a707d1a67dd18797169bbfe25bac52a1b464e7f990698da21fddd7475c0`  
		Last Modified: Mon, 29 Nov 2021 21:37:33 GMT  
		Size: 41.4 MB (41392271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740d9723635b34441b27b262933bd4b8418b26b67f4045cc9f64ec89bc227fd3`  
		Last Modified: Mon, 29 Nov 2021 21:37:11 GMT  
		Size: 708.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:2a37d0c77875b555f8ca6eb95423051dccd662fc043139f3ca0c454b3297c3d0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50731977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97f125861bc75731dc461286c1d1b0a2b17c8e0f205c97df4543729f7a8b7352`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:02:27 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 20:48:16 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=6.6.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 20:48:17 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 20:48:19 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Mon, 29 Nov 2021 20:48:19 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 20:48:20 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 20:48:21 GMT
CMD []
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9a5a9eecb648d857587d324062b4f87bb9dc62e6a4cb827c9e4464961c2e59`  
		Last Modified: Mon, 29 Nov 2021 20:52:51 GMT  
		Size: 48.0 MB (48013567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e736777a13cbd6c9e14db297a5c4bbb132c234eeeff9c10b17cd5452cd362216`  
		Last Modified: Mon, 29 Nov 2021 20:52:44 GMT  
		Size: 710.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; 386

```console
$ docker pull varnish@sha256:8d0d547249a14cde7e3bd5e01c2a40ddf1ba74cb90d66f5a093034cfff3e55c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58199339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0336cd46aeafd4ae83b0b6dc96d0f1f1614ec9ba408969822994a117199191bc`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:38:42 GMT
ADD file:403428c2903dd9dea10d069185873cb2c2c3149c553797807c69f22aa3d12fe3 in / 
# Fri, 12 Nov 2021 16:38:42 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 20:27:36 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 20:01:00 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=6.6.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 20:01:01 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 20:01:01 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Mon, 29 Nov 2021 20:01:01 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 20:01:01 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 20:01:02 GMT
CMD []
```

-	Layers:
	-	`sha256:5420e0d28c84ecb16748cb90cc6acf8e2a81dab10cb1f674f3eee8533e53c62a`  
		Last Modified: Fri, 12 Nov 2021 16:39:36 GMT  
		Size: 2.8 MB (2830948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d909c7ab2ae0be7fc0e4ae7aa02aa06a2e44ad53f3cff2268bfeed6937c499c3`  
		Last Modified: Mon, 29 Nov 2021 20:02:44 GMT  
		Size: 55.4 MB (55367685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19722b94f50ff8a0a17e55d0b2919cf221589ab013ad66a822669ae094c020de`  
		Last Modified: Mon, 29 Nov 2021 20:02:34 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:377e24a918f548a09f38a533afdcdecf4d9a30f2286434bce625df8260f06411
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47836328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fdc983240c36081b8a4d544f472904fa029137f9e87f69d41b24b43d0a16ca7`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 21:18:00 GMT
ADD file:4d45063079cb28a34f1e382fddb22f156ac99d5449aa05ed37cb653c1f7b80f2 in / 
# Fri, 12 Nov 2021 21:18:01 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:52:07 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 19:56:23 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=6.6.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 19:56:29 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 19:56:32 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Mon, 29 Nov 2021 19:56:34 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 19:56:35 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 19:56:36 GMT
CMD []
```

-	Layers:
	-	`sha256:72940440c1ab65eca4d38846164719ffde4b147543cc658d041407a925b13368`  
		Last Modified: Fri, 12 Nov 2021 21:19:32 GMT  
		Size: 2.8 MB (2817467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e0a28c63680f4f963ab893db97224b8d2b5ff2d6e06ea1e743d9c3731ebc85`  
		Last Modified: Mon, 29 Nov 2021 20:15:27 GMT  
		Size: 45.0 MB (45018158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7d4295e98da2f81183f70ef0dc76d1d3490a26ffcbf6354434e1651d44ae3c`  
		Last Modified: Mon, 29 Nov 2021 20:15:19 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:e1001918850b37c9a482e47544f06bfb1808f199cd9d7bf5e33d35c132ba702a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.4 MB (46372307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5888cbaa2a9d39840aedcdd59b0feb27f3687cbcd2be29caff8898de3799d2a6`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:41:35 GMT
ADD file:7e0cf02b3f015b1a0f867c03b2902b85f2140be1cee7af63c23f367a487e4577 in / 
# Fri, 12 Nov 2021 16:41:36 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 22:10:22 GMT
ENV VARNISH_SIZE=100M
# Mon, 29 Nov 2021 20:08:19 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=6.6.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Mon, 29 Nov 2021 20:08:20 GMT
WORKDIR /etc/varnish
# Mon, 29 Nov 2021 20:08:20 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Mon, 29 Nov 2021 20:08:20 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 29 Nov 2021 20:08:21 GMT
EXPOSE 80 8443
# Mon, 29 Nov 2021 20:08:21 GMT
CMD []
```

-	Layers:
	-	`sha256:817a13b0e05928f7491adbf1d2cf261ec35079112247bd03469bbe31156aca7c`  
		Last Modified: Fri, 12 Nov 2021 16:42:44 GMT  
		Size: 2.6 MB (2609278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2b2b1073e64d39da57603b96e9b9171e48a505e0e09a02cfd3e29658a2a58a`  
		Last Modified: Mon, 29 Nov 2021 20:11:46 GMT  
		Size: 43.8 MB (43762322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35ef3ae417d6531198e3ab2b6a00ef57d1474d0dde453fff48250ed6cf22703`  
		Last Modified: Mon, 29 Nov 2021 20:11:40 GMT  
		Size: 707.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:stable`

```console
$ docker pull varnish@sha256:786e9bd61f197b2720853007c7c507c6bdc71f4e3236e03d35da367a01e2d116
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
$ docker pull varnish@sha256:a21d8beb55aa8f902b55a6f773c581dcd6537a8883d0d24b5d32c18f1b662bdb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100572918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58725732895fe16eebccbad29fc67442778d35629b74e64b49b44538eaa3dcfe`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 02:48:20 GMT
ADD file:ece5ff85ca549f0b1e9139d29dcb43a52af672d0591c423e28180f6d8d700ad7 in / 
# Thu, 02 Dec 2021 02:48:21 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 17:48:20 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 17:58:16 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.0.8.tgz -o $tmpdir/orig.tgz;     echo "73ed2f465ba3b11680b20a70633fc78da9b3eac68395f927b7ff02f4106b6cc92a2b395db2813a0605da2771530e5c4fc594eaf5a9a32bf2e42181b6dd90cf3f  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.8|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 17:58:17 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 17:58:17 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 02 Dec 2021 17:58:17 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 17:58:17 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 17:58:18 GMT
CMD []
```

-	Layers:
	-	`sha256:e5ae68f740265288a4888db98d2999a638fdcb6d725f427678814538d253aa4d`  
		Last Modified: Thu, 02 Dec 2021 02:53:46 GMT  
		Size: 31.4 MB (31370221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3cfaf0bcb14454b543ce0498ecb01e3e93089900b28fb13ae862bb38a29a84`  
		Last Modified: Thu, 02 Dec 2021 17:59:42 GMT  
		Size: 69.2 MB (69201997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c37ac8a55c4f5f4a2cb6e64b5198e81377fdfa11ec23d4000d7c90e35edb37`  
		Last Modified: Thu, 02 Dec 2021 17:59:29 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; arm variant v7

```console
$ docker pull varnish@sha256:78c279b4c10a6687be3db34d347f867a234def120a1e06dc418c7f7e44a9c727
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77216753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57d84c4c56a5deeba196ae1f0a545651321f1381d4f6bc472f4495ce898ecfdf`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 09:05:17 GMT
ADD file:97ce5af9ff4fb4002733d5c402ddc01a13e765d31b85bb6525a7fa797b698e10 in / 
# Thu, 02 Dec 2021 09:05:17 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 17:16:05 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 17:34:44 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.0.8.tgz -o $tmpdir/orig.tgz;     echo "73ed2f465ba3b11680b20a70633fc78da9b3eac68395f927b7ff02f4106b6cc92a2b395db2813a0605da2771530e5c4fc594eaf5a9a32bf2e42181b6dd90cf3f  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.8|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 17:34:45 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 17:34:45 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 02 Dec 2021 17:34:46 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 17:34:46 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 17:34:47 GMT
CMD []
```

-	Layers:
	-	`sha256:ba82a1312e1efdcd1cc6eb31cd40358dcec180da31779dac399cba31bf3dc206`  
		Last Modified: Thu, 02 Dec 2021 09:21:03 GMT  
		Size: 26.6 MB (26573192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a26aabdc4af6fcc2f87ffedefcd2035994ad7c44dbfc8ca07bcc82b1fd49ac0`  
		Last Modified: Thu, 02 Dec 2021 17:38:18 GMT  
		Size: 50.6 MB (50642860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2885c8aa3ff49bada1b1b2038107980ee649083c64c42d6534df3bf77cbf35`  
		Last Modified: Thu, 02 Dec 2021 17:37:55 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:ac60c1e4761cc40d24baa103506086f6f415a4b67f72d02a4342ee7208300669
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94686680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:967bad5c1de22c86008e49361e2caf5e5e47e81271b94caf94047c037d70e1aa`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Dec 2021 01:42:23 GMT
ADD file:986f91febed4aa8e2072081ff8419d52ba2060510822e717086d3b3d9469e4d7 in / 
# Tue, 21 Dec 2021 01:42:24 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:28:06 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Dec 2021 10:35:31 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.0.8.tgz -o $tmpdir/orig.tgz;     echo "73ed2f465ba3b11680b20a70633fc78da9b3eac68395f927b7ff02f4106b6cc92a2b395db2813a0605da2771530e5c4fc594eaf5a9a32bf2e42181b6dd90cf3f  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.8|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 21 Dec 2021 10:35:31 GMT
WORKDIR /etc/varnish
# Tue, 21 Dec 2021 10:35:33 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 21 Dec 2021 10:35:33 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Dec 2021 10:35:34 GMT
EXPOSE 80 8443
# Tue, 21 Dec 2021 10:35:35 GMT
CMD []
```

-	Layers:
	-	`sha256:927a35006d93ea08499b57046904046d7926cd76fb17be193e3e74f56d634a08`  
		Last Modified: Tue, 21 Dec 2021 01:48:54 GMT  
		Size: 30.0 MB (30043793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2fa237057a545eaaa1d2005ed3acdefbf217c0e1186f5bc68ca4c0c5a311d6`  
		Last Modified: Tue, 21 Dec 2021 10:37:27 GMT  
		Size: 64.6 MB (64642186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d3a2610175a2cea7772fba94f24c41446ac559e3d93f920dce10b8975fdc34`  
		Last Modified: Tue, 21 Dec 2021 10:37:16 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; 386

```console
$ docker pull varnish@sha256:5ad40751894382694f868022af125c7b5b4bd737d339d465b4a1c175cd41bb2b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102062918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fc599f425f815d23bedac0d4d540e4a345932db7bc20035e03ccea8ee192045`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 02:39:54 GMT
ADD file:0284c10b06ba22560408e1e14c1147887f4302c79dba143277ece2e333d6dcbc in / 
# Thu, 02 Dec 2021 02:39:55 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 14:41:26 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 14:52:24 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.0.8.tgz -o $tmpdir/orig.tgz;     echo "73ed2f465ba3b11680b20a70633fc78da9b3eac68395f927b7ff02f4106b6cc92a2b395db2813a0605da2771530e5c4fc594eaf5a9a32bf2e42181b6dd90cf3f  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.8|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 14:52:25 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 14:52:25 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 02 Dec 2021 14:52:25 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 14:52:26 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 14:52:26 GMT
CMD []
```

-	Layers:
	-	`sha256:2df7932f17d752876c686aa22054692a38e88e182dd7b6a5cca7ffce4ffe6f84`  
		Last Modified: Thu, 02 Dec 2021 02:47:59 GMT  
		Size: 32.4 MB (32380814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6f8f5993208760bfd785dee6370007dde3e7837d9dc7e3cc74206ad6e54b6f`  
		Last Modified: Thu, 02 Dec 2021 14:55:16 GMT  
		Size: 69.7 MB (69681403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1900d954ea8bc8ac629ec212ad0ff3da652ff5189d2138156bb2445aefc20179`  
		Last Modified: Thu, 02 Dec 2021 14:55:01 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; ppc64le

```console
$ docker pull varnish@sha256:85b85d37828bb1349bc6dffa742f97d110d48b08ade48b00e4614db87669821b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.8 MB (99776391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:477f13d57ec581eb6568aee6dc2eaad1148d9fcc2e856cb9a237f5adc4c27574`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 07:21:21 GMT
ADD file:81a93de7f5dcdbb9397c05b9b6bb7dc5a4742119d46faf929b4c6277b02be7a5 in / 
# Thu, 02 Dec 2021 07:21:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 20:55:25 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 21:58:15 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.0.8.tgz -o $tmpdir/orig.tgz;     echo "73ed2f465ba3b11680b20a70633fc78da9b3eac68395f927b7ff02f4106b6cc92a2b395db2813a0605da2771530e5c4fc594eaf5a9a32bf2e42181b6dd90cf3f  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.8|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 21:58:21 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 21:58:22 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 02 Dec 2021 21:58:24 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 21:58:26 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 21:58:28 GMT
CMD []
```

-	Layers:
	-	`sha256:8d46978b233ccedeaa1cbef7248b214991469fa922cc4fbf9916f9d0711d2d2e`  
		Last Modified: Thu, 02 Dec 2021 07:31:43 GMT  
		Size: 35.3 MB (35271379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07dc89dd1f6108b0a247a91d91d5167422d9f447169268fc11f4d289a75f70a6`  
		Last Modified: Thu, 02 Dec 2021 22:00:40 GMT  
		Size: 64.5 MB (64504309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90804dc475998e237ff6f2f044f47b7bca1ae4d009676626f1761c1b44556496`  
		Last Modified: Thu, 02 Dec 2021 22:00:26 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; s390x

```console
$ docker pull varnish@sha256:1a58eec42888f09f1a1c33c632b474197658d4e07d04aa36f581a0254a457ed0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.0 MB (80994821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd2857448b98a5e632f673a99702a81e5cf9f880873cb813e97c3534237fb56b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 02 Dec 2021 07:19:07 GMT
ADD file:9303def035f391c14bdca007751c5061f36fe929d5b3f4d725ce376e25f7dd36 in / 
# Thu, 02 Dec 2021 07:19:09 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 12:47:34 GMT
ENV VARNISH_SIZE=100M
# Thu, 02 Dec 2021 12:52:13 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.0.8.tgz -o $tmpdir/orig.tgz;     echo "73ed2f465ba3b11680b20a70633fc78da9b3eac68395f927b7ff02f4106b6cc92a2b395db2813a0605da2771530e5c4fc594eaf5a9a32bf2e42181b6dd90cf3f  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.8|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 02 Dec 2021 12:52:15 GMT
WORKDIR /etc/varnish
# Thu, 02 Dec 2021 12:52:15 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 02 Dec 2021 12:52:15 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 02 Dec 2021 12:52:15 GMT
EXPOSE 80 8443
# Thu, 02 Dec 2021 12:52:15 GMT
CMD []
```

-	Layers:
	-	`sha256:bf2c280d82ca10801fb58bfc3f73029eef17592cbe00e94875cb189bdbac0c5f`  
		Last Modified: Thu, 02 Dec 2021 07:25:12 GMT  
		Size: 29.7 MB (29650954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b1cead4f753add4eee5c4fa71deb8b75b67a36d59deb9b760aa7bc95189a11`  
		Last Modified: Thu, 02 Dec 2021 12:53:33 GMT  
		Size: 51.3 MB (51343165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd72e0b5d5556153d85da35fb2538e849772bf4fdfa087a050284b761e28953`  
		Last Modified: Thu, 02 Dec 2021 12:53:26 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
