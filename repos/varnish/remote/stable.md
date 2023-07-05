## `varnish:stable`

```console
$ docker pull varnish@sha256:f8beeaa5e9dbdbb17461a814c34d2e40642e469a3717eebdd7ff3242102a8465
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
$ docker pull varnish@sha256:7afcf2425caa7ed5ddb919326c85b4ff422a30d7053d8707d2d010c8ee3e36ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.8 MB (95774849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0df77fb8530dd64c369b5d34d8baeaa80fa92e9fccef28f47d46acdf9aeee20c`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:22:19 GMT
ENV VARNISH_SIZE=100M
# Wed, 05 Jul 2023 20:35:29 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 05 Jul 2023 20:35:30 GMT
WORKDIR /etc/varnish
# Wed, 05 Jul 2023 20:35:30 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 05 Jul 2023 20:35:30 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 05 Jul 2023 20:35:30 GMT
EXPOSE 80 8443
# Wed, 05 Jul 2023 20:35:30 GMT
CMD []
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65e2685167689dda082819a4b53f9d786d7bdbbdee67ed4bfb3f5facf0e84dc8`  
		Last Modified: Wed, 05 Jul 2023 20:37:23 GMT  
		Size: 64.4 MB (64356761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a417559af27508c861a0e5dfbb77f11ce7134a0621b2d9064aa8de77df2333`  
		Last Modified: Wed, 05 Jul 2023 20:37:14 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; arm variant v7

```console
$ docker pull varnish@sha256:3ae6a838bc8d8d509788ed4691c636d50615009b56d4b1ebae6a0443f53eb2d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.8 MB (72777661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1e6d81a029381bfb806c3fbf48d63433f2ccf69b47c0b85e526103bd611e3f8`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Jul 2023 00:58:20 GMT
ADD file:c023c66ee4b7cdae5c542f2ad2dd35aef94ad24e1b3b479a16538c46013ae6a5 in / 
# Tue, 04 Jul 2023 00:58:21 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:44:00 GMT
ENV VARNISH_SIZE=100M
# Wed, 05 Jul 2023 21:15:19 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 05 Jul 2023 21:15:20 GMT
WORKDIR /etc/varnish
# Wed, 05 Jul 2023 21:15:20 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 05 Jul 2023 21:15:20 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 05 Jul 2023 21:15:20 GMT
EXPOSE 80 8443
# Wed, 05 Jul 2023 21:15:20 GMT
CMD []
```

-	Layers:
	-	`sha256:d9e6a8b782e380f447723ac26499c5014f2d383b9210819b9e73e97abaf81249`  
		Last Modified: Tue, 04 Jul 2023 01:03:35 GMT  
		Size: 26.6 MB (26578754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1357362ca19318246d42a1c0b2c89be0767080971f6c802c958c0a09c9eeaee3`  
		Last Modified: Wed, 05 Jul 2023 21:17:08 GMT  
		Size: 46.2 MB (46198210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e475c508639e0dddacf4bac09e0da3c6685713bea5f4b4a63b55edc61a579bf`  
		Last Modified: Wed, 05 Jul 2023 21:17:02 GMT  
		Size: 697.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:7938b821826fdc971edc4058be8eac59e18e4b8c627f5880d443a4d3794b2b17
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.9 MB (89875701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b3c44fd6afb68f3a2eab797c2b31846383964862c3a964987b4de89dddb4757`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:01:37 GMT
ENV VARNISH_SIZE=100M
# Wed, 05 Jul 2023 20:51:32 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 05 Jul 2023 20:51:32 GMT
WORKDIR /etc/varnish
# Wed, 05 Jul 2023 20:51:33 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 05 Jul 2023 20:51:33 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 05 Jul 2023 20:51:33 GMT
EXPOSE 80 8443
# Wed, 05 Jul 2023 20:51:33 GMT
CMD []
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814c66344faeb9561505c1af3f3797f9d09dd0e50864864ac5be9ce6efe1c84b`  
		Last Modified: Wed, 05 Jul 2023 20:53:11 GMT  
		Size: 59.8 MB (59812046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fcb4ee5ee74d8fc124d8e155fe18f8e86713330de50e63ed7f849e8c1f8568`  
		Last Modified: Wed, 05 Jul 2023 20:53:05 GMT  
		Size: 698.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; 386

```console
$ docker pull varnish@sha256:307ed644593ab6a27041b5b5126571f82b32f8fa1e490c0471a296a70960a49f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.1 MB (97070586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e9559e3ff384c58dfb1b026822d008fd5f0048fa30254c94b8898b439206780`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Jul 2023 01:38:59 GMT
ADD file:c39e332ccb9cb890ba7896a09e9f074b3c8d67094b4eaf73d5c67e8949c2e0be in / 
# Tue, 04 Jul 2023 01:39:00 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 09:07:42 GMT
ENV VARNISH_SIZE=100M
# Wed, 05 Jul 2023 21:56:10 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 05 Jul 2023 21:56:11 GMT
WORKDIR /etc/varnish
# Wed, 05 Jul 2023 21:56:11 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 05 Jul 2023 21:56:11 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 05 Jul 2023 21:56:11 GMT
EXPOSE 80 8443
# Wed, 05 Jul 2023 21:56:11 GMT
CMD []
```

-	Layers:
	-	`sha256:3466e7f9e8ec982697fc130dbb1706d708f5c53e348a638019a955c15c7395af`  
		Last Modified: Tue, 04 Jul 2023 01:44:12 GMT  
		Size: 32.4 MB (32397496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:543abe8fec4ed040da44a0567cac5ec8dada3d28338e1b2e4f640672c0964da6`  
		Last Modified: Wed, 05 Jul 2023 21:58:15 GMT  
		Size: 64.7 MB (64672390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f9773b86057d4eb302fca40fa03021dcc043d0b79bcb998d36d29628acb8a6`  
		Last Modified: Wed, 05 Jul 2023 21:58:03 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; ppc64le

```console
$ docker pull varnish@sha256:a83bb6b81377793cf51ca5f6723d292d6daa258ca9bcd7c1556078b0bccffd19
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.8 MB (99809410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1ce2fed0cb98e1da3aebf766e125c08c35f0f2e737acf0d30430eee5cc82c10`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Jul 2023 01:18:33 GMT
ADD file:37fa020aca7253d41d395ed529c38db73caaa4da098754836244552f65fa7d5d in / 
# Tue, 04 Jul 2023 01:18:35 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:14:58 GMT
ENV VARNISH_SIZE=100M
# Tue, 04 Jul 2023 03:22:54 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 04 Jul 2023 03:22:59 GMT
WORKDIR /etc/varnish
# Tue, 04 Jul 2023 03:22:59 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 04 Jul 2023 03:23:01 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 04 Jul 2023 03:23:03 GMT
EXPOSE 80 8443
# Tue, 04 Jul 2023 03:23:04 GMT
CMD []
```

-	Layers:
	-	`sha256:147bb8b5828c99cd6b07d252d2987490463c142099eaa0815025685f8fa4f3d8`  
		Last Modified: Tue, 04 Jul 2023 01:25:40 GMT  
		Size: 35.3 MB (35291082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2515e643cad9686b51c4bd217b1491fa0991abc06c0bde5fe6e3e71b9f39305`  
		Last Modified: Tue, 04 Jul 2023 03:25:15 GMT  
		Size: 64.5 MB (64517627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbfb5497f9ba00b211c53b9e65d75bf5b937d3324c7a49efff432a9225cd6200`  
		Last Modified: Tue, 04 Jul 2023 03:24:59 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; s390x

```console
$ docker pull varnish@sha256:3cca7610648d5a2606e93e6b390c26c123a6ff109f62ad369a74c66d581d7c4b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76186965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6403b6fd0cc5e9a19a583ee90fa41c15353333c56c96b66c7591f8072886b562`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Jul 2023 01:32:44 GMT
ADD file:799c0afa70fa3bf4bb7804964481cba79e80aa3fad5c7a25beadde206ed6a8ff in / 
# Tue, 04 Jul 2023 01:32:46 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:12:56 GMT
ENV VARNISH_SIZE=100M
# Wed, 05 Jul 2023 19:44:57 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 05 Jul 2023 19:45:03 GMT
WORKDIR /etc/varnish
# Wed, 05 Jul 2023 19:45:03 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 05 Jul 2023 19:45:04 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 05 Jul 2023 19:45:04 GMT
EXPOSE 80 8443
# Wed, 05 Jul 2023 19:45:05 GMT
CMD []
```

-	Layers:
	-	`sha256:bbee891481f2623da9c7d37a49947926519c858c2b06773370a6189440d4b4de`  
		Last Modified: Tue, 04 Jul 2023 01:37:37 GMT  
		Size: 29.7 MB (29652540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc37e06f5c17faa79cb8dd0eb96221cc0c1b778d5760750364236d5416cf879f`  
		Last Modified: Wed, 05 Jul 2023 19:46:51 GMT  
		Size: 46.5 MB (46533723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68965bfda60b16401692ae7302023ebebb868719aa46cc503f202796f466fd6`  
		Last Modified: Wed, 05 Jul 2023 19:46:44 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
