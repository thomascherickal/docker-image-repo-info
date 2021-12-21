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
