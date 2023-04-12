<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `varnish`

-	[`varnish:6.0`](#varnish60)
-	[`varnish:6.0.11`](#varnish6011)
-	[`varnish:7.2`](#varnish72)
-	[`varnish:7.2-alpine`](#varnish72-alpine)
-	[`varnish:7.2.1`](#varnish721)
-	[`varnish:7.2.1-alpine`](#varnish721-alpine)
-	[`varnish:7.3`](#varnish73)
-	[`varnish:7.3-alpine`](#varnish73-alpine)
-	[`varnish:7.3.0`](#varnish730)
-	[`varnish:7.3.0-alpine`](#varnish730-alpine)
-	[`varnish:alpine`](#varnishalpine)
-	[`varnish:fresh`](#varnishfresh)
-	[`varnish:fresh-alpine`](#varnishfresh-alpine)
-	[`varnish:latest`](#varnishlatest)
-	[`varnish:old`](#varnishold)
-	[`varnish:old-alpine`](#varnishold-alpine)
-	[`varnish:stable`](#varnishstable)

## `varnish:6.0`

```console
$ docker pull varnish@sha256:0e992a9c53300db59932059504d8df94b965ddf0c0db2a47c8bc83029b93f67e
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
$ docker pull varnish@sha256:f593b51393e4edffa20e5bb0fcfeef6bf09dd71a6ecd254ef9a055448e39d9ef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100660685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f821874ee374fc2690cc271a857a80cd79f288fa99c09daa13296016f8c6bc93`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:42:11 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 07:44:11 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 12 Apr 2023 07:44:11 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 07:44:11 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 12 Apr 2023 07:44:11 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 07:44:11 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 07:44:11 GMT
CMD []
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274c9ddef5cd48e2463d6b5bc111d79368c0f10f6a1040041952253bde9de5d8`  
		Last Modified: Wed, 12 Apr 2023 07:45:24 GMT  
		Size: 69.2 MB (69241757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d351ea0dbe4d60c605b1dc412d644d729517137393f865e66240a64582514b7e`  
		Last Modified: Wed, 12 Apr 2023 07:45:15 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; arm variant v7

```console
$ docker pull varnish@sha256:1eaf25f8067fb7f5f24129515c2d6043b571f15d7cb9b4f3082775fdebecbf4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77230907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b4d723caf3307762828942958dc505a55bb9d17a6a45d3a26652aa88fcabf4b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 11 Apr 2023 23:59:44 GMT
ADD file:e5f4777456ed4424053e9aa1f3d783f57da094c7a6c6d9d7a2fd315e00b5bbb0 in / 
# Tue, 11 Apr 2023 23:59:44 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 09:55:33 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 09:57:38 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 12 Apr 2023 09:57:38 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 09:57:38 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 12 Apr 2023 09:57:39 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 09:57:39 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 09:57:39 GMT
CMD []
```

-	Layers:
	-	`sha256:99c2a28b4a43ce341eb611e82106b886315f30a250473617f2293828e10d8fff`  
		Last Modified: Wed, 12 Apr 2023 00:03:19 GMT  
		Size: 26.6 MB (26579772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529f9895b0f9e006c21d373370b249b754e53c9c65c36ac74a7d119107e866d3`  
		Last Modified: Wed, 12 Apr 2023 09:58:37 GMT  
		Size: 50.7 MB (50650437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3dec06d3bbb4fa400129ccde514435125382ce56882357ccaac867c7ec5946c`  
		Last Modified: Wed, 12 Apr 2023 09:58:28 GMT  
		Size: 698.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:4497b8996cff43dd8a560c68964fe29e13a8db946473a82376e209dc0810beee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94717057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:007c8e618536b021221201d9958b4cd97558922fa549482bda3875fc2066dbcf`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 04:51:01 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 04:52:43 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 12 Apr 2023 04:52:44 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 04:52:44 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:52:44 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 04:52:44 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 04:52:44 GMT
CMD []
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:682527444ab1be7526396ac0bbb4f292068e8474d19254d67e495ea8f451be15`  
		Last Modified: Wed, 12 Apr 2023 04:53:48 GMT  
		Size: 64.7 MB (64652529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3454f24f83fdb3c9d4943c12fa0e06a0eeefe8b0012e9a5cae6dfcd89951dc1`  
		Last Modified: Wed, 12 Apr 2023 04:53:42 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; 386

```console
$ docker pull varnish@sha256:e3ae418f25ec73834e468b452e5b23e4d982b9cdcc0bdacaada801c58d054ba7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102083639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9c15e2d6a853229156a560e293584edb697596ab5e92252ab7b3a8f610c8a2b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:39:01 GMT
ADD file:42fc1b4536cdd6823499b0c94d799e9bfbcb280b7df55d8d6c9f6defd61ecb6e in / 
# Wed, 12 Apr 2023 00:39:01 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 04:22:01 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 04:24:29 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 12 Apr 2023 04:24:30 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 04:24:30 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:24:30 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 04:24:30 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 04:24:30 GMT
CMD []
```

-	Layers:
	-	`sha256:b2ee1f87789d52ef09851b4e5c9745fb8aceafa107b0d3452f9973f1abe65042`  
		Last Modified: Wed, 12 Apr 2023 00:42:45 GMT  
		Size: 32.4 MB (32398925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7355f41e5a426f8365e4578b296a964249f2359611192c75a22733eea31f2240`  
		Last Modified: Wed, 12 Apr 2023 04:25:52 GMT  
		Size: 69.7 MB (69684014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039d3b8c0e5dc9639808d5b8759e0ce0959c03ea06755da1fed6f9d662a4192d`  
		Last Modified: Wed, 12 Apr 2023 04:25:39 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; ppc64le

```console
$ docker pull varnish@sha256:18bd3322c2f9ccc96bfce197018af7ff9306a5913379476af9c84e061e770095
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.8 MB (99803629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27f0683fd328a003ec4c95f0c7d93bb88582d34cba7b9ea9a048b186914841c5`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:08:20 GMT
ADD file:63eb52aaff02c15bceabb87a78eb1b36389066ff4774cf8a754160ca7d509816 in / 
# Wed, 12 Apr 2023 00:08:23 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:06:51 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 01:16:48 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 12 Apr 2023 01:16:52 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 01:16:52 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 12 Apr 2023 01:16:53 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 01:16:53 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 01:16:54 GMT
CMD []
```

-	Layers:
	-	`sha256:5b41d5ec640939cf684959234ad3b80909268a32bfd520a31c6720a91521c2fa`  
		Last Modified: Wed, 12 Apr 2023 00:13:13 GMT  
		Size: 35.3 MB (35291995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c91ede6f2abd53adaec518fad85de307f689c38e8eab390a7359e142ae3a16`  
		Last Modified: Wed, 12 Apr 2023 01:18:31 GMT  
		Size: 64.5 MB (64510930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd33a842deca9de4a3e249248620b5666ab2fa35cae6fe8b10b79955f955c3e`  
		Last Modified: Wed, 12 Apr 2023 01:18:15 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; s390x

```console
$ docker pull varnish@sha256:91cf8dba2788f88ad8b8f188bb53c43d9b749547de652b93d26493f0c3cac63f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.0 MB (81006609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0df2b025628576f460505157da9b8f5f06d418c21686950786d49f881b8f9b2a`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:01:00 GMT
ADD file:b6463dba97ba9c0a29bacfafc4d67bc603ab57e80b75e23cd42d7ef4b0f8e6ae in / 
# Wed, 12 Apr 2023 00:01:04 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:50:27 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 07:52:14 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 12 Apr 2023 07:52:17 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 07:52:17 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 12 Apr 2023 07:52:17 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 07:52:17 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 07:52:17 GMT
CMD []
```

-	Layers:
	-	`sha256:97fe10bc7def58e7938e97e41eec4788ec7a45b6ef2cb1770cec02fa831fd19d`  
		Last Modified: Wed, 12 Apr 2023 00:05:18 GMT  
		Size: 29.7 MB (29653156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7822e42c3387f3cd91539d4e97252f558b188301244bec6480d7540b6a80882`  
		Last Modified: Wed, 12 Apr 2023 07:53:20 GMT  
		Size: 51.4 MB (51352752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750915994cfaac0ec2feb5390e1d622af471974ba829d7b86d1edf3d6b3beb0d`  
		Last Modified: Wed, 12 Apr 2023 07:53:13 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0.11`

```console
$ docker pull varnish@sha256:0e992a9c53300db59932059504d8df94b965ddf0c0db2a47c8bc83029b93f67e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:6.0.11` - linux; amd64

```console
$ docker pull varnish@sha256:f593b51393e4edffa20e5bb0fcfeef6bf09dd71a6ecd254ef9a055448e39d9ef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100660685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f821874ee374fc2690cc271a857a80cd79f288fa99c09daa13296016f8c6bc93`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:42:11 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 07:44:11 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 12 Apr 2023 07:44:11 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 07:44:11 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 12 Apr 2023 07:44:11 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 07:44:11 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 07:44:11 GMT
CMD []
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274c9ddef5cd48e2463d6b5bc111d79368c0f10f6a1040041952253bde9de5d8`  
		Last Modified: Wed, 12 Apr 2023 07:45:24 GMT  
		Size: 69.2 MB (69241757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d351ea0dbe4d60c605b1dc412d644d729517137393f865e66240a64582514b7e`  
		Last Modified: Wed, 12 Apr 2023 07:45:15 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.11` - linux; arm variant v7

```console
$ docker pull varnish@sha256:1eaf25f8067fb7f5f24129515c2d6043b571f15d7cb9b4f3082775fdebecbf4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77230907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b4d723caf3307762828942958dc505a55bb9d17a6a45d3a26652aa88fcabf4b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 11 Apr 2023 23:59:44 GMT
ADD file:e5f4777456ed4424053e9aa1f3d783f57da094c7a6c6d9d7a2fd315e00b5bbb0 in / 
# Tue, 11 Apr 2023 23:59:44 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 09:55:33 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 09:57:38 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 12 Apr 2023 09:57:38 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 09:57:38 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 12 Apr 2023 09:57:39 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 09:57:39 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 09:57:39 GMT
CMD []
```

-	Layers:
	-	`sha256:99c2a28b4a43ce341eb611e82106b886315f30a250473617f2293828e10d8fff`  
		Last Modified: Wed, 12 Apr 2023 00:03:19 GMT  
		Size: 26.6 MB (26579772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529f9895b0f9e006c21d373370b249b754e53c9c65c36ac74a7d119107e866d3`  
		Last Modified: Wed, 12 Apr 2023 09:58:37 GMT  
		Size: 50.7 MB (50650437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3dec06d3bbb4fa400129ccde514435125382ce56882357ccaac867c7ec5946c`  
		Last Modified: Wed, 12 Apr 2023 09:58:28 GMT  
		Size: 698.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.11` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:4497b8996cff43dd8a560c68964fe29e13a8db946473a82376e209dc0810beee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94717057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:007c8e618536b021221201d9958b4cd97558922fa549482bda3875fc2066dbcf`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 04:51:01 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 04:52:43 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 12 Apr 2023 04:52:44 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 04:52:44 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:52:44 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 04:52:44 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 04:52:44 GMT
CMD []
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:682527444ab1be7526396ac0bbb4f292068e8474d19254d67e495ea8f451be15`  
		Last Modified: Wed, 12 Apr 2023 04:53:48 GMT  
		Size: 64.7 MB (64652529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3454f24f83fdb3c9d4943c12fa0e06a0eeefe8b0012e9a5cae6dfcd89951dc1`  
		Last Modified: Wed, 12 Apr 2023 04:53:42 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.11` - linux; 386

```console
$ docker pull varnish@sha256:e3ae418f25ec73834e468b452e5b23e4d982b9cdcc0bdacaada801c58d054ba7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102083639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9c15e2d6a853229156a560e293584edb697596ab5e92252ab7b3a8f610c8a2b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:39:01 GMT
ADD file:42fc1b4536cdd6823499b0c94d799e9bfbcb280b7df55d8d6c9f6defd61ecb6e in / 
# Wed, 12 Apr 2023 00:39:01 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 04:22:01 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 04:24:29 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 12 Apr 2023 04:24:30 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 04:24:30 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:24:30 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 04:24:30 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 04:24:30 GMT
CMD []
```

-	Layers:
	-	`sha256:b2ee1f87789d52ef09851b4e5c9745fb8aceafa107b0d3452f9973f1abe65042`  
		Last Modified: Wed, 12 Apr 2023 00:42:45 GMT  
		Size: 32.4 MB (32398925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7355f41e5a426f8365e4578b296a964249f2359611192c75a22733eea31f2240`  
		Last Modified: Wed, 12 Apr 2023 04:25:52 GMT  
		Size: 69.7 MB (69684014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039d3b8c0e5dc9639808d5b8759e0ce0959c03ea06755da1fed6f9d662a4192d`  
		Last Modified: Wed, 12 Apr 2023 04:25:39 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.11` - linux; ppc64le

```console
$ docker pull varnish@sha256:18bd3322c2f9ccc96bfce197018af7ff9306a5913379476af9c84e061e770095
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.8 MB (99803629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27f0683fd328a003ec4c95f0c7d93bb88582d34cba7b9ea9a048b186914841c5`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:08:20 GMT
ADD file:63eb52aaff02c15bceabb87a78eb1b36389066ff4774cf8a754160ca7d509816 in / 
# Wed, 12 Apr 2023 00:08:23 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:06:51 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 01:16:48 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 12 Apr 2023 01:16:52 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 01:16:52 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 12 Apr 2023 01:16:53 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 01:16:53 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 01:16:54 GMT
CMD []
```

-	Layers:
	-	`sha256:5b41d5ec640939cf684959234ad3b80909268a32bfd520a31c6720a91521c2fa`  
		Last Modified: Wed, 12 Apr 2023 00:13:13 GMT  
		Size: 35.3 MB (35291995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c91ede6f2abd53adaec518fad85de307f689c38e8eab390a7359e142ae3a16`  
		Last Modified: Wed, 12 Apr 2023 01:18:31 GMT  
		Size: 64.5 MB (64510930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd33a842deca9de4a3e249248620b5666ab2fa35cae6fe8b10b79955f955c3e`  
		Last Modified: Wed, 12 Apr 2023 01:18:15 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.11` - linux; s390x

```console
$ docker pull varnish@sha256:91cf8dba2788f88ad8b8f188bb53c43d9b749547de652b93d26493f0c3cac63f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.0 MB (81006609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0df2b025628576f460505157da9b8f5f06d418c21686950786d49f881b8f9b2a`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:01:00 GMT
ADD file:b6463dba97ba9c0a29bacfafc4d67bc603ab57e80b75e23cd42d7ef4b0f8e6ae in / 
# Wed, 12 Apr 2023 00:01:04 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:50:27 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 07:52:14 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 12 Apr 2023 07:52:17 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 07:52:17 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 12 Apr 2023 07:52:17 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 07:52:17 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 07:52:17 GMT
CMD []
```

-	Layers:
	-	`sha256:97fe10bc7def58e7938e97e41eec4788ec7a45b6ef2cb1770cec02fa831fd19d`  
		Last Modified: Wed, 12 Apr 2023 00:05:18 GMT  
		Size: 29.7 MB (29653156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7822e42c3387f3cd91539d4e97252f558b188301244bec6480d7540b6a80882`  
		Last Modified: Wed, 12 Apr 2023 07:53:20 GMT  
		Size: 51.4 MB (51352752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750915994cfaac0ec2feb5390e1d622af471974ba829d7b86d1edf3d6b3beb0d`  
		Last Modified: Wed, 12 Apr 2023 07:53:13 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.2`

```console
$ docker pull varnish@sha256:28b9207d49c4e302fc86546b7d45ea4d9e6b5422cc77cb49f51be275d864b039
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:7.2` - linux; amd64

```console
$ docker pull varnish@sha256:dfb97568859cbd5e3b745a67668df23a1ceca18eb292218d9871d52954805d99
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106849839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e192e3d65e5429e6f2a7f23281c3cf04d43217560b3c01e47dd8654ab470e545`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:39:16 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Wed, 12 Apr 2023 07:39:16 GMT
ARG VARNISH_VERSION=7.2.1
# Wed, 12 Apr 2023 07:39:16 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Wed, 12 Apr 2023 07:39:17 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Wed, 12 Apr 2023 07:39:17 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Wed, 12 Apr 2023 07:39:17 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 07:39:17 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Wed, 12 Apr 2023 07:39:17 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Wed, 12 Apr 2023 07:39:17 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 07:39:17 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 07:39:17 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 07:41:53 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 07:41:54 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 07:41:54 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 07:41:54 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 07:41:54 GMT
USER varnish
# Wed, 12 Apr 2023 07:41:54 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 07:41:54 GMT
CMD []
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c968e0ee4a730130252480debde7124ca86d34f741bf51571a5a29a5ba34693c`  
		Last Modified: Wed, 12 Apr 2023 07:45:05 GMT  
		Size: 75.4 MB (75431120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25daa5e6ca914814a8155ca526ce4bb0b71741603e1898c2e87ec69bd20c5ab0`  
		Last Modified: Wed, 12 Apr 2023 07:44:55 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2` - linux; arm variant v7

```console
$ docker pull varnish@sha256:c244a05033959bcfd06dad6e9bb4c15405ca97412a35d196aa7288a8d0b98865
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.2 MB (83190520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18f4f1a4a71ea168baeb1694ae369389fda214c037ea35ff0165991f0abe556d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 11 Apr 2023 23:59:44 GMT
ADD file:e5f4777456ed4424053e9aa1f3d783f57da094c7a6c6d9d7a2fd315e00b5bbb0 in / 
# Tue, 11 Apr 2023 23:59:44 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 09:52:54 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Wed, 12 Apr 2023 09:52:54 GMT
ARG VARNISH_VERSION=7.2.1
# Wed, 12 Apr 2023 09:52:54 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Wed, 12 Apr 2023 09:52:55 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Wed, 12 Apr 2023 09:52:55 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Wed, 12 Apr 2023 09:52:55 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 09:52:55 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Wed, 12 Apr 2023 09:52:55 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Wed, 12 Apr 2023 09:52:55 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 09:52:55 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 09:52:55 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 09:55:29 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 09:55:29 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 09:55:29 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 09:55:29 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 09:55:29 GMT
USER varnish
# Wed, 12 Apr 2023 09:55:29 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 09:55:29 GMT
CMD []
```

-	Layers:
	-	`sha256:99c2a28b4a43ce341eb611e82106b886315f30a250473617f2293828e10d8fff`  
		Last Modified: Wed, 12 Apr 2023 00:03:19 GMT  
		Size: 26.6 MB (26579772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02c3bf9e9ab14cb00f2a7b32fd61f0dc7f58385c6b36746b7a28d8db143af093`  
		Last Modified: Wed, 12 Apr 2023 09:58:19 GMT  
		Size: 56.6 MB (56610256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3f12a5b2f13f28364d239561b484e09aab0533fa4291c2ec7c6fb72ae6dbe3`  
		Last Modified: Wed, 12 Apr 2023 09:58:10 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:c7c5b44d1b649b8e18f2fa02e3ac6cfbe1219629ee51fb0c297f2ad9d340835c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.9 MB (100869468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:064d1446bbe323f8a5118936bc056bec5669a4efea357a44b0250aefebce979f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 04:48:37 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Wed, 12 Apr 2023 04:48:38 GMT
ARG VARNISH_VERSION=7.2.1
# Wed, 12 Apr 2023 04:48:38 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Wed, 12 Apr 2023 04:48:38 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Wed, 12 Apr 2023 04:48:38 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Wed, 12 Apr 2023 04:48:38 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 04:48:38 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Wed, 12 Apr 2023 04:48:38 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Wed, 12 Apr 2023 04:48:38 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 04:48:38 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 04:48:38 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 04:50:57 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 04:50:57 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 04:50:57 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:50:57 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 04:50:58 GMT
USER varnish
# Wed, 12 Apr 2023 04:50:58 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 04:50:58 GMT
CMD []
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd387399b52bcda6a293afa412dc3c7ffe5106e36f6820bbfe7b36cfe9c84ce6`  
		Last Modified: Wed, 12 Apr 2023 04:53:31 GMT  
		Size: 70.8 MB (70805151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717900fa7e49b8851eb8e3cc5cb7174be8ba02fa5fae4efc1d5889369dc19982`  
		Last Modified: Wed, 12 Apr 2023 04:53:24 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2` - linux; 386

```console
$ docker pull varnish@sha256:132d16358cb9c81ea691480e6340bafa5db22839213c2608eb00bb1c2e318778
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.2 MB (108229812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:701dd3cc6e511fd1e6a0ccb05404b60373851c1f0318dd8035b6526b81707c28`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:39:01 GMT
ADD file:42fc1b4536cdd6823499b0c94d799e9bfbcb280b7df55d8d6c9f6defd61ecb6e in / 
# Wed, 12 Apr 2023 00:39:01 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 04:18:22 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Wed, 12 Apr 2023 04:18:22 GMT
ARG VARNISH_VERSION=7.2.1
# Wed, 12 Apr 2023 04:18:22 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Wed, 12 Apr 2023 04:18:22 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Wed, 12 Apr 2023 04:18:23 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Wed, 12 Apr 2023 04:18:23 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 04:18:23 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Wed, 12 Apr 2023 04:18:23 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Wed, 12 Apr 2023 04:18:23 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 04:18:23 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 04:18:23 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 04:21:46 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 04:21:46 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 04:21:47 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:21:47 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 04:21:47 GMT
USER varnish
# Wed, 12 Apr 2023 04:21:47 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 04:21:47 GMT
CMD []
```

-	Layers:
	-	`sha256:b2ee1f87789d52ef09851b4e5c9745fb8aceafa107b0d3452f9973f1abe65042`  
		Last Modified: Wed, 12 Apr 2023 00:42:45 GMT  
		Size: 32.4 MB (32398925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a639361d9918a14ff82f7bba72feea5809b05f1c6a1c6da01ac194a148379e2`  
		Last Modified: Wed, 12 Apr 2023 04:25:29 GMT  
		Size: 75.8 MB (75830396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e95964f0144157e5774aa830935fc68f7bf5b0a1834e27bc6272d49816484fda`  
		Last Modified: Wed, 12 Apr 2023 04:25:15 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2` - linux; ppc64le

```console
$ docker pull varnish@sha256:2ddbd11558d86d08b3f82a25da574d70734fed468550edb4d6b957cf2fc4ff55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.1 MB (106112382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fcc671da9acaf8ae312a5ba85fd3d77e7e1b88a900054ac23433f6dad4b7cde`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:08:20 GMT
ADD file:63eb52aaff02c15bceabb87a78eb1b36389066ff4774cf8a754160ca7d509816 in / 
# Wed, 12 Apr 2023 00:08:23 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:55:40 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Wed, 12 Apr 2023 00:55:40 GMT
ARG VARNISH_VERSION=7.2.1
# Wed, 12 Apr 2023 00:55:41 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Wed, 12 Apr 2023 00:55:41 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Wed, 12 Apr 2023 00:55:42 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Wed, 12 Apr 2023 00:55:42 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 00:55:43 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Wed, 12 Apr 2023 00:55:44 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Wed, 12 Apr 2023 00:55:44 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 00:55:45 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 00:55:45 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 01:06:37 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 01:06:41 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 01:06:41 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 01:06:42 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 01:06:43 GMT
USER varnish
# Wed, 12 Apr 2023 01:06:43 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 01:06:45 GMT
CMD []
```

-	Layers:
	-	`sha256:5b41d5ec640939cf684959234ad3b80909268a32bfd520a31c6720a91521c2fa`  
		Last Modified: Wed, 12 Apr 2023 00:13:13 GMT  
		Size: 35.3 MB (35291995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4a89d7f741d3117b0ee6c2f7194da63a2eb7e31a212514121c21a0f9a2d56d`  
		Last Modified: Wed, 12 Apr 2023 01:18:03 GMT  
		Size: 70.8 MB (70819898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3fec9bc4ead77e694d7ee941f4809ba1dc75a4379c2e14982a287a907f61d2`  
		Last Modified: Wed, 12 Apr 2023 01:17:46 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2` - linux; s390x

```console
$ docker pull varnish@sha256:8e03fc4febcb1085c13e0d907ca56a70bd0a5015b6001b7575deddb067700889
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.1 MB (87145481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae5308c0a1d01c5120da7ddc51e7161062bf73b4fe635935570d47dce15b4888`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:01:00 GMT
ADD file:b6463dba97ba9c0a29bacfafc4d67bc603ab57e80b75e23cd42d7ef4b0f8e6ae in / 
# Wed, 12 Apr 2023 00:01:04 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:47:32 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Wed, 12 Apr 2023 07:47:32 GMT
ARG VARNISH_VERSION=7.2.1
# Wed, 12 Apr 2023 07:47:32 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Wed, 12 Apr 2023 07:47:32 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Wed, 12 Apr 2023 07:47:32 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Wed, 12 Apr 2023 07:47:32 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 07:47:32 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Wed, 12 Apr 2023 07:47:33 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Wed, 12 Apr 2023 07:47:33 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 07:47:33 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 07:47:33 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 07:50:04 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 07:50:08 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 07:50:08 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 07:50:08 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 07:50:08 GMT
USER varnish
# Wed, 12 Apr 2023 07:50:08 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 07:50:08 GMT
CMD []
```

-	Layers:
	-	`sha256:97fe10bc7def58e7938e97e41eec4788ec7a45b6ef2cb1770cec02fa831fd19d`  
		Last Modified: Wed, 12 Apr 2023 00:05:18 GMT  
		Size: 29.7 MB (29653156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6c0378159be2b47ba02173837a0605e110437dd56ebde55c1b33b16e3a64c1`  
		Last Modified: Wed, 12 Apr 2023 07:53:06 GMT  
		Size: 57.5 MB (57491834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b0aa3c751db4a00420dc9624ea76c92014f9ff8e7975d01d47e5bf3743531c`  
		Last Modified: Wed, 12 Apr 2023 07:52:59 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.2-alpine`

```console
$ docker pull varnish@sha256:4afc17b0aa7c483b822ae0c548f93d87fdcfc38715e30734657bad8a3171f534
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:7.2-alpine` - linux; amd64

```console
$ docker pull varnish@sha256:a320ad063c3556dfea1308e7747a7b74de2e6580bb136653f10480b192d2b7ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.4 MB (59399546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:619a779899e4b887658162b42b9f51b181570836a20e93eabacd1c0634421c23`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:16:18 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 30 Mar 2023 02:16:18 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 30 Mar 2023 02:16:18 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 30 Mar 2023 02:16:19 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 30 Mar 2023 02:16:19 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 30 Mar 2023 02:16:19 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 02:16:19 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 30 Mar 2023 02:16:19 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 30 Mar 2023 02:16:19 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 02:16:19 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 02:16:19 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 02:17:35 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 02:17:35 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 02:17:35 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 02:17:35 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 02:17:35 GMT
USER varnish
# Thu, 30 Mar 2023 02:17:35 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 02:17:36 GMT
CMD []
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c114fe4204a2c955105dd5cd8a42a772594a1642947fbefba511406b0e60e5`  
		Last Modified: Thu, 30 Mar 2023 02:18:20 GMT  
		Size: 56.6 MB (56572454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debea196e0761731bed241b5b0124d7dab6070192ebf9f49532117ef228a4fd7`  
		Last Modified: Thu, 30 Mar 2023 02:18:13 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:fccf7f20e1622e5cc7de9c8a0374d530f4ce08e15bae3fa806e6c5f34100a250
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45148202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31ac3c9362d31494b1482831d5f9600db9a9423084b5bcdfb6bf502d29be4134`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 18:05:06 GMT
ADD file:0516b2e2d8a5c0a3e85e67a20375312bdc586a63094d779b9ac92517cf74a19d in / 
# Wed, 29 Mar 2023 18:05:06 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:16:02 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 30 Mar 2023 00:16:02 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 30 Mar 2023 00:16:02 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 30 Mar 2023 00:16:02 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 30 Mar 2023 00:16:02 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 30 Mar 2023 00:16:02 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 00:16:02 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 30 Mar 2023 00:16:03 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 30 Mar 2023 00:16:03 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 00:16:03 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 00:16:03 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 00:17:15 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 00:17:16 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 00:17:16 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 00:17:16 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 00:17:16 GMT
USER varnish
# Thu, 30 Mar 2023 00:17:16 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 00:17:16 GMT
CMD []
```

-	Layers:
	-	`sha256:fafb00bc68cf26e4a27ad2dce7303945ba9e40994e77c9269e610e0452ae9dce`  
		Last Modified: Wed, 29 Mar 2023 18:07:17 GMT  
		Size: 2.4 MB (2437606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7ec1086689ab0fd73293e70d501d454a27eb5ea261d03a2430cb0d14696427`  
		Last Modified: Sat, 08 Apr 2023 02:41:03 GMT  
		Size: 42.7 MB (42710102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9ac18a355d90f33336fbada96e19569338d541feae42ae2d313ce006609bb1`  
		Last Modified: Sat, 08 Apr 2023 02:40:57 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:4b01c566b91d765af9c55ca58772d6926b481ba4c60bfe7b9d6b0adca255f10b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52139702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3552cf8b859208887e19e7d4ff64ae304e14cf411f5dadeb80d6c52b607f72d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:55:19 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 30 Mar 2023 05:55:20 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 30 Mar 2023 05:55:20 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 30 Mar 2023 05:55:20 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 30 Mar 2023 05:55:20 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 30 Mar 2023 05:55:20 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 05:55:20 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 30 Mar 2023 05:55:20 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 30 Mar 2023 05:55:20 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 05:55:20 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 05:55:20 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 05:56:25 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 05:56:25 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 05:56:25 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 05:56:26 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 05:56:26 GMT
USER varnish
# Thu, 30 Mar 2023 05:56:26 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 05:56:26 GMT
CMD []
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c53d05c94805192159ec306400f8402f101647b10b4f2862a4b9cafe6d9ea95`  
		Last Modified: Thu, 30 Mar 2023 05:57:04 GMT  
		Size: 49.4 MB (49417204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dfbbc1899969f2944b32d817962c27670200b641a7ff5b382026a2a6f1e91f8`  
		Last Modified: Thu, 30 Mar 2023 05:56:58 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2-alpine` - linux; 386

```console
$ docker pull varnish@sha256:b4aed57dfb69759cbbf97f8251f733ed209e5377c0b138e878768446cf3f1012
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.6 MB (59579474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb2d5054f0237342f09e7c81d57f5b91b2a7258c98c54862bcd60b70f213eff4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 17:38:36 GMT
ADD file:fca96dde137b6b045359aec9d24257996738ac6cb7cce9518460a66802a27bd7 in / 
# Wed, 29 Mar 2023 17:38:36 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 01:36:10 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 30 Mar 2023 01:36:10 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 30 Mar 2023 01:36:10 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 30 Mar 2023 01:36:10 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 30 Mar 2023 01:36:10 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 30 Mar 2023 01:36:10 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 01:36:10 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 30 Mar 2023 01:36:10 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 30 Mar 2023 01:36:11 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 01:36:11 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 01:36:11 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 01:38:03 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 01:38:03 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 01:38:03 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 01:38:03 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 01:38:03 GMT
USER varnish
# Thu, 30 Mar 2023 01:38:04 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 01:38:04 GMT
CMD []
```

-	Layers:
	-	`sha256:333f5f619d7efe58316b2d71276f19d0a59bcb471f4dadaa85762b2c9e02775c`  
		Last Modified: Wed, 29 Mar 2023 17:39:19 GMT  
		Size: 2.8 MB (2832576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec17ca4c36e5d196286fcd4f66f0a6879ff35841617edc48c24a2b0d3fed6c5`  
		Last Modified: Thu, 30 Mar 2023 01:39:02 GMT  
		Size: 56.7 MB (56746401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3acb1c0b2cc2ca1f40568c89f6ace8d204192474b0b299f6afbd1d5b87c89ad4`  
		Last Modified: Thu, 30 Mar 2023 01:38:52 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:47175a4b9a3d7cc10400bda61c20d308651152bf93f3268aa3b4c850c4cebb3c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49172829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe520b41ef8593a0ca87c4b15e445248e7728729026968d7c7167a33b40a8e28`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 18:16:40 GMT
ADD file:3c2a8d553fa0998f13f86592f104a9a4ad14f8db46dfa9145c8fbbca0b87ee9a in / 
# Wed, 29 Mar 2023 18:16:40 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:35:48 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 30 Mar 2023 04:35:48 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 30 Mar 2023 04:35:49 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 30 Mar 2023 04:35:49 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 30 Mar 2023 04:35:49 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 30 Mar 2023 04:35:50 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 04:35:50 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 30 Mar 2023 04:35:50 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 30 Mar 2023 04:35:51 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 04:35:51 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 04:35:51 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 04:37:42 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 04:37:43 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 04:37:44 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 04:37:44 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 04:37:44 GMT
USER varnish
# Thu, 30 Mar 2023 04:37:45 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 04:37:45 GMT
CMD []
```

-	Layers:
	-	`sha256:0b40b0bd0da3095d93bf74233a1d0bf638b2511fee461df8f6a71aad5a038589`  
		Last Modified: Wed, 29 Mar 2023 18:17:38 GMT  
		Size: 2.8 MB (2813760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69361e01f667423c0f2d961984f6e7db1a81226574e2f2e13b25de56a1ed714d`  
		Last Modified: Thu, 30 Mar 2023 04:38:48 GMT  
		Size: 46.4 MB (46358574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b033b092d98a898fd606406859a2bdc093c0babde613a26ed82fff5736c9290`  
		Last Modified: Thu, 30 Mar 2023 04:38:37 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:cae32a9f29cd9997a1fe2ee6f8d0b8e3ff91c21e6213716d9ac34675317dc70d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47646967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e24f77bba538e7715318a014e47a2ab4183cd521c07f85ecc3a82ab13ed2830`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 17:42:07 GMT
ADD file:5cf392863cd9a0735de88f9e7dab93c9e74aca59ca05b792943cf3b621ea2c59 in / 
# Wed, 29 Mar 2023 17:42:07 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 23:10:06 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Wed, 29 Mar 2023 23:10:06 GMT
ARG VARNISH_VERSION=7.2.1
# Wed, 29 Mar 2023 23:10:06 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Wed, 29 Mar 2023 23:10:06 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Wed, 29 Mar 2023 23:10:06 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Wed, 29 Mar 2023 23:10:06 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 29 Mar 2023 23:10:06 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Wed, 29 Mar 2023 23:10:06 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Wed, 29 Mar 2023 23:10:07 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 29 Mar 2023 23:10:07 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Wed, 29 Mar 2023 23:10:07 GMT
ENV VARNISH_SIZE=100M
# Wed, 29 Mar 2023 23:11:26 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Wed, 29 Mar 2023 23:11:28 GMT
WORKDIR /etc/varnish
# Wed, 29 Mar 2023 23:11:28 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 29 Mar 2023 23:11:28 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 29 Mar 2023 23:11:28 GMT
USER varnish
# Wed, 29 Mar 2023 23:11:28 GMT
EXPOSE 80 8443
# Wed, 29 Mar 2023 23:11:28 GMT
CMD []
```

-	Layers:
	-	`sha256:1536575ac9c5f5fff4522c60d4610af0a52be584c36e652080c6c0ad169d4f27`  
		Last Modified: Wed, 29 Mar 2023 17:42:42 GMT  
		Size: 2.6 MB (2610636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091447cbd58b57bbe1eb2edf62b5e2d9c06467104aebfc70c02d7cfafa01868c`  
		Last Modified: Wed, 29 Mar 2023 23:12:17 GMT  
		Size: 45.0 MB (45035834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390574d541f53e2036c226ec79255c18a2429053de04847092de875c4925890b`  
		Last Modified: Wed, 29 Mar 2023 23:12:12 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.2.1`

```console
$ docker pull varnish@sha256:28b9207d49c4e302fc86546b7d45ea4d9e6b5422cc77cb49f51be275d864b039
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:7.2.1` - linux; amd64

```console
$ docker pull varnish@sha256:dfb97568859cbd5e3b745a67668df23a1ceca18eb292218d9871d52954805d99
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106849839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e192e3d65e5429e6f2a7f23281c3cf04d43217560b3c01e47dd8654ab470e545`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:39:16 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Wed, 12 Apr 2023 07:39:16 GMT
ARG VARNISH_VERSION=7.2.1
# Wed, 12 Apr 2023 07:39:16 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Wed, 12 Apr 2023 07:39:17 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Wed, 12 Apr 2023 07:39:17 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Wed, 12 Apr 2023 07:39:17 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 07:39:17 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Wed, 12 Apr 2023 07:39:17 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Wed, 12 Apr 2023 07:39:17 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 07:39:17 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 07:39:17 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 07:41:53 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 07:41:54 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 07:41:54 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 07:41:54 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 07:41:54 GMT
USER varnish
# Wed, 12 Apr 2023 07:41:54 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 07:41:54 GMT
CMD []
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c968e0ee4a730130252480debde7124ca86d34f741bf51571a5a29a5ba34693c`  
		Last Modified: Wed, 12 Apr 2023 07:45:05 GMT  
		Size: 75.4 MB (75431120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25daa5e6ca914814a8155ca526ce4bb0b71741603e1898c2e87ec69bd20c5ab0`  
		Last Modified: Wed, 12 Apr 2023 07:44:55 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2.1` - linux; arm variant v7

```console
$ docker pull varnish@sha256:c244a05033959bcfd06dad6e9bb4c15405ca97412a35d196aa7288a8d0b98865
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.2 MB (83190520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18f4f1a4a71ea168baeb1694ae369389fda214c037ea35ff0165991f0abe556d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 11 Apr 2023 23:59:44 GMT
ADD file:e5f4777456ed4424053e9aa1f3d783f57da094c7a6c6d9d7a2fd315e00b5bbb0 in / 
# Tue, 11 Apr 2023 23:59:44 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 09:52:54 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Wed, 12 Apr 2023 09:52:54 GMT
ARG VARNISH_VERSION=7.2.1
# Wed, 12 Apr 2023 09:52:54 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Wed, 12 Apr 2023 09:52:55 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Wed, 12 Apr 2023 09:52:55 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Wed, 12 Apr 2023 09:52:55 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 09:52:55 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Wed, 12 Apr 2023 09:52:55 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Wed, 12 Apr 2023 09:52:55 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 09:52:55 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 09:52:55 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 09:55:29 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 09:55:29 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 09:55:29 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 09:55:29 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 09:55:29 GMT
USER varnish
# Wed, 12 Apr 2023 09:55:29 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 09:55:29 GMT
CMD []
```

-	Layers:
	-	`sha256:99c2a28b4a43ce341eb611e82106b886315f30a250473617f2293828e10d8fff`  
		Last Modified: Wed, 12 Apr 2023 00:03:19 GMT  
		Size: 26.6 MB (26579772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02c3bf9e9ab14cb00f2a7b32fd61f0dc7f58385c6b36746b7a28d8db143af093`  
		Last Modified: Wed, 12 Apr 2023 09:58:19 GMT  
		Size: 56.6 MB (56610256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3f12a5b2f13f28364d239561b484e09aab0533fa4291c2ec7c6fb72ae6dbe3`  
		Last Modified: Wed, 12 Apr 2023 09:58:10 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2.1` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:c7c5b44d1b649b8e18f2fa02e3ac6cfbe1219629ee51fb0c297f2ad9d340835c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.9 MB (100869468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:064d1446bbe323f8a5118936bc056bec5669a4efea357a44b0250aefebce979f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 04:48:37 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Wed, 12 Apr 2023 04:48:38 GMT
ARG VARNISH_VERSION=7.2.1
# Wed, 12 Apr 2023 04:48:38 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Wed, 12 Apr 2023 04:48:38 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Wed, 12 Apr 2023 04:48:38 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Wed, 12 Apr 2023 04:48:38 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 04:48:38 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Wed, 12 Apr 2023 04:48:38 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Wed, 12 Apr 2023 04:48:38 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 04:48:38 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 04:48:38 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 04:50:57 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 04:50:57 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 04:50:57 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:50:57 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 04:50:58 GMT
USER varnish
# Wed, 12 Apr 2023 04:50:58 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 04:50:58 GMT
CMD []
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd387399b52bcda6a293afa412dc3c7ffe5106e36f6820bbfe7b36cfe9c84ce6`  
		Last Modified: Wed, 12 Apr 2023 04:53:31 GMT  
		Size: 70.8 MB (70805151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717900fa7e49b8851eb8e3cc5cb7174be8ba02fa5fae4efc1d5889369dc19982`  
		Last Modified: Wed, 12 Apr 2023 04:53:24 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2.1` - linux; 386

```console
$ docker pull varnish@sha256:132d16358cb9c81ea691480e6340bafa5db22839213c2608eb00bb1c2e318778
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.2 MB (108229812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:701dd3cc6e511fd1e6a0ccb05404b60373851c1f0318dd8035b6526b81707c28`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:39:01 GMT
ADD file:42fc1b4536cdd6823499b0c94d799e9bfbcb280b7df55d8d6c9f6defd61ecb6e in / 
# Wed, 12 Apr 2023 00:39:01 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 04:18:22 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Wed, 12 Apr 2023 04:18:22 GMT
ARG VARNISH_VERSION=7.2.1
# Wed, 12 Apr 2023 04:18:22 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Wed, 12 Apr 2023 04:18:22 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Wed, 12 Apr 2023 04:18:23 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Wed, 12 Apr 2023 04:18:23 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 04:18:23 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Wed, 12 Apr 2023 04:18:23 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Wed, 12 Apr 2023 04:18:23 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 04:18:23 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 04:18:23 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 04:21:46 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 04:21:46 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 04:21:47 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:21:47 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 04:21:47 GMT
USER varnish
# Wed, 12 Apr 2023 04:21:47 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 04:21:47 GMT
CMD []
```

-	Layers:
	-	`sha256:b2ee1f87789d52ef09851b4e5c9745fb8aceafa107b0d3452f9973f1abe65042`  
		Last Modified: Wed, 12 Apr 2023 00:42:45 GMT  
		Size: 32.4 MB (32398925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a639361d9918a14ff82f7bba72feea5809b05f1c6a1c6da01ac194a148379e2`  
		Last Modified: Wed, 12 Apr 2023 04:25:29 GMT  
		Size: 75.8 MB (75830396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e95964f0144157e5774aa830935fc68f7bf5b0a1834e27bc6272d49816484fda`  
		Last Modified: Wed, 12 Apr 2023 04:25:15 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2.1` - linux; ppc64le

```console
$ docker pull varnish@sha256:2ddbd11558d86d08b3f82a25da574d70734fed468550edb4d6b957cf2fc4ff55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.1 MB (106112382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fcc671da9acaf8ae312a5ba85fd3d77e7e1b88a900054ac23433f6dad4b7cde`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:08:20 GMT
ADD file:63eb52aaff02c15bceabb87a78eb1b36389066ff4774cf8a754160ca7d509816 in / 
# Wed, 12 Apr 2023 00:08:23 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:55:40 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Wed, 12 Apr 2023 00:55:40 GMT
ARG VARNISH_VERSION=7.2.1
# Wed, 12 Apr 2023 00:55:41 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Wed, 12 Apr 2023 00:55:41 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Wed, 12 Apr 2023 00:55:42 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Wed, 12 Apr 2023 00:55:42 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 00:55:43 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Wed, 12 Apr 2023 00:55:44 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Wed, 12 Apr 2023 00:55:44 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 00:55:45 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 00:55:45 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 01:06:37 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 01:06:41 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 01:06:41 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 01:06:42 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 01:06:43 GMT
USER varnish
# Wed, 12 Apr 2023 01:06:43 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 01:06:45 GMT
CMD []
```

-	Layers:
	-	`sha256:5b41d5ec640939cf684959234ad3b80909268a32bfd520a31c6720a91521c2fa`  
		Last Modified: Wed, 12 Apr 2023 00:13:13 GMT  
		Size: 35.3 MB (35291995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4a89d7f741d3117b0ee6c2f7194da63a2eb7e31a212514121c21a0f9a2d56d`  
		Last Modified: Wed, 12 Apr 2023 01:18:03 GMT  
		Size: 70.8 MB (70819898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3fec9bc4ead77e694d7ee941f4809ba1dc75a4379c2e14982a287a907f61d2`  
		Last Modified: Wed, 12 Apr 2023 01:17:46 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2.1` - linux; s390x

```console
$ docker pull varnish@sha256:8e03fc4febcb1085c13e0d907ca56a70bd0a5015b6001b7575deddb067700889
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.1 MB (87145481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae5308c0a1d01c5120da7ddc51e7161062bf73b4fe635935570d47dce15b4888`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:01:00 GMT
ADD file:b6463dba97ba9c0a29bacfafc4d67bc603ab57e80b75e23cd42d7ef4b0f8e6ae in / 
# Wed, 12 Apr 2023 00:01:04 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:47:32 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Wed, 12 Apr 2023 07:47:32 GMT
ARG VARNISH_VERSION=7.2.1
# Wed, 12 Apr 2023 07:47:32 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Wed, 12 Apr 2023 07:47:32 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Wed, 12 Apr 2023 07:47:32 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Wed, 12 Apr 2023 07:47:32 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 07:47:32 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Wed, 12 Apr 2023 07:47:33 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Wed, 12 Apr 2023 07:47:33 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 07:47:33 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 07:47:33 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 07:50:04 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 07:50:08 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 07:50:08 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 07:50:08 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 07:50:08 GMT
USER varnish
# Wed, 12 Apr 2023 07:50:08 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 07:50:08 GMT
CMD []
```

-	Layers:
	-	`sha256:97fe10bc7def58e7938e97e41eec4788ec7a45b6ef2cb1770cec02fa831fd19d`  
		Last Modified: Wed, 12 Apr 2023 00:05:18 GMT  
		Size: 29.7 MB (29653156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6c0378159be2b47ba02173837a0605e110437dd56ebde55c1b33b16e3a64c1`  
		Last Modified: Wed, 12 Apr 2023 07:53:06 GMT  
		Size: 57.5 MB (57491834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b0aa3c751db4a00420dc9624ea76c92014f9ff8e7975d01d47e5bf3743531c`  
		Last Modified: Wed, 12 Apr 2023 07:52:59 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.2.1-alpine`

```console
$ docker pull varnish@sha256:4afc17b0aa7c483b822ae0c548f93d87fdcfc38715e30734657bad8a3171f534
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:7.2.1-alpine` - linux; amd64

```console
$ docker pull varnish@sha256:a320ad063c3556dfea1308e7747a7b74de2e6580bb136653f10480b192d2b7ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.4 MB (59399546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:619a779899e4b887658162b42b9f51b181570836a20e93eabacd1c0634421c23`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:16:18 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 30 Mar 2023 02:16:18 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 30 Mar 2023 02:16:18 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 30 Mar 2023 02:16:19 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 30 Mar 2023 02:16:19 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 30 Mar 2023 02:16:19 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 02:16:19 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 30 Mar 2023 02:16:19 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 30 Mar 2023 02:16:19 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 02:16:19 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 02:16:19 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 02:17:35 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 02:17:35 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 02:17:35 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 02:17:35 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 02:17:35 GMT
USER varnish
# Thu, 30 Mar 2023 02:17:35 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 02:17:36 GMT
CMD []
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c114fe4204a2c955105dd5cd8a42a772594a1642947fbefba511406b0e60e5`  
		Last Modified: Thu, 30 Mar 2023 02:18:20 GMT  
		Size: 56.6 MB (56572454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debea196e0761731bed241b5b0124d7dab6070192ebf9f49532117ef228a4fd7`  
		Last Modified: Thu, 30 Mar 2023 02:18:13 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2.1-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:fccf7f20e1622e5cc7de9c8a0374d530f4ce08e15bae3fa806e6c5f34100a250
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45148202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31ac3c9362d31494b1482831d5f9600db9a9423084b5bcdfb6bf502d29be4134`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 18:05:06 GMT
ADD file:0516b2e2d8a5c0a3e85e67a20375312bdc586a63094d779b9ac92517cf74a19d in / 
# Wed, 29 Mar 2023 18:05:06 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:16:02 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 30 Mar 2023 00:16:02 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 30 Mar 2023 00:16:02 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 30 Mar 2023 00:16:02 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 30 Mar 2023 00:16:02 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 30 Mar 2023 00:16:02 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 00:16:02 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 30 Mar 2023 00:16:03 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 30 Mar 2023 00:16:03 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 00:16:03 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 00:16:03 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 00:17:15 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 00:17:16 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 00:17:16 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 00:17:16 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 00:17:16 GMT
USER varnish
# Thu, 30 Mar 2023 00:17:16 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 00:17:16 GMT
CMD []
```

-	Layers:
	-	`sha256:fafb00bc68cf26e4a27ad2dce7303945ba9e40994e77c9269e610e0452ae9dce`  
		Last Modified: Wed, 29 Mar 2023 18:07:17 GMT  
		Size: 2.4 MB (2437606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7ec1086689ab0fd73293e70d501d454a27eb5ea261d03a2430cb0d14696427`  
		Last Modified: Sat, 08 Apr 2023 02:41:03 GMT  
		Size: 42.7 MB (42710102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9ac18a355d90f33336fbada96e19569338d541feae42ae2d313ce006609bb1`  
		Last Modified: Sat, 08 Apr 2023 02:40:57 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2.1-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:4b01c566b91d765af9c55ca58772d6926b481ba4c60bfe7b9d6b0adca255f10b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52139702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3552cf8b859208887e19e7d4ff64ae304e14cf411f5dadeb80d6c52b607f72d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:55:19 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 30 Mar 2023 05:55:20 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 30 Mar 2023 05:55:20 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 30 Mar 2023 05:55:20 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 30 Mar 2023 05:55:20 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 30 Mar 2023 05:55:20 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 05:55:20 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 30 Mar 2023 05:55:20 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 30 Mar 2023 05:55:20 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 05:55:20 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 05:55:20 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 05:56:25 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 05:56:25 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 05:56:25 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 05:56:26 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 05:56:26 GMT
USER varnish
# Thu, 30 Mar 2023 05:56:26 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 05:56:26 GMT
CMD []
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c53d05c94805192159ec306400f8402f101647b10b4f2862a4b9cafe6d9ea95`  
		Last Modified: Thu, 30 Mar 2023 05:57:04 GMT  
		Size: 49.4 MB (49417204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dfbbc1899969f2944b32d817962c27670200b641a7ff5b382026a2a6f1e91f8`  
		Last Modified: Thu, 30 Mar 2023 05:56:58 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2.1-alpine` - linux; 386

```console
$ docker pull varnish@sha256:b4aed57dfb69759cbbf97f8251f733ed209e5377c0b138e878768446cf3f1012
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.6 MB (59579474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb2d5054f0237342f09e7c81d57f5b91b2a7258c98c54862bcd60b70f213eff4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 17:38:36 GMT
ADD file:fca96dde137b6b045359aec9d24257996738ac6cb7cce9518460a66802a27bd7 in / 
# Wed, 29 Mar 2023 17:38:36 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 01:36:10 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 30 Mar 2023 01:36:10 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 30 Mar 2023 01:36:10 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 30 Mar 2023 01:36:10 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 30 Mar 2023 01:36:10 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 30 Mar 2023 01:36:10 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 01:36:10 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 30 Mar 2023 01:36:10 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 30 Mar 2023 01:36:11 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 01:36:11 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 01:36:11 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 01:38:03 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 01:38:03 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 01:38:03 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 01:38:03 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 01:38:03 GMT
USER varnish
# Thu, 30 Mar 2023 01:38:04 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 01:38:04 GMT
CMD []
```

-	Layers:
	-	`sha256:333f5f619d7efe58316b2d71276f19d0a59bcb471f4dadaa85762b2c9e02775c`  
		Last Modified: Wed, 29 Mar 2023 17:39:19 GMT  
		Size: 2.8 MB (2832576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec17ca4c36e5d196286fcd4f66f0a6879ff35841617edc48c24a2b0d3fed6c5`  
		Last Modified: Thu, 30 Mar 2023 01:39:02 GMT  
		Size: 56.7 MB (56746401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3acb1c0b2cc2ca1f40568c89f6ace8d204192474b0b299f6afbd1d5b87c89ad4`  
		Last Modified: Thu, 30 Mar 2023 01:38:52 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2.1-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:47175a4b9a3d7cc10400bda61c20d308651152bf93f3268aa3b4c850c4cebb3c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49172829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe520b41ef8593a0ca87c4b15e445248e7728729026968d7c7167a33b40a8e28`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 18:16:40 GMT
ADD file:3c2a8d553fa0998f13f86592f104a9a4ad14f8db46dfa9145c8fbbca0b87ee9a in / 
# Wed, 29 Mar 2023 18:16:40 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:35:48 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 30 Mar 2023 04:35:48 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 30 Mar 2023 04:35:49 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 30 Mar 2023 04:35:49 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 30 Mar 2023 04:35:49 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 30 Mar 2023 04:35:50 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 04:35:50 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 30 Mar 2023 04:35:50 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 30 Mar 2023 04:35:51 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 04:35:51 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 04:35:51 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 04:37:42 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 04:37:43 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 04:37:44 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 04:37:44 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 04:37:44 GMT
USER varnish
# Thu, 30 Mar 2023 04:37:45 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 04:37:45 GMT
CMD []
```

-	Layers:
	-	`sha256:0b40b0bd0da3095d93bf74233a1d0bf638b2511fee461df8f6a71aad5a038589`  
		Last Modified: Wed, 29 Mar 2023 18:17:38 GMT  
		Size: 2.8 MB (2813760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69361e01f667423c0f2d961984f6e7db1a81226574e2f2e13b25de56a1ed714d`  
		Last Modified: Thu, 30 Mar 2023 04:38:48 GMT  
		Size: 46.4 MB (46358574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b033b092d98a898fd606406859a2bdc093c0babde613a26ed82fff5736c9290`  
		Last Modified: Thu, 30 Mar 2023 04:38:37 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2.1-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:cae32a9f29cd9997a1fe2ee6f8d0b8e3ff91c21e6213716d9ac34675317dc70d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47646967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e24f77bba538e7715318a014e47a2ab4183cd521c07f85ecc3a82ab13ed2830`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 17:42:07 GMT
ADD file:5cf392863cd9a0735de88f9e7dab93c9e74aca59ca05b792943cf3b621ea2c59 in / 
# Wed, 29 Mar 2023 17:42:07 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 23:10:06 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Wed, 29 Mar 2023 23:10:06 GMT
ARG VARNISH_VERSION=7.2.1
# Wed, 29 Mar 2023 23:10:06 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Wed, 29 Mar 2023 23:10:06 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Wed, 29 Mar 2023 23:10:06 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Wed, 29 Mar 2023 23:10:06 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 29 Mar 2023 23:10:06 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Wed, 29 Mar 2023 23:10:06 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Wed, 29 Mar 2023 23:10:07 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 29 Mar 2023 23:10:07 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Wed, 29 Mar 2023 23:10:07 GMT
ENV VARNISH_SIZE=100M
# Wed, 29 Mar 2023 23:11:26 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Wed, 29 Mar 2023 23:11:28 GMT
WORKDIR /etc/varnish
# Wed, 29 Mar 2023 23:11:28 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 29 Mar 2023 23:11:28 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 29 Mar 2023 23:11:28 GMT
USER varnish
# Wed, 29 Mar 2023 23:11:28 GMT
EXPOSE 80 8443
# Wed, 29 Mar 2023 23:11:28 GMT
CMD []
```

-	Layers:
	-	`sha256:1536575ac9c5f5fff4522c60d4610af0a52be584c36e652080c6c0ad169d4f27`  
		Last Modified: Wed, 29 Mar 2023 17:42:42 GMT  
		Size: 2.6 MB (2610636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091447cbd58b57bbe1eb2edf62b5e2d9c06467104aebfc70c02d7cfafa01868c`  
		Last Modified: Wed, 29 Mar 2023 23:12:17 GMT  
		Size: 45.0 MB (45035834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390574d541f53e2036c226ec79255c18a2429053de04847092de875c4925890b`  
		Last Modified: Wed, 29 Mar 2023 23:12:12 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.3`

```console
$ docker pull varnish@sha256:d50f601a76ff2cefca6afa7587c75dc46ad482b7734baab89eaf79a6516c90f4
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
$ docker pull varnish@sha256:01c1f0ee2a532a0f480fa00e8b754c2a1662ab5989e3958d966222ed09f95d02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106805687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38f8fe02f4ba954dfed4760af3cb20e716fb19e427144a743bb942eca093bd75`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:35:52 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 12 Apr 2023 07:35:52 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 12 Apr 2023 07:35:52 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 12 Apr 2023 07:35:52 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 12 Apr 2023 07:35:52 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 12 Apr 2023 07:35:52 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 07:35:52 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 12 Apr 2023 07:35:52 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 12 Apr 2023 07:35:52 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 07:35:52 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 07:35:53 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 07:38:58 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 07:38:58 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 07:38:59 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 07:38:59 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 07:38:59 GMT
USER varnish
# Wed, 12 Apr 2023 07:38:59 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 07:38:59 GMT
CMD []
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c1be847abb1fb38853dbae20352d1f2e2b780db54e88fbb737549a5aab7a79`  
		Last Modified: Wed, 12 Apr 2023 07:44:41 GMT  
		Size: 75.4 MB (75386967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb31db21e143ba8b279a4dc67a859edafd358e53f1efdbe4ac92744d507f6ddd`  
		Last Modified: Wed, 12 Apr 2023 07:44:32 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3` - linux; arm variant v7

```console
$ docker pull varnish@sha256:ee2c275680aed583fea7ceba04074e69fda8c8747dbd68766d2e0d9c55512f03
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.1 MB (83149297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7730d361798ab6943823a20c73d9f1bee65ccfe1300978e219422823cbce78b9`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 11 Apr 2023 23:59:44 GMT
ADD file:e5f4777456ed4424053e9aa1f3d783f57da094c7a6c6d9d7a2fd315e00b5bbb0 in / 
# Tue, 11 Apr 2023 23:59:44 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 09:48:46 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 12 Apr 2023 09:48:47 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 12 Apr 2023 09:48:47 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 12 Apr 2023 09:48:47 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 12 Apr 2023 09:48:47 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 12 Apr 2023 09:48:48 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 09:48:48 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 12 Apr 2023 09:48:48 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 12 Apr 2023 09:48:48 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 09:48:49 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 09:48:49 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 09:52:44 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 09:52:44 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 09:52:44 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 09:52:45 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 09:52:45 GMT
USER varnish
# Wed, 12 Apr 2023 09:52:45 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 09:52:45 GMT
CMD []
```

-	Layers:
	-	`sha256:99c2a28b4a43ce341eb611e82106b886315f30a250473617f2293828e10d8fff`  
		Last Modified: Wed, 12 Apr 2023 00:03:19 GMT  
		Size: 26.6 MB (26579772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:946f48177dd61e98fafd1f5db674994ba0ad766c7b50f4b06c552e129d2be463`  
		Last Modified: Wed, 12 Apr 2023 09:57:58 GMT  
		Size: 56.6 MB (56569036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c94d0d1168a78363c629071b130cf202012a5c2285cff907fbe05f9f7d3166e2`  
		Last Modified: Wed, 12 Apr 2023 09:57:50 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:02ef5b0996ff812c54abd99265f8b339cd393d1be211f3cc646f918ffd4bea02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100589822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:036a0598d94c3d082574590889afad8344a4b710a2705cc884c821afd482967e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 04:45:29 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 12 Apr 2023 04:45:29 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 12 Apr 2023 04:45:29 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 12 Apr 2023 04:45:29 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 12 Apr 2023 04:45:29 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 12 Apr 2023 04:45:29 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 04:45:29 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 12 Apr 2023 04:45:29 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 12 Apr 2023 04:45:30 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 04:45:30 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 04:45:30 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 04:48:22 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 04:48:23 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 04:48:23 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:48:23 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 04:48:23 GMT
USER varnish
# Wed, 12 Apr 2023 04:48:23 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 04:48:23 GMT
CMD []
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b6030c7f52818939f055e2f6663b1b9cc13fd7547b1c2e0f753f5b87cd93ca`  
		Last Modified: Wed, 12 Apr 2023 04:53:10 GMT  
		Size: 70.5 MB (70525505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74565242087dac611bbba86cb8a4ef8aa9aa3712f40e4ab8949602813f427c6b`  
		Last Modified: Wed, 12 Apr 2023 04:53:03 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3` - linux; 386

```console
$ docker pull varnish@sha256:88f2d7b6250c7d29544a99d128dc2aafe14c362633b4ff697b2720611c261141
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.2 MB (108173601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bfc3f953767b14e681b22c82c947846dedc22c394cd082cea401378516935b4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:39:01 GMT
ADD file:42fc1b4536cdd6823499b0c94d799e9bfbcb280b7df55d8d6c9f6defd61ecb6e in / 
# Wed, 12 Apr 2023 00:39:01 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 04:13:43 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 12 Apr 2023 04:13:44 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 12 Apr 2023 04:13:44 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 12 Apr 2023 04:13:44 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 12 Apr 2023 04:13:44 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 12 Apr 2023 04:13:44 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 04:13:44 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 12 Apr 2023 04:13:44 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 12 Apr 2023 04:13:44 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 04:13:44 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 04:13:44 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 04:18:07 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 04:18:08 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 04:18:08 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:18:08 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 04:18:08 GMT
USER varnish
# Wed, 12 Apr 2023 04:18:08 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 04:18:08 GMT
CMD []
```

-	Layers:
	-	`sha256:b2ee1f87789d52ef09851b4e5c9745fb8aceafa107b0d3452f9973f1abe65042`  
		Last Modified: Wed, 12 Apr 2023 00:42:45 GMT  
		Size: 32.4 MB (32398925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee5e7f863a0627e32c4308f8e477d218c74b26149178e5f23057f2339a55e64`  
		Last Modified: Wed, 12 Apr 2023 04:25:03 GMT  
		Size: 75.8 MB (75774186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c73471ce047c640427aa8d168e423ce9d464179d283e9ecc90c6dca784deef`  
		Last Modified: Wed, 12 Apr 2023 04:24:49 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3` - linux; ppc64le

```console
$ docker pull varnish@sha256:99a9dcf0cddca561abbcd5bc5b002adbb083de964d8746e3063cab564573c331
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.1 MB (106076410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e817121269101ae25eb3c824355809f156a4e72be8a908710817a5575d2fb848`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:08:20 GMT
ADD file:63eb52aaff02c15bceabb87a78eb1b36389066ff4774cf8a754160ca7d509816 in / 
# Wed, 12 Apr 2023 00:08:23 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:43:55 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 12 Apr 2023 00:43:56 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 12 Apr 2023 00:43:56 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 12 Apr 2023 00:43:57 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 12 Apr 2023 00:43:57 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 12 Apr 2023 00:43:58 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 00:43:58 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 12 Apr 2023 00:43:59 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 12 Apr 2023 00:43:59 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 00:44:00 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 00:44:00 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 00:55:22 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 00:55:26 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 00:55:26 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 00:55:27 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 00:55:28 GMT
USER varnish
# Wed, 12 Apr 2023 00:55:28 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 00:55:29 GMT
CMD []
```

-	Layers:
	-	`sha256:5b41d5ec640939cf684959234ad3b80909268a32bfd520a31c6720a91521c2fa`  
		Last Modified: Wed, 12 Apr 2023 00:13:13 GMT  
		Size: 35.3 MB (35291995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a23cf789a1d6f1a8f615b2f894ff5d23dfc1871bec09bf4ddc25dfc2f51729`  
		Last Modified: Wed, 12 Apr 2023 01:17:31 GMT  
		Size: 70.8 MB (70783923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f561be54d7ea2acd53189c9a5ceccfe7bcc785342020b6d142e731caa7146a85`  
		Last Modified: Wed, 12 Apr 2023 01:17:14 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3` - linux; s390x

```console
$ docker pull varnish@sha256:76dbe4d565daefa0520c378db042ff9df076dc427aeff7f5e5a18c7e7ab43c6c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.1 MB (87104431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61b1bdad50643f3f50c776b5b349fcd8bc3cde09b4bc391343f3a3d89d1bbe2f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:01:00 GMT
ADD file:b6463dba97ba9c0a29bacfafc4d67bc603ab57e80b75e23cd42d7ef4b0f8e6ae in / 
# Wed, 12 Apr 2023 00:01:04 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:44:24 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 12 Apr 2023 07:44:24 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 12 Apr 2023 07:44:24 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 12 Apr 2023 07:44:24 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 12 Apr 2023 07:44:24 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 12 Apr 2023 07:44:24 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 07:44:25 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 12 Apr 2023 07:44:25 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 12 Apr 2023 07:44:25 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 07:44:25 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 07:44:25 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 07:47:14 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 07:47:17 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 07:47:17 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 07:47:17 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 07:47:17 GMT
USER varnish
# Wed, 12 Apr 2023 07:47:18 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 07:47:18 GMT
CMD []
```

-	Layers:
	-	`sha256:97fe10bc7def58e7938e97e41eec4788ec7a45b6ef2cb1770cec02fa831fd19d`  
		Last Modified: Wed, 12 Apr 2023 00:05:18 GMT  
		Size: 29.7 MB (29653156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:975ac802e6432b31c2c91531f8f143c71a8109aab7895da564b25615d16f2901`  
		Last Modified: Wed, 12 Apr 2023 07:52:51 GMT  
		Size: 57.5 MB (57450785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2115594ecc7bff7e1220a85d4f39fd6717c6cbafa529e8652cee0c74f1abf3b`  
		Last Modified: Wed, 12 Apr 2023 07:52:44 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.3-alpine`

```console
$ docker pull varnish@sha256:1bcc61baae22531bd59b4f66ac0559b261907ca095d5eccf350ffb64f658c813
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
$ docker pull varnish@sha256:5d53f3cea335d15c3e518d4b4bd9ed6d9723e83a11cba3a0096e8dd81bb500a1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.4 MB (59350414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d8db36f71eea7cd47b1a6202cc8f6c57788e74b167c002c0f960e288cf7166e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:14:39 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Thu, 30 Mar 2023 02:14:39 GMT
ARG VARNISH_VERSION=7.3.0
# Thu, 30 Mar 2023 02:14:39 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Thu, 30 Mar 2023 02:14:39 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 30 Mar 2023 02:14:39 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 30 Mar 2023 02:14:39 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 02:14:39 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Thu, 30 Mar 2023 02:14:39 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Thu, 30 Mar 2023 02:14:39 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 02:14:40 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 02:14:40 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 02:16:00 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 02:16:00 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 02:16:00 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 02:16:01 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 02:16:01 GMT
USER varnish
# Thu, 30 Mar 2023 02:16:01 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 02:16:01 GMT
CMD []
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ecd0ddb0fcb995ea02ce3c7936dcb1d915a193f322ca158d7dad0631ac18af`  
		Last Modified: Thu, 30 Mar 2023 02:18:01 GMT  
		Size: 56.5 MB (56523322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7869007cb383d86d06b6b514b6d46fc40ac581add12bbbf143f319ba7a8e7015`  
		Last Modified: Thu, 30 Mar 2023 02:17:54 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:17ebddf73589304daba01e60bdc7bdb5bd09c4ec3a101619994a8c4d77fe4198
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45109401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c39e8bab4b3a15d6f7cb3d240b0f058d4044628947338dda3270ad223d1af8f4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 18:05:06 GMT
ADD file:0516b2e2d8a5c0a3e85e67a20375312bdc586a63094d779b9ac92517cf74a19d in / 
# Wed, 29 Mar 2023 18:05:06 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:10:33 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Thu, 30 Mar 2023 00:10:33 GMT
ARG VARNISH_VERSION=7.3.0
# Thu, 30 Mar 2023 00:10:33 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Thu, 30 Mar 2023 00:10:33 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 30 Mar 2023 00:10:33 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 30 Mar 2023 00:10:33 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 00:10:34 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Thu, 30 Mar 2023 00:10:34 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Thu, 30 Mar 2023 00:10:34 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 00:10:34 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 00:10:34 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 00:11:55 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 00:11:55 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 00:11:55 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 00:11:55 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 00:11:55 GMT
USER varnish
# Thu, 30 Mar 2023 00:11:55 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 00:11:55 GMT
CMD []
```

-	Layers:
	-	`sha256:fafb00bc68cf26e4a27ad2dce7303945ba9e40994e77c9269e610e0452ae9dce`  
		Last Modified: Wed, 29 Mar 2023 18:07:17 GMT  
		Size: 2.4 MB (2437606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f196af073038a0d6be5e1af91b28163c0eaca95c0243eac019991add8bb276`  
		Last Modified: Sat, 08 Apr 2023 02:40:45 GMT  
		Size: 42.7 MB (42671302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d483681d593a3936990d940c17cfe78497a6b081463653220e180980f80af780`  
		Last Modified: Sat, 08 Apr 2023 02:40:39 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:cdef2ee791f1fea0bb632e5fdbe7ab3d1dc08640e869ecbaad970af72cb62ed2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52090155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d26631d7414d095798d5e7800471d90767915486d8223cffd0d9a95dc9379d7a`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:53:56 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Thu, 30 Mar 2023 05:53:56 GMT
ARG VARNISH_VERSION=7.3.0
# Thu, 30 Mar 2023 05:53:56 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Thu, 30 Mar 2023 05:53:56 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 30 Mar 2023 05:53:56 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 30 Mar 2023 05:53:56 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 05:53:56 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Thu, 30 Mar 2023 05:53:56 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Thu, 30 Mar 2023 05:53:57 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 05:53:57 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 05:53:57 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 05:55:07 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 05:55:07 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 05:55:07 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 05:55:07 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 05:55:07 GMT
USER varnish
# Thu, 30 Mar 2023 05:55:07 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 05:55:07 GMT
CMD []
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50d982964542b8110c8924003584227b1310249ecd04ddd79df743a575bc925`  
		Last Modified: Thu, 30 Mar 2023 05:56:46 GMT  
		Size: 49.4 MB (49367657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12b6ca5add2e0d079fd385cac5fdbaa5864540dcd10b770e1548f117a90bd41`  
		Last Modified: Thu, 30 Mar 2023 05:56:40 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3-alpine` - linux; 386

```console
$ docker pull varnish@sha256:f834ae921c56c3eb925d9bea6bc8e1ab80f60425be23ff96bb15cdba11930285
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59538735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ec87c585f44b8fefde94e4cb6f1eef3835e1db4c9686969169c7cd5dd6fb735`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 17:38:36 GMT
ADD file:fca96dde137b6b045359aec9d24257996738ac6cb7cce9518460a66802a27bd7 in / 
# Wed, 29 Mar 2023 17:38:36 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 01:33:46 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Thu, 30 Mar 2023 01:33:46 GMT
ARG VARNISH_VERSION=7.3.0
# Thu, 30 Mar 2023 01:33:46 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Thu, 30 Mar 2023 01:33:47 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 30 Mar 2023 01:33:47 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 30 Mar 2023 01:33:47 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 01:33:47 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Thu, 30 Mar 2023 01:33:47 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Thu, 30 Mar 2023 01:33:47 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 01:33:47 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 01:33:47 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 01:35:56 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 01:35:56 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 01:35:56 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 01:35:56 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 01:35:56 GMT
USER varnish
# Thu, 30 Mar 2023 01:35:56 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 01:35:57 GMT
CMD []
```

-	Layers:
	-	`sha256:333f5f619d7efe58316b2d71276f19d0a59bcb471f4dadaa85762b2c9e02775c`  
		Last Modified: Wed, 29 Mar 2023 17:39:19 GMT  
		Size: 2.8 MB (2832576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20da4d176e921bbb51748136a8fbf517d3cc60798e35724aebdd51ecf2b61ab6`  
		Last Modified: Thu, 30 Mar 2023 01:38:40 GMT  
		Size: 56.7 MB (56705662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a78548a60d6b9d7baf75051feb0fca2994834030bbc04a3645a4572a9757471`  
		Last Modified: Thu, 30 Mar 2023 01:38:30 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:909478b58a275ec2ab8a14120cc9591ebbbdff86f860ea8df1485ae2c264e488
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49136000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d067fd63b0dd3bfee0cefb4eaba611ad41e8cfecb8b2c16ada69e7e227fcb7b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 18:16:40 GMT
ADD file:3c2a8d553fa0998f13f86592f104a9a4ad14f8db46dfa9145c8fbbca0b87ee9a in / 
# Wed, 29 Mar 2023 18:16:40 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:33:21 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Thu, 30 Mar 2023 04:33:22 GMT
ARG VARNISH_VERSION=7.3.0
# Thu, 30 Mar 2023 04:33:22 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Thu, 30 Mar 2023 04:33:22 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 30 Mar 2023 04:33:23 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 30 Mar 2023 04:33:23 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 04:33:23 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Thu, 30 Mar 2023 04:33:23 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Thu, 30 Mar 2023 04:33:24 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 04:33:24 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 04:33:24 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 04:35:35 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 04:35:37 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 04:35:37 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 04:35:37 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 04:35:38 GMT
USER varnish
# Thu, 30 Mar 2023 04:35:38 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 04:35:38 GMT
CMD []
```

-	Layers:
	-	`sha256:0b40b0bd0da3095d93bf74233a1d0bf638b2511fee461df8f6a71aad5a038589`  
		Last Modified: Wed, 29 Mar 2023 18:17:38 GMT  
		Size: 2.8 MB (2813760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5980c95097dfced199688de3f6aa45cd2216bfddef048561966b6608945af2f0`  
		Last Modified: Thu, 30 Mar 2023 04:38:24 GMT  
		Size: 46.3 MB (46321744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690ae6fe9c6e1be629171f54ae05b866b6572efa3b1d22692d741929e7d11bb7`  
		Last Modified: Thu, 30 Mar 2023 04:38:12 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:2fabb6c5fa95ead9711c9785ebab43a38eacb02b418775d6b5ab1a73fa8acc8f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47598984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63eb61c9640b3da92089de86d78ac057c997e5d877f757120cda472c896b941e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 17:42:07 GMT
ADD file:5cf392863cd9a0735de88f9e7dab93c9e74aca59ca05b792943cf3b621ea2c59 in / 
# Wed, 29 Mar 2023 17:42:07 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 23:08:14 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 29 Mar 2023 23:08:14 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 29 Mar 2023 23:08:14 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 29 Mar 2023 23:08:14 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 29 Mar 2023 23:08:14 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 29 Mar 2023 23:08:14 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 29 Mar 2023 23:08:14 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 29 Mar 2023 23:08:15 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 29 Mar 2023 23:08:15 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 29 Mar 2023 23:08:15 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Wed, 29 Mar 2023 23:08:15 GMT
ENV VARNISH_SIZE=100M
# Wed, 29 Mar 2023 23:09:46 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Wed, 29 Mar 2023 23:09:47 GMT
WORKDIR /etc/varnish
# Wed, 29 Mar 2023 23:09:47 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 29 Mar 2023 23:09:48 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 29 Mar 2023 23:09:48 GMT
USER varnish
# Wed, 29 Mar 2023 23:09:48 GMT
EXPOSE 80 8443
# Wed, 29 Mar 2023 23:09:48 GMT
CMD []
```

-	Layers:
	-	`sha256:1536575ac9c5f5fff4522c60d4610af0a52be584c36e652080c6c0ad169d4f27`  
		Last Modified: Wed, 29 Mar 2023 17:42:42 GMT  
		Size: 2.6 MB (2610636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dadb2417c7920374afa7798d98c70d2f0a8290f641bb3dbc112a2158ac097a2d`  
		Last Modified: Wed, 29 Mar 2023 23:12:02 GMT  
		Size: 45.0 MB (44987850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a556b2e0ae2040be8338c713604078ac74fa7ec335f48fff28337d8b007e52`  
		Last Modified: Wed, 29 Mar 2023 23:11:56 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.3.0`

```console
$ docker pull varnish@sha256:d50f601a76ff2cefca6afa7587c75dc46ad482b7734baab89eaf79a6516c90f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:7.3.0` - linux; amd64

```console
$ docker pull varnish@sha256:01c1f0ee2a532a0f480fa00e8b754c2a1662ab5989e3958d966222ed09f95d02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106805687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38f8fe02f4ba954dfed4760af3cb20e716fb19e427144a743bb942eca093bd75`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:35:52 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 12 Apr 2023 07:35:52 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 12 Apr 2023 07:35:52 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 12 Apr 2023 07:35:52 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 12 Apr 2023 07:35:52 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 12 Apr 2023 07:35:52 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 07:35:52 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 12 Apr 2023 07:35:52 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 12 Apr 2023 07:35:52 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 07:35:52 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 07:35:53 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 07:38:58 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 07:38:58 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 07:38:59 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 07:38:59 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 07:38:59 GMT
USER varnish
# Wed, 12 Apr 2023 07:38:59 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 07:38:59 GMT
CMD []
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c1be847abb1fb38853dbae20352d1f2e2b780db54e88fbb737549a5aab7a79`  
		Last Modified: Wed, 12 Apr 2023 07:44:41 GMT  
		Size: 75.4 MB (75386967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb31db21e143ba8b279a4dc67a859edafd358e53f1efdbe4ac92744d507f6ddd`  
		Last Modified: Wed, 12 Apr 2023 07:44:32 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3.0` - linux; arm variant v7

```console
$ docker pull varnish@sha256:ee2c275680aed583fea7ceba04074e69fda8c8747dbd68766d2e0d9c55512f03
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.1 MB (83149297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7730d361798ab6943823a20c73d9f1bee65ccfe1300978e219422823cbce78b9`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 11 Apr 2023 23:59:44 GMT
ADD file:e5f4777456ed4424053e9aa1f3d783f57da094c7a6c6d9d7a2fd315e00b5bbb0 in / 
# Tue, 11 Apr 2023 23:59:44 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 09:48:46 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 12 Apr 2023 09:48:47 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 12 Apr 2023 09:48:47 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 12 Apr 2023 09:48:47 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 12 Apr 2023 09:48:47 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 12 Apr 2023 09:48:48 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 09:48:48 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 12 Apr 2023 09:48:48 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 12 Apr 2023 09:48:48 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 09:48:49 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 09:48:49 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 09:52:44 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 09:52:44 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 09:52:44 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 09:52:45 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 09:52:45 GMT
USER varnish
# Wed, 12 Apr 2023 09:52:45 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 09:52:45 GMT
CMD []
```

-	Layers:
	-	`sha256:99c2a28b4a43ce341eb611e82106b886315f30a250473617f2293828e10d8fff`  
		Last Modified: Wed, 12 Apr 2023 00:03:19 GMT  
		Size: 26.6 MB (26579772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:946f48177dd61e98fafd1f5db674994ba0ad766c7b50f4b06c552e129d2be463`  
		Last Modified: Wed, 12 Apr 2023 09:57:58 GMT  
		Size: 56.6 MB (56569036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c94d0d1168a78363c629071b130cf202012a5c2285cff907fbe05f9f7d3166e2`  
		Last Modified: Wed, 12 Apr 2023 09:57:50 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3.0` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:02ef5b0996ff812c54abd99265f8b339cd393d1be211f3cc646f918ffd4bea02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100589822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:036a0598d94c3d082574590889afad8344a4b710a2705cc884c821afd482967e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 04:45:29 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 12 Apr 2023 04:45:29 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 12 Apr 2023 04:45:29 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 12 Apr 2023 04:45:29 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 12 Apr 2023 04:45:29 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 12 Apr 2023 04:45:29 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 04:45:29 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 12 Apr 2023 04:45:29 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 12 Apr 2023 04:45:30 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 04:45:30 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 04:45:30 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 04:48:22 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 04:48:23 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 04:48:23 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:48:23 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 04:48:23 GMT
USER varnish
# Wed, 12 Apr 2023 04:48:23 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 04:48:23 GMT
CMD []
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b6030c7f52818939f055e2f6663b1b9cc13fd7547b1c2e0f753f5b87cd93ca`  
		Last Modified: Wed, 12 Apr 2023 04:53:10 GMT  
		Size: 70.5 MB (70525505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74565242087dac611bbba86cb8a4ef8aa9aa3712f40e4ab8949602813f427c6b`  
		Last Modified: Wed, 12 Apr 2023 04:53:03 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3.0` - linux; 386

```console
$ docker pull varnish@sha256:88f2d7b6250c7d29544a99d128dc2aafe14c362633b4ff697b2720611c261141
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.2 MB (108173601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bfc3f953767b14e681b22c82c947846dedc22c394cd082cea401378516935b4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:39:01 GMT
ADD file:42fc1b4536cdd6823499b0c94d799e9bfbcb280b7df55d8d6c9f6defd61ecb6e in / 
# Wed, 12 Apr 2023 00:39:01 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 04:13:43 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 12 Apr 2023 04:13:44 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 12 Apr 2023 04:13:44 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 12 Apr 2023 04:13:44 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 12 Apr 2023 04:13:44 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 12 Apr 2023 04:13:44 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 04:13:44 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 12 Apr 2023 04:13:44 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 12 Apr 2023 04:13:44 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 04:13:44 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 04:13:44 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 04:18:07 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 04:18:08 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 04:18:08 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:18:08 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 04:18:08 GMT
USER varnish
# Wed, 12 Apr 2023 04:18:08 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 04:18:08 GMT
CMD []
```

-	Layers:
	-	`sha256:b2ee1f87789d52ef09851b4e5c9745fb8aceafa107b0d3452f9973f1abe65042`  
		Last Modified: Wed, 12 Apr 2023 00:42:45 GMT  
		Size: 32.4 MB (32398925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee5e7f863a0627e32c4308f8e477d218c74b26149178e5f23057f2339a55e64`  
		Last Modified: Wed, 12 Apr 2023 04:25:03 GMT  
		Size: 75.8 MB (75774186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c73471ce047c640427aa8d168e423ce9d464179d283e9ecc90c6dca784deef`  
		Last Modified: Wed, 12 Apr 2023 04:24:49 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3.0` - linux; ppc64le

```console
$ docker pull varnish@sha256:99a9dcf0cddca561abbcd5bc5b002adbb083de964d8746e3063cab564573c331
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.1 MB (106076410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e817121269101ae25eb3c824355809f156a4e72be8a908710817a5575d2fb848`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:08:20 GMT
ADD file:63eb52aaff02c15bceabb87a78eb1b36389066ff4774cf8a754160ca7d509816 in / 
# Wed, 12 Apr 2023 00:08:23 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:43:55 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 12 Apr 2023 00:43:56 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 12 Apr 2023 00:43:56 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 12 Apr 2023 00:43:57 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 12 Apr 2023 00:43:57 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 12 Apr 2023 00:43:58 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 00:43:58 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 12 Apr 2023 00:43:59 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 12 Apr 2023 00:43:59 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 00:44:00 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 00:44:00 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 00:55:22 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 00:55:26 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 00:55:26 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 00:55:27 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 00:55:28 GMT
USER varnish
# Wed, 12 Apr 2023 00:55:28 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 00:55:29 GMT
CMD []
```

-	Layers:
	-	`sha256:5b41d5ec640939cf684959234ad3b80909268a32bfd520a31c6720a91521c2fa`  
		Last Modified: Wed, 12 Apr 2023 00:13:13 GMT  
		Size: 35.3 MB (35291995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a23cf789a1d6f1a8f615b2f894ff5d23dfc1871bec09bf4ddc25dfc2f51729`  
		Last Modified: Wed, 12 Apr 2023 01:17:31 GMT  
		Size: 70.8 MB (70783923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f561be54d7ea2acd53189c9a5ceccfe7bcc785342020b6d142e731caa7146a85`  
		Last Modified: Wed, 12 Apr 2023 01:17:14 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3.0` - linux; s390x

```console
$ docker pull varnish@sha256:76dbe4d565daefa0520c378db042ff9df076dc427aeff7f5e5a18c7e7ab43c6c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.1 MB (87104431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61b1bdad50643f3f50c776b5b349fcd8bc3cde09b4bc391343f3a3d89d1bbe2f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:01:00 GMT
ADD file:b6463dba97ba9c0a29bacfafc4d67bc603ab57e80b75e23cd42d7ef4b0f8e6ae in / 
# Wed, 12 Apr 2023 00:01:04 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:44:24 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 12 Apr 2023 07:44:24 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 12 Apr 2023 07:44:24 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 12 Apr 2023 07:44:24 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 12 Apr 2023 07:44:24 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 12 Apr 2023 07:44:24 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 07:44:25 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 12 Apr 2023 07:44:25 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 12 Apr 2023 07:44:25 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 07:44:25 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 07:44:25 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 07:47:14 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 07:47:17 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 07:47:17 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 07:47:17 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 07:47:17 GMT
USER varnish
# Wed, 12 Apr 2023 07:47:18 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 07:47:18 GMT
CMD []
```

-	Layers:
	-	`sha256:97fe10bc7def58e7938e97e41eec4788ec7a45b6ef2cb1770cec02fa831fd19d`  
		Last Modified: Wed, 12 Apr 2023 00:05:18 GMT  
		Size: 29.7 MB (29653156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:975ac802e6432b31c2c91531f8f143c71a8109aab7895da564b25615d16f2901`  
		Last Modified: Wed, 12 Apr 2023 07:52:51 GMT  
		Size: 57.5 MB (57450785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2115594ecc7bff7e1220a85d4f39fd6717c6cbafa529e8652cee0c74f1abf3b`  
		Last Modified: Wed, 12 Apr 2023 07:52:44 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.3.0-alpine`

```console
$ docker pull varnish@sha256:1bcc61baae22531bd59b4f66ac0559b261907ca095d5eccf350ffb64f658c813
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:7.3.0-alpine` - linux; amd64

```console
$ docker pull varnish@sha256:5d53f3cea335d15c3e518d4b4bd9ed6d9723e83a11cba3a0096e8dd81bb500a1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.4 MB (59350414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d8db36f71eea7cd47b1a6202cc8f6c57788e74b167c002c0f960e288cf7166e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:14:39 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Thu, 30 Mar 2023 02:14:39 GMT
ARG VARNISH_VERSION=7.3.0
# Thu, 30 Mar 2023 02:14:39 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Thu, 30 Mar 2023 02:14:39 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 30 Mar 2023 02:14:39 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 30 Mar 2023 02:14:39 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 02:14:39 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Thu, 30 Mar 2023 02:14:39 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Thu, 30 Mar 2023 02:14:39 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 02:14:40 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 02:14:40 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 02:16:00 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 02:16:00 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 02:16:00 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 02:16:01 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 02:16:01 GMT
USER varnish
# Thu, 30 Mar 2023 02:16:01 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 02:16:01 GMT
CMD []
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ecd0ddb0fcb995ea02ce3c7936dcb1d915a193f322ca158d7dad0631ac18af`  
		Last Modified: Thu, 30 Mar 2023 02:18:01 GMT  
		Size: 56.5 MB (56523322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7869007cb383d86d06b6b514b6d46fc40ac581add12bbbf143f319ba7a8e7015`  
		Last Modified: Thu, 30 Mar 2023 02:17:54 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3.0-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:17ebddf73589304daba01e60bdc7bdb5bd09c4ec3a101619994a8c4d77fe4198
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45109401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c39e8bab4b3a15d6f7cb3d240b0f058d4044628947338dda3270ad223d1af8f4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 18:05:06 GMT
ADD file:0516b2e2d8a5c0a3e85e67a20375312bdc586a63094d779b9ac92517cf74a19d in / 
# Wed, 29 Mar 2023 18:05:06 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:10:33 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Thu, 30 Mar 2023 00:10:33 GMT
ARG VARNISH_VERSION=7.3.0
# Thu, 30 Mar 2023 00:10:33 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Thu, 30 Mar 2023 00:10:33 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 30 Mar 2023 00:10:33 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 30 Mar 2023 00:10:33 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 00:10:34 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Thu, 30 Mar 2023 00:10:34 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Thu, 30 Mar 2023 00:10:34 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 00:10:34 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 00:10:34 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 00:11:55 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 00:11:55 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 00:11:55 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 00:11:55 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 00:11:55 GMT
USER varnish
# Thu, 30 Mar 2023 00:11:55 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 00:11:55 GMT
CMD []
```

-	Layers:
	-	`sha256:fafb00bc68cf26e4a27ad2dce7303945ba9e40994e77c9269e610e0452ae9dce`  
		Last Modified: Wed, 29 Mar 2023 18:07:17 GMT  
		Size: 2.4 MB (2437606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f196af073038a0d6be5e1af91b28163c0eaca95c0243eac019991add8bb276`  
		Last Modified: Sat, 08 Apr 2023 02:40:45 GMT  
		Size: 42.7 MB (42671302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d483681d593a3936990d940c17cfe78497a6b081463653220e180980f80af780`  
		Last Modified: Sat, 08 Apr 2023 02:40:39 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3.0-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:cdef2ee791f1fea0bb632e5fdbe7ab3d1dc08640e869ecbaad970af72cb62ed2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52090155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d26631d7414d095798d5e7800471d90767915486d8223cffd0d9a95dc9379d7a`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:53:56 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Thu, 30 Mar 2023 05:53:56 GMT
ARG VARNISH_VERSION=7.3.0
# Thu, 30 Mar 2023 05:53:56 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Thu, 30 Mar 2023 05:53:56 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 30 Mar 2023 05:53:56 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 30 Mar 2023 05:53:56 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 05:53:56 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Thu, 30 Mar 2023 05:53:56 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Thu, 30 Mar 2023 05:53:57 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 05:53:57 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 05:53:57 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 05:55:07 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 05:55:07 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 05:55:07 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 05:55:07 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 05:55:07 GMT
USER varnish
# Thu, 30 Mar 2023 05:55:07 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 05:55:07 GMT
CMD []
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50d982964542b8110c8924003584227b1310249ecd04ddd79df743a575bc925`  
		Last Modified: Thu, 30 Mar 2023 05:56:46 GMT  
		Size: 49.4 MB (49367657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12b6ca5add2e0d079fd385cac5fdbaa5864540dcd10b770e1548f117a90bd41`  
		Last Modified: Thu, 30 Mar 2023 05:56:40 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3.0-alpine` - linux; 386

```console
$ docker pull varnish@sha256:f834ae921c56c3eb925d9bea6bc8e1ab80f60425be23ff96bb15cdba11930285
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59538735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ec87c585f44b8fefde94e4cb6f1eef3835e1db4c9686969169c7cd5dd6fb735`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 17:38:36 GMT
ADD file:fca96dde137b6b045359aec9d24257996738ac6cb7cce9518460a66802a27bd7 in / 
# Wed, 29 Mar 2023 17:38:36 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 01:33:46 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Thu, 30 Mar 2023 01:33:46 GMT
ARG VARNISH_VERSION=7.3.0
# Thu, 30 Mar 2023 01:33:46 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Thu, 30 Mar 2023 01:33:47 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 30 Mar 2023 01:33:47 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 30 Mar 2023 01:33:47 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 01:33:47 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Thu, 30 Mar 2023 01:33:47 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Thu, 30 Mar 2023 01:33:47 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 01:33:47 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 01:33:47 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 01:35:56 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 01:35:56 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 01:35:56 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 01:35:56 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 01:35:56 GMT
USER varnish
# Thu, 30 Mar 2023 01:35:56 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 01:35:57 GMT
CMD []
```

-	Layers:
	-	`sha256:333f5f619d7efe58316b2d71276f19d0a59bcb471f4dadaa85762b2c9e02775c`  
		Last Modified: Wed, 29 Mar 2023 17:39:19 GMT  
		Size: 2.8 MB (2832576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20da4d176e921bbb51748136a8fbf517d3cc60798e35724aebdd51ecf2b61ab6`  
		Last Modified: Thu, 30 Mar 2023 01:38:40 GMT  
		Size: 56.7 MB (56705662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a78548a60d6b9d7baf75051feb0fca2994834030bbc04a3645a4572a9757471`  
		Last Modified: Thu, 30 Mar 2023 01:38:30 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3.0-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:909478b58a275ec2ab8a14120cc9591ebbbdff86f860ea8df1485ae2c264e488
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49136000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d067fd63b0dd3bfee0cefb4eaba611ad41e8cfecb8b2c16ada69e7e227fcb7b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 18:16:40 GMT
ADD file:3c2a8d553fa0998f13f86592f104a9a4ad14f8db46dfa9145c8fbbca0b87ee9a in / 
# Wed, 29 Mar 2023 18:16:40 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:33:21 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Thu, 30 Mar 2023 04:33:22 GMT
ARG VARNISH_VERSION=7.3.0
# Thu, 30 Mar 2023 04:33:22 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Thu, 30 Mar 2023 04:33:22 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 30 Mar 2023 04:33:23 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 30 Mar 2023 04:33:23 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 04:33:23 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Thu, 30 Mar 2023 04:33:23 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Thu, 30 Mar 2023 04:33:24 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 04:33:24 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 04:33:24 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 04:35:35 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 04:35:37 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 04:35:37 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 04:35:37 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 04:35:38 GMT
USER varnish
# Thu, 30 Mar 2023 04:35:38 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 04:35:38 GMT
CMD []
```

-	Layers:
	-	`sha256:0b40b0bd0da3095d93bf74233a1d0bf638b2511fee461df8f6a71aad5a038589`  
		Last Modified: Wed, 29 Mar 2023 18:17:38 GMT  
		Size: 2.8 MB (2813760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5980c95097dfced199688de3f6aa45cd2216bfddef048561966b6608945af2f0`  
		Last Modified: Thu, 30 Mar 2023 04:38:24 GMT  
		Size: 46.3 MB (46321744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690ae6fe9c6e1be629171f54ae05b866b6572efa3b1d22692d741929e7d11bb7`  
		Last Modified: Thu, 30 Mar 2023 04:38:12 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3.0-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:2fabb6c5fa95ead9711c9785ebab43a38eacb02b418775d6b5ab1a73fa8acc8f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47598984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63eb61c9640b3da92089de86d78ac057c997e5d877f757120cda472c896b941e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 17:42:07 GMT
ADD file:5cf392863cd9a0735de88f9e7dab93c9e74aca59ca05b792943cf3b621ea2c59 in / 
# Wed, 29 Mar 2023 17:42:07 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 23:08:14 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 29 Mar 2023 23:08:14 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 29 Mar 2023 23:08:14 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 29 Mar 2023 23:08:14 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 29 Mar 2023 23:08:14 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 29 Mar 2023 23:08:14 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 29 Mar 2023 23:08:14 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 29 Mar 2023 23:08:15 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 29 Mar 2023 23:08:15 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 29 Mar 2023 23:08:15 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Wed, 29 Mar 2023 23:08:15 GMT
ENV VARNISH_SIZE=100M
# Wed, 29 Mar 2023 23:09:46 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Wed, 29 Mar 2023 23:09:47 GMT
WORKDIR /etc/varnish
# Wed, 29 Mar 2023 23:09:47 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 29 Mar 2023 23:09:48 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 29 Mar 2023 23:09:48 GMT
USER varnish
# Wed, 29 Mar 2023 23:09:48 GMT
EXPOSE 80 8443
# Wed, 29 Mar 2023 23:09:48 GMT
CMD []
```

-	Layers:
	-	`sha256:1536575ac9c5f5fff4522c60d4610af0a52be584c36e652080c6c0ad169d4f27`  
		Last Modified: Wed, 29 Mar 2023 17:42:42 GMT  
		Size: 2.6 MB (2610636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dadb2417c7920374afa7798d98c70d2f0a8290f641bb3dbc112a2158ac097a2d`  
		Last Modified: Wed, 29 Mar 2023 23:12:02 GMT  
		Size: 45.0 MB (44987850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a556b2e0ae2040be8338c713604078ac74fa7ec335f48fff28337d8b007e52`  
		Last Modified: Wed, 29 Mar 2023 23:11:56 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:alpine`

```console
$ docker pull varnish@sha256:1bcc61baae22531bd59b4f66ac0559b261907ca095d5eccf350ffb64f658c813
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
$ docker pull varnish@sha256:5d53f3cea335d15c3e518d4b4bd9ed6d9723e83a11cba3a0096e8dd81bb500a1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.4 MB (59350414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d8db36f71eea7cd47b1a6202cc8f6c57788e74b167c002c0f960e288cf7166e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:14:39 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Thu, 30 Mar 2023 02:14:39 GMT
ARG VARNISH_VERSION=7.3.0
# Thu, 30 Mar 2023 02:14:39 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Thu, 30 Mar 2023 02:14:39 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 30 Mar 2023 02:14:39 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 30 Mar 2023 02:14:39 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 02:14:39 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Thu, 30 Mar 2023 02:14:39 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Thu, 30 Mar 2023 02:14:39 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 02:14:40 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 02:14:40 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 02:16:00 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 02:16:00 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 02:16:00 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 02:16:01 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 02:16:01 GMT
USER varnish
# Thu, 30 Mar 2023 02:16:01 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 02:16:01 GMT
CMD []
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ecd0ddb0fcb995ea02ce3c7936dcb1d915a193f322ca158d7dad0631ac18af`  
		Last Modified: Thu, 30 Mar 2023 02:18:01 GMT  
		Size: 56.5 MB (56523322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7869007cb383d86d06b6b514b6d46fc40ac581add12bbbf143f319ba7a8e7015`  
		Last Modified: Thu, 30 Mar 2023 02:17:54 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:17ebddf73589304daba01e60bdc7bdb5bd09c4ec3a101619994a8c4d77fe4198
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45109401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c39e8bab4b3a15d6f7cb3d240b0f058d4044628947338dda3270ad223d1af8f4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 18:05:06 GMT
ADD file:0516b2e2d8a5c0a3e85e67a20375312bdc586a63094d779b9ac92517cf74a19d in / 
# Wed, 29 Mar 2023 18:05:06 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:10:33 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Thu, 30 Mar 2023 00:10:33 GMT
ARG VARNISH_VERSION=7.3.0
# Thu, 30 Mar 2023 00:10:33 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Thu, 30 Mar 2023 00:10:33 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 30 Mar 2023 00:10:33 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 30 Mar 2023 00:10:33 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 00:10:34 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Thu, 30 Mar 2023 00:10:34 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Thu, 30 Mar 2023 00:10:34 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 00:10:34 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 00:10:34 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 00:11:55 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 00:11:55 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 00:11:55 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 00:11:55 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 00:11:55 GMT
USER varnish
# Thu, 30 Mar 2023 00:11:55 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 00:11:55 GMT
CMD []
```

-	Layers:
	-	`sha256:fafb00bc68cf26e4a27ad2dce7303945ba9e40994e77c9269e610e0452ae9dce`  
		Last Modified: Wed, 29 Mar 2023 18:07:17 GMT  
		Size: 2.4 MB (2437606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f196af073038a0d6be5e1af91b28163c0eaca95c0243eac019991add8bb276`  
		Last Modified: Sat, 08 Apr 2023 02:40:45 GMT  
		Size: 42.7 MB (42671302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d483681d593a3936990d940c17cfe78497a6b081463653220e180980f80af780`  
		Last Modified: Sat, 08 Apr 2023 02:40:39 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:cdef2ee791f1fea0bb632e5fdbe7ab3d1dc08640e869ecbaad970af72cb62ed2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52090155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d26631d7414d095798d5e7800471d90767915486d8223cffd0d9a95dc9379d7a`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:53:56 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Thu, 30 Mar 2023 05:53:56 GMT
ARG VARNISH_VERSION=7.3.0
# Thu, 30 Mar 2023 05:53:56 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Thu, 30 Mar 2023 05:53:56 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 30 Mar 2023 05:53:56 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 30 Mar 2023 05:53:56 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 05:53:56 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Thu, 30 Mar 2023 05:53:56 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Thu, 30 Mar 2023 05:53:57 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 05:53:57 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 05:53:57 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 05:55:07 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 05:55:07 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 05:55:07 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 05:55:07 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 05:55:07 GMT
USER varnish
# Thu, 30 Mar 2023 05:55:07 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 05:55:07 GMT
CMD []
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50d982964542b8110c8924003584227b1310249ecd04ddd79df743a575bc925`  
		Last Modified: Thu, 30 Mar 2023 05:56:46 GMT  
		Size: 49.4 MB (49367657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12b6ca5add2e0d079fd385cac5fdbaa5864540dcd10b770e1548f117a90bd41`  
		Last Modified: Thu, 30 Mar 2023 05:56:40 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; 386

```console
$ docker pull varnish@sha256:f834ae921c56c3eb925d9bea6bc8e1ab80f60425be23ff96bb15cdba11930285
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59538735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ec87c585f44b8fefde94e4cb6f1eef3835e1db4c9686969169c7cd5dd6fb735`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 17:38:36 GMT
ADD file:fca96dde137b6b045359aec9d24257996738ac6cb7cce9518460a66802a27bd7 in / 
# Wed, 29 Mar 2023 17:38:36 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 01:33:46 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Thu, 30 Mar 2023 01:33:46 GMT
ARG VARNISH_VERSION=7.3.0
# Thu, 30 Mar 2023 01:33:46 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Thu, 30 Mar 2023 01:33:47 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 30 Mar 2023 01:33:47 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 30 Mar 2023 01:33:47 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 01:33:47 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Thu, 30 Mar 2023 01:33:47 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Thu, 30 Mar 2023 01:33:47 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 01:33:47 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 01:33:47 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 01:35:56 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 01:35:56 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 01:35:56 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 01:35:56 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 01:35:56 GMT
USER varnish
# Thu, 30 Mar 2023 01:35:56 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 01:35:57 GMT
CMD []
```

-	Layers:
	-	`sha256:333f5f619d7efe58316b2d71276f19d0a59bcb471f4dadaa85762b2c9e02775c`  
		Last Modified: Wed, 29 Mar 2023 17:39:19 GMT  
		Size: 2.8 MB (2832576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20da4d176e921bbb51748136a8fbf517d3cc60798e35724aebdd51ecf2b61ab6`  
		Last Modified: Thu, 30 Mar 2023 01:38:40 GMT  
		Size: 56.7 MB (56705662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a78548a60d6b9d7baf75051feb0fca2994834030bbc04a3645a4572a9757471`  
		Last Modified: Thu, 30 Mar 2023 01:38:30 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:909478b58a275ec2ab8a14120cc9591ebbbdff86f860ea8df1485ae2c264e488
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49136000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d067fd63b0dd3bfee0cefb4eaba611ad41e8cfecb8b2c16ada69e7e227fcb7b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 18:16:40 GMT
ADD file:3c2a8d553fa0998f13f86592f104a9a4ad14f8db46dfa9145c8fbbca0b87ee9a in / 
# Wed, 29 Mar 2023 18:16:40 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:33:21 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Thu, 30 Mar 2023 04:33:22 GMT
ARG VARNISH_VERSION=7.3.0
# Thu, 30 Mar 2023 04:33:22 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Thu, 30 Mar 2023 04:33:22 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 30 Mar 2023 04:33:23 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 30 Mar 2023 04:33:23 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 04:33:23 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Thu, 30 Mar 2023 04:33:23 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Thu, 30 Mar 2023 04:33:24 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 04:33:24 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 04:33:24 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 04:35:35 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 04:35:37 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 04:35:37 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 04:35:37 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 04:35:38 GMT
USER varnish
# Thu, 30 Mar 2023 04:35:38 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 04:35:38 GMT
CMD []
```

-	Layers:
	-	`sha256:0b40b0bd0da3095d93bf74233a1d0bf638b2511fee461df8f6a71aad5a038589`  
		Last Modified: Wed, 29 Mar 2023 18:17:38 GMT  
		Size: 2.8 MB (2813760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5980c95097dfced199688de3f6aa45cd2216bfddef048561966b6608945af2f0`  
		Last Modified: Thu, 30 Mar 2023 04:38:24 GMT  
		Size: 46.3 MB (46321744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690ae6fe9c6e1be629171f54ae05b866b6572efa3b1d22692d741929e7d11bb7`  
		Last Modified: Thu, 30 Mar 2023 04:38:12 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; s390x

```console
$ docker pull varnish@sha256:2fabb6c5fa95ead9711c9785ebab43a38eacb02b418775d6b5ab1a73fa8acc8f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47598984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63eb61c9640b3da92089de86d78ac057c997e5d877f757120cda472c896b941e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 17:42:07 GMT
ADD file:5cf392863cd9a0735de88f9e7dab93c9e74aca59ca05b792943cf3b621ea2c59 in / 
# Wed, 29 Mar 2023 17:42:07 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 23:08:14 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 29 Mar 2023 23:08:14 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 29 Mar 2023 23:08:14 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 29 Mar 2023 23:08:14 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 29 Mar 2023 23:08:14 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 29 Mar 2023 23:08:14 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 29 Mar 2023 23:08:14 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 29 Mar 2023 23:08:15 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 29 Mar 2023 23:08:15 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 29 Mar 2023 23:08:15 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Wed, 29 Mar 2023 23:08:15 GMT
ENV VARNISH_SIZE=100M
# Wed, 29 Mar 2023 23:09:46 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Wed, 29 Mar 2023 23:09:47 GMT
WORKDIR /etc/varnish
# Wed, 29 Mar 2023 23:09:47 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 29 Mar 2023 23:09:48 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 29 Mar 2023 23:09:48 GMT
USER varnish
# Wed, 29 Mar 2023 23:09:48 GMT
EXPOSE 80 8443
# Wed, 29 Mar 2023 23:09:48 GMT
CMD []
```

-	Layers:
	-	`sha256:1536575ac9c5f5fff4522c60d4610af0a52be584c36e652080c6c0ad169d4f27`  
		Last Modified: Wed, 29 Mar 2023 17:42:42 GMT  
		Size: 2.6 MB (2610636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dadb2417c7920374afa7798d98c70d2f0a8290f641bb3dbc112a2158ac097a2d`  
		Last Modified: Wed, 29 Mar 2023 23:12:02 GMT  
		Size: 45.0 MB (44987850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a556b2e0ae2040be8338c713604078ac74fa7ec335f48fff28337d8b007e52`  
		Last Modified: Wed, 29 Mar 2023 23:11:56 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:fresh`

```console
$ docker pull varnish@sha256:d50f601a76ff2cefca6afa7587c75dc46ad482b7734baab89eaf79a6516c90f4
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
$ docker pull varnish@sha256:01c1f0ee2a532a0f480fa00e8b754c2a1662ab5989e3958d966222ed09f95d02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106805687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38f8fe02f4ba954dfed4760af3cb20e716fb19e427144a743bb942eca093bd75`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:35:52 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 12 Apr 2023 07:35:52 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 12 Apr 2023 07:35:52 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 12 Apr 2023 07:35:52 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 12 Apr 2023 07:35:52 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 12 Apr 2023 07:35:52 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 07:35:52 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 12 Apr 2023 07:35:52 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 12 Apr 2023 07:35:52 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 07:35:52 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 07:35:53 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 07:38:58 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 07:38:58 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 07:38:59 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 07:38:59 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 07:38:59 GMT
USER varnish
# Wed, 12 Apr 2023 07:38:59 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 07:38:59 GMT
CMD []
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c1be847abb1fb38853dbae20352d1f2e2b780db54e88fbb737549a5aab7a79`  
		Last Modified: Wed, 12 Apr 2023 07:44:41 GMT  
		Size: 75.4 MB (75386967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb31db21e143ba8b279a4dc67a859edafd358e53f1efdbe4ac92744d507f6ddd`  
		Last Modified: Wed, 12 Apr 2023 07:44:32 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; arm variant v7

```console
$ docker pull varnish@sha256:ee2c275680aed583fea7ceba04074e69fda8c8747dbd68766d2e0d9c55512f03
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.1 MB (83149297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7730d361798ab6943823a20c73d9f1bee65ccfe1300978e219422823cbce78b9`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 11 Apr 2023 23:59:44 GMT
ADD file:e5f4777456ed4424053e9aa1f3d783f57da094c7a6c6d9d7a2fd315e00b5bbb0 in / 
# Tue, 11 Apr 2023 23:59:44 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 09:48:46 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 12 Apr 2023 09:48:47 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 12 Apr 2023 09:48:47 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 12 Apr 2023 09:48:47 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 12 Apr 2023 09:48:47 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 12 Apr 2023 09:48:48 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 09:48:48 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 12 Apr 2023 09:48:48 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 12 Apr 2023 09:48:48 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 09:48:49 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 09:48:49 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 09:52:44 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 09:52:44 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 09:52:44 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 09:52:45 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 09:52:45 GMT
USER varnish
# Wed, 12 Apr 2023 09:52:45 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 09:52:45 GMT
CMD []
```

-	Layers:
	-	`sha256:99c2a28b4a43ce341eb611e82106b886315f30a250473617f2293828e10d8fff`  
		Last Modified: Wed, 12 Apr 2023 00:03:19 GMT  
		Size: 26.6 MB (26579772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:946f48177dd61e98fafd1f5db674994ba0ad766c7b50f4b06c552e129d2be463`  
		Last Modified: Wed, 12 Apr 2023 09:57:58 GMT  
		Size: 56.6 MB (56569036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c94d0d1168a78363c629071b130cf202012a5c2285cff907fbe05f9f7d3166e2`  
		Last Modified: Wed, 12 Apr 2023 09:57:50 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:02ef5b0996ff812c54abd99265f8b339cd393d1be211f3cc646f918ffd4bea02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100589822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:036a0598d94c3d082574590889afad8344a4b710a2705cc884c821afd482967e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 04:45:29 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 12 Apr 2023 04:45:29 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 12 Apr 2023 04:45:29 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 12 Apr 2023 04:45:29 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 12 Apr 2023 04:45:29 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 12 Apr 2023 04:45:29 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 04:45:29 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 12 Apr 2023 04:45:29 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 12 Apr 2023 04:45:30 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 04:45:30 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 04:45:30 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 04:48:22 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 04:48:23 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 04:48:23 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:48:23 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 04:48:23 GMT
USER varnish
# Wed, 12 Apr 2023 04:48:23 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 04:48:23 GMT
CMD []
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b6030c7f52818939f055e2f6663b1b9cc13fd7547b1c2e0f753f5b87cd93ca`  
		Last Modified: Wed, 12 Apr 2023 04:53:10 GMT  
		Size: 70.5 MB (70525505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74565242087dac611bbba86cb8a4ef8aa9aa3712f40e4ab8949602813f427c6b`  
		Last Modified: Wed, 12 Apr 2023 04:53:03 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; 386

```console
$ docker pull varnish@sha256:88f2d7b6250c7d29544a99d128dc2aafe14c362633b4ff697b2720611c261141
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.2 MB (108173601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bfc3f953767b14e681b22c82c947846dedc22c394cd082cea401378516935b4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:39:01 GMT
ADD file:42fc1b4536cdd6823499b0c94d799e9bfbcb280b7df55d8d6c9f6defd61ecb6e in / 
# Wed, 12 Apr 2023 00:39:01 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 04:13:43 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 12 Apr 2023 04:13:44 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 12 Apr 2023 04:13:44 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 12 Apr 2023 04:13:44 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 12 Apr 2023 04:13:44 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 12 Apr 2023 04:13:44 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 04:13:44 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 12 Apr 2023 04:13:44 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 12 Apr 2023 04:13:44 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 04:13:44 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 04:13:44 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 04:18:07 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 04:18:08 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 04:18:08 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:18:08 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 04:18:08 GMT
USER varnish
# Wed, 12 Apr 2023 04:18:08 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 04:18:08 GMT
CMD []
```

-	Layers:
	-	`sha256:b2ee1f87789d52ef09851b4e5c9745fb8aceafa107b0d3452f9973f1abe65042`  
		Last Modified: Wed, 12 Apr 2023 00:42:45 GMT  
		Size: 32.4 MB (32398925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee5e7f863a0627e32c4308f8e477d218c74b26149178e5f23057f2339a55e64`  
		Last Modified: Wed, 12 Apr 2023 04:25:03 GMT  
		Size: 75.8 MB (75774186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c73471ce047c640427aa8d168e423ce9d464179d283e9ecc90c6dca784deef`  
		Last Modified: Wed, 12 Apr 2023 04:24:49 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; ppc64le

```console
$ docker pull varnish@sha256:99a9dcf0cddca561abbcd5bc5b002adbb083de964d8746e3063cab564573c331
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.1 MB (106076410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e817121269101ae25eb3c824355809f156a4e72be8a908710817a5575d2fb848`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:08:20 GMT
ADD file:63eb52aaff02c15bceabb87a78eb1b36389066ff4774cf8a754160ca7d509816 in / 
# Wed, 12 Apr 2023 00:08:23 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:43:55 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 12 Apr 2023 00:43:56 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 12 Apr 2023 00:43:56 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 12 Apr 2023 00:43:57 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 12 Apr 2023 00:43:57 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 12 Apr 2023 00:43:58 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 00:43:58 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 12 Apr 2023 00:43:59 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 12 Apr 2023 00:43:59 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 00:44:00 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 00:44:00 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 00:55:22 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 00:55:26 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 00:55:26 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 00:55:27 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 00:55:28 GMT
USER varnish
# Wed, 12 Apr 2023 00:55:28 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 00:55:29 GMT
CMD []
```

-	Layers:
	-	`sha256:5b41d5ec640939cf684959234ad3b80909268a32bfd520a31c6720a91521c2fa`  
		Last Modified: Wed, 12 Apr 2023 00:13:13 GMT  
		Size: 35.3 MB (35291995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a23cf789a1d6f1a8f615b2f894ff5d23dfc1871bec09bf4ddc25dfc2f51729`  
		Last Modified: Wed, 12 Apr 2023 01:17:31 GMT  
		Size: 70.8 MB (70783923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f561be54d7ea2acd53189c9a5ceccfe7bcc785342020b6d142e731caa7146a85`  
		Last Modified: Wed, 12 Apr 2023 01:17:14 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; s390x

```console
$ docker pull varnish@sha256:76dbe4d565daefa0520c378db042ff9df076dc427aeff7f5e5a18c7e7ab43c6c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.1 MB (87104431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61b1bdad50643f3f50c776b5b349fcd8bc3cde09b4bc391343f3a3d89d1bbe2f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:01:00 GMT
ADD file:b6463dba97ba9c0a29bacfafc4d67bc603ab57e80b75e23cd42d7ef4b0f8e6ae in / 
# Wed, 12 Apr 2023 00:01:04 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:44:24 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 12 Apr 2023 07:44:24 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 12 Apr 2023 07:44:24 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 12 Apr 2023 07:44:24 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 12 Apr 2023 07:44:24 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 12 Apr 2023 07:44:24 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 07:44:25 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 12 Apr 2023 07:44:25 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 12 Apr 2023 07:44:25 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 07:44:25 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 07:44:25 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 07:47:14 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 07:47:17 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 07:47:17 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 07:47:17 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 07:47:17 GMT
USER varnish
# Wed, 12 Apr 2023 07:47:18 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 07:47:18 GMT
CMD []
```

-	Layers:
	-	`sha256:97fe10bc7def58e7938e97e41eec4788ec7a45b6ef2cb1770cec02fa831fd19d`  
		Last Modified: Wed, 12 Apr 2023 00:05:18 GMT  
		Size: 29.7 MB (29653156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:975ac802e6432b31c2c91531f8f143c71a8109aab7895da564b25615d16f2901`  
		Last Modified: Wed, 12 Apr 2023 07:52:51 GMT  
		Size: 57.5 MB (57450785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2115594ecc7bff7e1220a85d4f39fd6717c6cbafa529e8652cee0c74f1abf3b`  
		Last Modified: Wed, 12 Apr 2023 07:52:44 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:fresh-alpine`

```console
$ docker pull varnish@sha256:1bcc61baae22531bd59b4f66ac0559b261907ca095d5eccf350ffb64f658c813
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
$ docker pull varnish@sha256:5d53f3cea335d15c3e518d4b4bd9ed6d9723e83a11cba3a0096e8dd81bb500a1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.4 MB (59350414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d8db36f71eea7cd47b1a6202cc8f6c57788e74b167c002c0f960e288cf7166e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:14:39 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Thu, 30 Mar 2023 02:14:39 GMT
ARG VARNISH_VERSION=7.3.0
# Thu, 30 Mar 2023 02:14:39 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Thu, 30 Mar 2023 02:14:39 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 30 Mar 2023 02:14:39 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 30 Mar 2023 02:14:39 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 02:14:39 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Thu, 30 Mar 2023 02:14:39 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Thu, 30 Mar 2023 02:14:39 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 02:14:40 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 02:14:40 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 02:16:00 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 02:16:00 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 02:16:00 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 02:16:01 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 02:16:01 GMT
USER varnish
# Thu, 30 Mar 2023 02:16:01 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 02:16:01 GMT
CMD []
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ecd0ddb0fcb995ea02ce3c7936dcb1d915a193f322ca158d7dad0631ac18af`  
		Last Modified: Thu, 30 Mar 2023 02:18:01 GMT  
		Size: 56.5 MB (56523322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7869007cb383d86d06b6b514b6d46fc40ac581add12bbbf143f319ba7a8e7015`  
		Last Modified: Thu, 30 Mar 2023 02:17:54 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:17ebddf73589304daba01e60bdc7bdb5bd09c4ec3a101619994a8c4d77fe4198
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45109401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c39e8bab4b3a15d6f7cb3d240b0f058d4044628947338dda3270ad223d1af8f4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 18:05:06 GMT
ADD file:0516b2e2d8a5c0a3e85e67a20375312bdc586a63094d779b9ac92517cf74a19d in / 
# Wed, 29 Mar 2023 18:05:06 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:10:33 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Thu, 30 Mar 2023 00:10:33 GMT
ARG VARNISH_VERSION=7.3.0
# Thu, 30 Mar 2023 00:10:33 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Thu, 30 Mar 2023 00:10:33 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 30 Mar 2023 00:10:33 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 30 Mar 2023 00:10:33 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 00:10:34 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Thu, 30 Mar 2023 00:10:34 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Thu, 30 Mar 2023 00:10:34 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 00:10:34 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 00:10:34 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 00:11:55 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 00:11:55 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 00:11:55 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 00:11:55 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 00:11:55 GMT
USER varnish
# Thu, 30 Mar 2023 00:11:55 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 00:11:55 GMT
CMD []
```

-	Layers:
	-	`sha256:fafb00bc68cf26e4a27ad2dce7303945ba9e40994e77c9269e610e0452ae9dce`  
		Last Modified: Wed, 29 Mar 2023 18:07:17 GMT  
		Size: 2.4 MB (2437606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f196af073038a0d6be5e1af91b28163c0eaca95c0243eac019991add8bb276`  
		Last Modified: Sat, 08 Apr 2023 02:40:45 GMT  
		Size: 42.7 MB (42671302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d483681d593a3936990d940c17cfe78497a6b081463653220e180980f80af780`  
		Last Modified: Sat, 08 Apr 2023 02:40:39 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:cdef2ee791f1fea0bb632e5fdbe7ab3d1dc08640e869ecbaad970af72cb62ed2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52090155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d26631d7414d095798d5e7800471d90767915486d8223cffd0d9a95dc9379d7a`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:53:56 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Thu, 30 Mar 2023 05:53:56 GMT
ARG VARNISH_VERSION=7.3.0
# Thu, 30 Mar 2023 05:53:56 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Thu, 30 Mar 2023 05:53:56 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 30 Mar 2023 05:53:56 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 30 Mar 2023 05:53:56 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 05:53:56 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Thu, 30 Mar 2023 05:53:56 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Thu, 30 Mar 2023 05:53:57 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 05:53:57 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 05:53:57 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 05:55:07 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 05:55:07 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 05:55:07 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 05:55:07 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 05:55:07 GMT
USER varnish
# Thu, 30 Mar 2023 05:55:07 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 05:55:07 GMT
CMD []
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50d982964542b8110c8924003584227b1310249ecd04ddd79df743a575bc925`  
		Last Modified: Thu, 30 Mar 2023 05:56:46 GMT  
		Size: 49.4 MB (49367657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12b6ca5add2e0d079fd385cac5fdbaa5864540dcd10b770e1548f117a90bd41`  
		Last Modified: Thu, 30 Mar 2023 05:56:40 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; 386

```console
$ docker pull varnish@sha256:f834ae921c56c3eb925d9bea6bc8e1ab80f60425be23ff96bb15cdba11930285
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59538735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ec87c585f44b8fefde94e4cb6f1eef3835e1db4c9686969169c7cd5dd6fb735`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 17:38:36 GMT
ADD file:fca96dde137b6b045359aec9d24257996738ac6cb7cce9518460a66802a27bd7 in / 
# Wed, 29 Mar 2023 17:38:36 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 01:33:46 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Thu, 30 Mar 2023 01:33:46 GMT
ARG VARNISH_VERSION=7.3.0
# Thu, 30 Mar 2023 01:33:46 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Thu, 30 Mar 2023 01:33:47 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 30 Mar 2023 01:33:47 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 30 Mar 2023 01:33:47 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 01:33:47 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Thu, 30 Mar 2023 01:33:47 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Thu, 30 Mar 2023 01:33:47 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 01:33:47 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 01:33:47 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 01:35:56 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 01:35:56 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 01:35:56 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 01:35:56 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 01:35:56 GMT
USER varnish
# Thu, 30 Mar 2023 01:35:56 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 01:35:57 GMT
CMD []
```

-	Layers:
	-	`sha256:333f5f619d7efe58316b2d71276f19d0a59bcb471f4dadaa85762b2c9e02775c`  
		Last Modified: Wed, 29 Mar 2023 17:39:19 GMT  
		Size: 2.8 MB (2832576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20da4d176e921bbb51748136a8fbf517d3cc60798e35724aebdd51ecf2b61ab6`  
		Last Modified: Thu, 30 Mar 2023 01:38:40 GMT  
		Size: 56.7 MB (56705662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a78548a60d6b9d7baf75051feb0fca2994834030bbc04a3645a4572a9757471`  
		Last Modified: Thu, 30 Mar 2023 01:38:30 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:909478b58a275ec2ab8a14120cc9591ebbbdff86f860ea8df1485ae2c264e488
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49136000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d067fd63b0dd3bfee0cefb4eaba611ad41e8cfecb8b2c16ada69e7e227fcb7b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 18:16:40 GMT
ADD file:3c2a8d553fa0998f13f86592f104a9a4ad14f8db46dfa9145c8fbbca0b87ee9a in / 
# Wed, 29 Mar 2023 18:16:40 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:33:21 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Thu, 30 Mar 2023 04:33:22 GMT
ARG VARNISH_VERSION=7.3.0
# Thu, 30 Mar 2023 04:33:22 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Thu, 30 Mar 2023 04:33:22 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 30 Mar 2023 04:33:23 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 30 Mar 2023 04:33:23 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 04:33:23 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Thu, 30 Mar 2023 04:33:23 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Thu, 30 Mar 2023 04:33:24 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 04:33:24 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 04:33:24 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 04:35:35 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 04:35:37 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 04:35:37 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 04:35:37 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 04:35:38 GMT
USER varnish
# Thu, 30 Mar 2023 04:35:38 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 04:35:38 GMT
CMD []
```

-	Layers:
	-	`sha256:0b40b0bd0da3095d93bf74233a1d0bf638b2511fee461df8f6a71aad5a038589`  
		Last Modified: Wed, 29 Mar 2023 18:17:38 GMT  
		Size: 2.8 MB (2813760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5980c95097dfced199688de3f6aa45cd2216bfddef048561966b6608945af2f0`  
		Last Modified: Thu, 30 Mar 2023 04:38:24 GMT  
		Size: 46.3 MB (46321744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690ae6fe9c6e1be629171f54ae05b866b6572efa3b1d22692d741929e7d11bb7`  
		Last Modified: Thu, 30 Mar 2023 04:38:12 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:2fabb6c5fa95ead9711c9785ebab43a38eacb02b418775d6b5ab1a73fa8acc8f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47598984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63eb61c9640b3da92089de86d78ac057c997e5d877f757120cda472c896b941e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 17:42:07 GMT
ADD file:5cf392863cd9a0735de88f9e7dab93c9e74aca59ca05b792943cf3b621ea2c59 in / 
# Wed, 29 Mar 2023 17:42:07 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 23:08:14 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 29 Mar 2023 23:08:14 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 29 Mar 2023 23:08:14 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 29 Mar 2023 23:08:14 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 29 Mar 2023 23:08:14 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 29 Mar 2023 23:08:14 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 29 Mar 2023 23:08:14 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 29 Mar 2023 23:08:15 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 29 Mar 2023 23:08:15 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 29 Mar 2023 23:08:15 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Wed, 29 Mar 2023 23:08:15 GMT
ENV VARNISH_SIZE=100M
# Wed, 29 Mar 2023 23:09:46 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Wed, 29 Mar 2023 23:09:47 GMT
WORKDIR /etc/varnish
# Wed, 29 Mar 2023 23:09:47 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 29 Mar 2023 23:09:48 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 29 Mar 2023 23:09:48 GMT
USER varnish
# Wed, 29 Mar 2023 23:09:48 GMT
EXPOSE 80 8443
# Wed, 29 Mar 2023 23:09:48 GMT
CMD []
```

-	Layers:
	-	`sha256:1536575ac9c5f5fff4522c60d4610af0a52be584c36e652080c6c0ad169d4f27`  
		Last Modified: Wed, 29 Mar 2023 17:42:42 GMT  
		Size: 2.6 MB (2610636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dadb2417c7920374afa7798d98c70d2f0a8290f641bb3dbc112a2158ac097a2d`  
		Last Modified: Wed, 29 Mar 2023 23:12:02 GMT  
		Size: 45.0 MB (44987850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a556b2e0ae2040be8338c713604078ac74fa7ec335f48fff28337d8b007e52`  
		Last Modified: Wed, 29 Mar 2023 23:11:56 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:latest`

```console
$ docker pull varnish@sha256:d50f601a76ff2cefca6afa7587c75dc46ad482b7734baab89eaf79a6516c90f4
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
$ docker pull varnish@sha256:01c1f0ee2a532a0f480fa00e8b754c2a1662ab5989e3958d966222ed09f95d02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106805687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38f8fe02f4ba954dfed4760af3cb20e716fb19e427144a743bb942eca093bd75`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:35:52 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 12 Apr 2023 07:35:52 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 12 Apr 2023 07:35:52 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 12 Apr 2023 07:35:52 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 12 Apr 2023 07:35:52 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 12 Apr 2023 07:35:52 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 07:35:52 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 12 Apr 2023 07:35:52 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 12 Apr 2023 07:35:52 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 07:35:52 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 07:35:53 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 07:38:58 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 07:38:58 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 07:38:59 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 07:38:59 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 07:38:59 GMT
USER varnish
# Wed, 12 Apr 2023 07:38:59 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 07:38:59 GMT
CMD []
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c1be847abb1fb38853dbae20352d1f2e2b780db54e88fbb737549a5aab7a79`  
		Last Modified: Wed, 12 Apr 2023 07:44:41 GMT  
		Size: 75.4 MB (75386967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb31db21e143ba8b279a4dc67a859edafd358e53f1efdbe4ac92744d507f6ddd`  
		Last Modified: Wed, 12 Apr 2023 07:44:32 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; arm variant v7

```console
$ docker pull varnish@sha256:ee2c275680aed583fea7ceba04074e69fda8c8747dbd68766d2e0d9c55512f03
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.1 MB (83149297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7730d361798ab6943823a20c73d9f1bee65ccfe1300978e219422823cbce78b9`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 11 Apr 2023 23:59:44 GMT
ADD file:e5f4777456ed4424053e9aa1f3d783f57da094c7a6c6d9d7a2fd315e00b5bbb0 in / 
# Tue, 11 Apr 2023 23:59:44 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 09:48:46 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 12 Apr 2023 09:48:47 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 12 Apr 2023 09:48:47 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 12 Apr 2023 09:48:47 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 12 Apr 2023 09:48:47 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 12 Apr 2023 09:48:48 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 09:48:48 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 12 Apr 2023 09:48:48 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 12 Apr 2023 09:48:48 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 09:48:49 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 09:48:49 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 09:52:44 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 09:52:44 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 09:52:44 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 09:52:45 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 09:52:45 GMT
USER varnish
# Wed, 12 Apr 2023 09:52:45 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 09:52:45 GMT
CMD []
```

-	Layers:
	-	`sha256:99c2a28b4a43ce341eb611e82106b886315f30a250473617f2293828e10d8fff`  
		Last Modified: Wed, 12 Apr 2023 00:03:19 GMT  
		Size: 26.6 MB (26579772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:946f48177dd61e98fafd1f5db674994ba0ad766c7b50f4b06c552e129d2be463`  
		Last Modified: Wed, 12 Apr 2023 09:57:58 GMT  
		Size: 56.6 MB (56569036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c94d0d1168a78363c629071b130cf202012a5c2285cff907fbe05f9f7d3166e2`  
		Last Modified: Wed, 12 Apr 2023 09:57:50 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:02ef5b0996ff812c54abd99265f8b339cd393d1be211f3cc646f918ffd4bea02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100589822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:036a0598d94c3d082574590889afad8344a4b710a2705cc884c821afd482967e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 04:45:29 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 12 Apr 2023 04:45:29 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 12 Apr 2023 04:45:29 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 12 Apr 2023 04:45:29 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 12 Apr 2023 04:45:29 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 12 Apr 2023 04:45:29 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 04:45:29 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 12 Apr 2023 04:45:29 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 12 Apr 2023 04:45:30 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 04:45:30 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 04:45:30 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 04:48:22 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 04:48:23 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 04:48:23 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:48:23 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 04:48:23 GMT
USER varnish
# Wed, 12 Apr 2023 04:48:23 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 04:48:23 GMT
CMD []
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b6030c7f52818939f055e2f6663b1b9cc13fd7547b1c2e0f753f5b87cd93ca`  
		Last Modified: Wed, 12 Apr 2023 04:53:10 GMT  
		Size: 70.5 MB (70525505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74565242087dac611bbba86cb8a4ef8aa9aa3712f40e4ab8949602813f427c6b`  
		Last Modified: Wed, 12 Apr 2023 04:53:03 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; 386

```console
$ docker pull varnish@sha256:88f2d7b6250c7d29544a99d128dc2aafe14c362633b4ff697b2720611c261141
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.2 MB (108173601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bfc3f953767b14e681b22c82c947846dedc22c394cd082cea401378516935b4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:39:01 GMT
ADD file:42fc1b4536cdd6823499b0c94d799e9bfbcb280b7df55d8d6c9f6defd61ecb6e in / 
# Wed, 12 Apr 2023 00:39:01 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 04:13:43 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 12 Apr 2023 04:13:44 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 12 Apr 2023 04:13:44 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 12 Apr 2023 04:13:44 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 12 Apr 2023 04:13:44 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 12 Apr 2023 04:13:44 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 04:13:44 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 12 Apr 2023 04:13:44 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 12 Apr 2023 04:13:44 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 04:13:44 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 04:13:44 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 04:18:07 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 04:18:08 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 04:18:08 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:18:08 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 04:18:08 GMT
USER varnish
# Wed, 12 Apr 2023 04:18:08 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 04:18:08 GMT
CMD []
```

-	Layers:
	-	`sha256:b2ee1f87789d52ef09851b4e5c9745fb8aceafa107b0d3452f9973f1abe65042`  
		Last Modified: Wed, 12 Apr 2023 00:42:45 GMT  
		Size: 32.4 MB (32398925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee5e7f863a0627e32c4308f8e477d218c74b26149178e5f23057f2339a55e64`  
		Last Modified: Wed, 12 Apr 2023 04:25:03 GMT  
		Size: 75.8 MB (75774186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c73471ce047c640427aa8d168e423ce9d464179d283e9ecc90c6dca784deef`  
		Last Modified: Wed, 12 Apr 2023 04:24:49 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; ppc64le

```console
$ docker pull varnish@sha256:99a9dcf0cddca561abbcd5bc5b002adbb083de964d8746e3063cab564573c331
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.1 MB (106076410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e817121269101ae25eb3c824355809f156a4e72be8a908710817a5575d2fb848`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:08:20 GMT
ADD file:63eb52aaff02c15bceabb87a78eb1b36389066ff4774cf8a754160ca7d509816 in / 
# Wed, 12 Apr 2023 00:08:23 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:43:55 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 12 Apr 2023 00:43:56 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 12 Apr 2023 00:43:56 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 12 Apr 2023 00:43:57 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 12 Apr 2023 00:43:57 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 12 Apr 2023 00:43:58 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 00:43:58 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 12 Apr 2023 00:43:59 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 12 Apr 2023 00:43:59 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 00:44:00 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 00:44:00 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 00:55:22 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 00:55:26 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 00:55:26 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 00:55:27 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 00:55:28 GMT
USER varnish
# Wed, 12 Apr 2023 00:55:28 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 00:55:29 GMT
CMD []
```

-	Layers:
	-	`sha256:5b41d5ec640939cf684959234ad3b80909268a32bfd520a31c6720a91521c2fa`  
		Last Modified: Wed, 12 Apr 2023 00:13:13 GMT  
		Size: 35.3 MB (35291995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a23cf789a1d6f1a8f615b2f894ff5d23dfc1871bec09bf4ddc25dfc2f51729`  
		Last Modified: Wed, 12 Apr 2023 01:17:31 GMT  
		Size: 70.8 MB (70783923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f561be54d7ea2acd53189c9a5ceccfe7bcc785342020b6d142e731caa7146a85`  
		Last Modified: Wed, 12 Apr 2023 01:17:14 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; s390x

```console
$ docker pull varnish@sha256:76dbe4d565daefa0520c378db042ff9df076dc427aeff7f5e5a18c7e7ab43c6c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.1 MB (87104431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61b1bdad50643f3f50c776b5b349fcd8bc3cde09b4bc391343f3a3d89d1bbe2f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:01:00 GMT
ADD file:b6463dba97ba9c0a29bacfafc4d67bc603ab57e80b75e23cd42d7ef4b0f8e6ae in / 
# Wed, 12 Apr 2023 00:01:04 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:44:24 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 12 Apr 2023 07:44:24 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 12 Apr 2023 07:44:24 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 12 Apr 2023 07:44:24 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 12 Apr 2023 07:44:24 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 12 Apr 2023 07:44:24 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 07:44:25 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 12 Apr 2023 07:44:25 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 12 Apr 2023 07:44:25 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 07:44:25 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 07:44:25 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 07:47:14 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 07:47:17 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 07:47:17 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 07:47:17 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 07:47:17 GMT
USER varnish
# Wed, 12 Apr 2023 07:47:18 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 07:47:18 GMT
CMD []
```

-	Layers:
	-	`sha256:97fe10bc7def58e7938e97e41eec4788ec7a45b6ef2cb1770cec02fa831fd19d`  
		Last Modified: Wed, 12 Apr 2023 00:05:18 GMT  
		Size: 29.7 MB (29653156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:975ac802e6432b31c2c91531f8f143c71a8109aab7895da564b25615d16f2901`  
		Last Modified: Wed, 12 Apr 2023 07:52:51 GMT  
		Size: 57.5 MB (57450785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2115594ecc7bff7e1220a85d4f39fd6717c6cbafa529e8652cee0c74f1abf3b`  
		Last Modified: Wed, 12 Apr 2023 07:52:44 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:old`

```console
$ docker pull varnish@sha256:28b9207d49c4e302fc86546b7d45ea4d9e6b5422cc77cb49f51be275d864b039
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
$ docker pull varnish@sha256:dfb97568859cbd5e3b745a67668df23a1ceca18eb292218d9871d52954805d99
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106849839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e192e3d65e5429e6f2a7f23281c3cf04d43217560b3c01e47dd8654ab470e545`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:39:16 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Wed, 12 Apr 2023 07:39:16 GMT
ARG VARNISH_VERSION=7.2.1
# Wed, 12 Apr 2023 07:39:16 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Wed, 12 Apr 2023 07:39:17 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Wed, 12 Apr 2023 07:39:17 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Wed, 12 Apr 2023 07:39:17 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 07:39:17 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Wed, 12 Apr 2023 07:39:17 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Wed, 12 Apr 2023 07:39:17 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 07:39:17 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 07:39:17 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 07:41:53 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 07:41:54 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 07:41:54 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 07:41:54 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 07:41:54 GMT
USER varnish
# Wed, 12 Apr 2023 07:41:54 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 07:41:54 GMT
CMD []
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c968e0ee4a730130252480debde7124ca86d34f741bf51571a5a29a5ba34693c`  
		Last Modified: Wed, 12 Apr 2023 07:45:05 GMT  
		Size: 75.4 MB (75431120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25daa5e6ca914814a8155ca526ce4bb0b71741603e1898c2e87ec69bd20c5ab0`  
		Last Modified: Wed, 12 Apr 2023 07:44:55 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; arm variant v7

```console
$ docker pull varnish@sha256:c244a05033959bcfd06dad6e9bb4c15405ca97412a35d196aa7288a8d0b98865
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.2 MB (83190520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18f4f1a4a71ea168baeb1694ae369389fda214c037ea35ff0165991f0abe556d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 11 Apr 2023 23:59:44 GMT
ADD file:e5f4777456ed4424053e9aa1f3d783f57da094c7a6c6d9d7a2fd315e00b5bbb0 in / 
# Tue, 11 Apr 2023 23:59:44 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 09:52:54 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Wed, 12 Apr 2023 09:52:54 GMT
ARG VARNISH_VERSION=7.2.1
# Wed, 12 Apr 2023 09:52:54 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Wed, 12 Apr 2023 09:52:55 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Wed, 12 Apr 2023 09:52:55 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Wed, 12 Apr 2023 09:52:55 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 09:52:55 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Wed, 12 Apr 2023 09:52:55 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Wed, 12 Apr 2023 09:52:55 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 09:52:55 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 09:52:55 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 09:55:29 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 09:55:29 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 09:55:29 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 09:55:29 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 09:55:29 GMT
USER varnish
# Wed, 12 Apr 2023 09:55:29 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 09:55:29 GMT
CMD []
```

-	Layers:
	-	`sha256:99c2a28b4a43ce341eb611e82106b886315f30a250473617f2293828e10d8fff`  
		Last Modified: Wed, 12 Apr 2023 00:03:19 GMT  
		Size: 26.6 MB (26579772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02c3bf9e9ab14cb00f2a7b32fd61f0dc7f58385c6b36746b7a28d8db143af093`  
		Last Modified: Wed, 12 Apr 2023 09:58:19 GMT  
		Size: 56.6 MB (56610256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3f12a5b2f13f28364d239561b484e09aab0533fa4291c2ec7c6fb72ae6dbe3`  
		Last Modified: Wed, 12 Apr 2023 09:58:10 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:c7c5b44d1b649b8e18f2fa02e3ac6cfbe1219629ee51fb0c297f2ad9d340835c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.9 MB (100869468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:064d1446bbe323f8a5118936bc056bec5669a4efea357a44b0250aefebce979f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 04:48:37 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Wed, 12 Apr 2023 04:48:38 GMT
ARG VARNISH_VERSION=7.2.1
# Wed, 12 Apr 2023 04:48:38 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Wed, 12 Apr 2023 04:48:38 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Wed, 12 Apr 2023 04:48:38 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Wed, 12 Apr 2023 04:48:38 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 04:48:38 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Wed, 12 Apr 2023 04:48:38 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Wed, 12 Apr 2023 04:48:38 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 04:48:38 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 04:48:38 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 04:50:57 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 04:50:57 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 04:50:57 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:50:57 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 04:50:58 GMT
USER varnish
# Wed, 12 Apr 2023 04:50:58 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 04:50:58 GMT
CMD []
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd387399b52bcda6a293afa412dc3c7ffe5106e36f6820bbfe7b36cfe9c84ce6`  
		Last Modified: Wed, 12 Apr 2023 04:53:31 GMT  
		Size: 70.8 MB (70805151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717900fa7e49b8851eb8e3cc5cb7174be8ba02fa5fae4efc1d5889369dc19982`  
		Last Modified: Wed, 12 Apr 2023 04:53:24 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; 386

```console
$ docker pull varnish@sha256:132d16358cb9c81ea691480e6340bafa5db22839213c2608eb00bb1c2e318778
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.2 MB (108229812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:701dd3cc6e511fd1e6a0ccb05404b60373851c1f0318dd8035b6526b81707c28`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:39:01 GMT
ADD file:42fc1b4536cdd6823499b0c94d799e9bfbcb280b7df55d8d6c9f6defd61ecb6e in / 
# Wed, 12 Apr 2023 00:39:01 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 04:18:22 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Wed, 12 Apr 2023 04:18:22 GMT
ARG VARNISH_VERSION=7.2.1
# Wed, 12 Apr 2023 04:18:22 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Wed, 12 Apr 2023 04:18:22 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Wed, 12 Apr 2023 04:18:23 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Wed, 12 Apr 2023 04:18:23 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 04:18:23 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Wed, 12 Apr 2023 04:18:23 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Wed, 12 Apr 2023 04:18:23 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 04:18:23 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 04:18:23 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 04:21:46 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 04:21:46 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 04:21:47 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:21:47 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 04:21:47 GMT
USER varnish
# Wed, 12 Apr 2023 04:21:47 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 04:21:47 GMT
CMD []
```

-	Layers:
	-	`sha256:b2ee1f87789d52ef09851b4e5c9745fb8aceafa107b0d3452f9973f1abe65042`  
		Last Modified: Wed, 12 Apr 2023 00:42:45 GMT  
		Size: 32.4 MB (32398925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a639361d9918a14ff82f7bba72feea5809b05f1c6a1c6da01ac194a148379e2`  
		Last Modified: Wed, 12 Apr 2023 04:25:29 GMT  
		Size: 75.8 MB (75830396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e95964f0144157e5774aa830935fc68f7bf5b0a1834e27bc6272d49816484fda`  
		Last Modified: Wed, 12 Apr 2023 04:25:15 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; ppc64le

```console
$ docker pull varnish@sha256:2ddbd11558d86d08b3f82a25da574d70734fed468550edb4d6b957cf2fc4ff55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.1 MB (106112382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fcc671da9acaf8ae312a5ba85fd3d77e7e1b88a900054ac23433f6dad4b7cde`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:08:20 GMT
ADD file:63eb52aaff02c15bceabb87a78eb1b36389066ff4774cf8a754160ca7d509816 in / 
# Wed, 12 Apr 2023 00:08:23 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:55:40 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Wed, 12 Apr 2023 00:55:40 GMT
ARG VARNISH_VERSION=7.2.1
# Wed, 12 Apr 2023 00:55:41 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Wed, 12 Apr 2023 00:55:41 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Wed, 12 Apr 2023 00:55:42 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Wed, 12 Apr 2023 00:55:42 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 00:55:43 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Wed, 12 Apr 2023 00:55:44 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Wed, 12 Apr 2023 00:55:44 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 00:55:45 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 00:55:45 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 01:06:37 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 01:06:41 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 01:06:41 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 01:06:42 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 01:06:43 GMT
USER varnish
# Wed, 12 Apr 2023 01:06:43 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 01:06:45 GMT
CMD []
```

-	Layers:
	-	`sha256:5b41d5ec640939cf684959234ad3b80909268a32bfd520a31c6720a91521c2fa`  
		Last Modified: Wed, 12 Apr 2023 00:13:13 GMT  
		Size: 35.3 MB (35291995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4a89d7f741d3117b0ee6c2f7194da63a2eb7e31a212514121c21a0f9a2d56d`  
		Last Modified: Wed, 12 Apr 2023 01:18:03 GMT  
		Size: 70.8 MB (70819898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3fec9bc4ead77e694d7ee941f4809ba1dc75a4379c2e14982a287a907f61d2`  
		Last Modified: Wed, 12 Apr 2023 01:17:46 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; s390x

```console
$ docker pull varnish@sha256:8e03fc4febcb1085c13e0d907ca56a70bd0a5015b6001b7575deddb067700889
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.1 MB (87145481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae5308c0a1d01c5120da7ddc51e7161062bf73b4fe635935570d47dce15b4888`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:01:00 GMT
ADD file:b6463dba97ba9c0a29bacfafc4d67bc603ab57e80b75e23cd42d7ef4b0f8e6ae in / 
# Wed, 12 Apr 2023 00:01:04 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:47:32 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Wed, 12 Apr 2023 07:47:32 GMT
ARG VARNISH_VERSION=7.2.1
# Wed, 12 Apr 2023 07:47:32 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Wed, 12 Apr 2023 07:47:32 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Wed, 12 Apr 2023 07:47:32 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Wed, 12 Apr 2023 07:47:32 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 07:47:32 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Wed, 12 Apr 2023 07:47:33 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Wed, 12 Apr 2023 07:47:33 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 07:47:33 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 07:47:33 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 07:50:04 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 07:50:08 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 07:50:08 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 07:50:08 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 07:50:08 GMT
USER varnish
# Wed, 12 Apr 2023 07:50:08 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 07:50:08 GMT
CMD []
```

-	Layers:
	-	`sha256:97fe10bc7def58e7938e97e41eec4788ec7a45b6ef2cb1770cec02fa831fd19d`  
		Last Modified: Wed, 12 Apr 2023 00:05:18 GMT  
		Size: 29.7 MB (29653156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6c0378159be2b47ba02173837a0605e110437dd56ebde55c1b33b16e3a64c1`  
		Last Modified: Wed, 12 Apr 2023 07:53:06 GMT  
		Size: 57.5 MB (57491834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b0aa3c751db4a00420dc9624ea76c92014f9ff8e7975d01d47e5bf3743531c`  
		Last Modified: Wed, 12 Apr 2023 07:52:59 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:old-alpine`

```console
$ docker pull varnish@sha256:4afc17b0aa7c483b822ae0c548f93d87fdcfc38715e30734657bad8a3171f534
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
$ docker pull varnish@sha256:a320ad063c3556dfea1308e7747a7b74de2e6580bb136653f10480b192d2b7ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.4 MB (59399546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:619a779899e4b887658162b42b9f51b181570836a20e93eabacd1c0634421c23`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:16:18 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 30 Mar 2023 02:16:18 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 30 Mar 2023 02:16:18 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 30 Mar 2023 02:16:19 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 30 Mar 2023 02:16:19 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 30 Mar 2023 02:16:19 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 02:16:19 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 30 Mar 2023 02:16:19 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 30 Mar 2023 02:16:19 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 02:16:19 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 02:16:19 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 02:17:35 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 02:17:35 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 02:17:35 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 02:17:35 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 02:17:35 GMT
USER varnish
# Thu, 30 Mar 2023 02:17:35 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 02:17:36 GMT
CMD []
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c114fe4204a2c955105dd5cd8a42a772594a1642947fbefba511406b0e60e5`  
		Last Modified: Thu, 30 Mar 2023 02:18:20 GMT  
		Size: 56.6 MB (56572454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debea196e0761731bed241b5b0124d7dab6070192ebf9f49532117ef228a4fd7`  
		Last Modified: Thu, 30 Mar 2023 02:18:13 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:fccf7f20e1622e5cc7de9c8a0374d530f4ce08e15bae3fa806e6c5f34100a250
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45148202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31ac3c9362d31494b1482831d5f9600db9a9423084b5bcdfb6bf502d29be4134`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 18:05:06 GMT
ADD file:0516b2e2d8a5c0a3e85e67a20375312bdc586a63094d779b9ac92517cf74a19d in / 
# Wed, 29 Mar 2023 18:05:06 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:16:02 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 30 Mar 2023 00:16:02 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 30 Mar 2023 00:16:02 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 30 Mar 2023 00:16:02 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 30 Mar 2023 00:16:02 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 30 Mar 2023 00:16:02 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 00:16:02 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 30 Mar 2023 00:16:03 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 30 Mar 2023 00:16:03 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 00:16:03 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 00:16:03 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 00:17:15 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 00:17:16 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 00:17:16 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 00:17:16 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 00:17:16 GMT
USER varnish
# Thu, 30 Mar 2023 00:17:16 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 00:17:16 GMT
CMD []
```

-	Layers:
	-	`sha256:fafb00bc68cf26e4a27ad2dce7303945ba9e40994e77c9269e610e0452ae9dce`  
		Last Modified: Wed, 29 Mar 2023 18:07:17 GMT  
		Size: 2.4 MB (2437606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7ec1086689ab0fd73293e70d501d454a27eb5ea261d03a2430cb0d14696427`  
		Last Modified: Sat, 08 Apr 2023 02:41:03 GMT  
		Size: 42.7 MB (42710102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9ac18a355d90f33336fbada96e19569338d541feae42ae2d313ce006609bb1`  
		Last Modified: Sat, 08 Apr 2023 02:40:57 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:4b01c566b91d765af9c55ca58772d6926b481ba4c60bfe7b9d6b0adca255f10b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52139702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3552cf8b859208887e19e7d4ff64ae304e14cf411f5dadeb80d6c52b607f72d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:55:19 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 30 Mar 2023 05:55:20 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 30 Mar 2023 05:55:20 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 30 Mar 2023 05:55:20 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 30 Mar 2023 05:55:20 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 30 Mar 2023 05:55:20 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 05:55:20 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 30 Mar 2023 05:55:20 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 30 Mar 2023 05:55:20 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 05:55:20 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 05:55:20 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 05:56:25 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 05:56:25 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 05:56:25 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 05:56:26 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 05:56:26 GMT
USER varnish
# Thu, 30 Mar 2023 05:56:26 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 05:56:26 GMT
CMD []
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c53d05c94805192159ec306400f8402f101647b10b4f2862a4b9cafe6d9ea95`  
		Last Modified: Thu, 30 Mar 2023 05:57:04 GMT  
		Size: 49.4 MB (49417204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dfbbc1899969f2944b32d817962c27670200b641a7ff5b382026a2a6f1e91f8`  
		Last Modified: Thu, 30 Mar 2023 05:56:58 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; 386

```console
$ docker pull varnish@sha256:b4aed57dfb69759cbbf97f8251f733ed209e5377c0b138e878768446cf3f1012
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.6 MB (59579474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb2d5054f0237342f09e7c81d57f5b91b2a7258c98c54862bcd60b70f213eff4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 17:38:36 GMT
ADD file:fca96dde137b6b045359aec9d24257996738ac6cb7cce9518460a66802a27bd7 in / 
# Wed, 29 Mar 2023 17:38:36 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 01:36:10 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 30 Mar 2023 01:36:10 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 30 Mar 2023 01:36:10 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 30 Mar 2023 01:36:10 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 30 Mar 2023 01:36:10 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 30 Mar 2023 01:36:10 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 01:36:10 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 30 Mar 2023 01:36:10 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 30 Mar 2023 01:36:11 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 01:36:11 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 01:36:11 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 01:38:03 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 01:38:03 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 01:38:03 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 01:38:03 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 01:38:03 GMT
USER varnish
# Thu, 30 Mar 2023 01:38:04 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 01:38:04 GMT
CMD []
```

-	Layers:
	-	`sha256:333f5f619d7efe58316b2d71276f19d0a59bcb471f4dadaa85762b2c9e02775c`  
		Last Modified: Wed, 29 Mar 2023 17:39:19 GMT  
		Size: 2.8 MB (2832576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec17ca4c36e5d196286fcd4f66f0a6879ff35841617edc48c24a2b0d3fed6c5`  
		Last Modified: Thu, 30 Mar 2023 01:39:02 GMT  
		Size: 56.7 MB (56746401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3acb1c0b2cc2ca1f40568c89f6ace8d204192474b0b299f6afbd1d5b87c89ad4`  
		Last Modified: Thu, 30 Mar 2023 01:38:52 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:47175a4b9a3d7cc10400bda61c20d308651152bf93f3268aa3b4c850c4cebb3c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49172829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe520b41ef8593a0ca87c4b15e445248e7728729026968d7c7167a33b40a8e28`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 18:16:40 GMT
ADD file:3c2a8d553fa0998f13f86592f104a9a4ad14f8db46dfa9145c8fbbca0b87ee9a in / 
# Wed, 29 Mar 2023 18:16:40 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:35:48 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 30 Mar 2023 04:35:48 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 30 Mar 2023 04:35:49 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 30 Mar 2023 04:35:49 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 30 Mar 2023 04:35:49 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 30 Mar 2023 04:35:50 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 30 Mar 2023 04:35:50 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 30 Mar 2023 04:35:50 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 30 Mar 2023 04:35:51 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 30 Mar 2023 04:35:51 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Thu, 30 Mar 2023 04:35:51 GMT
ENV VARNISH_SIZE=100M
# Thu, 30 Mar 2023 04:37:42 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 30 Mar 2023 04:37:43 GMT
WORKDIR /etc/varnish
# Thu, 30 Mar 2023 04:37:44 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 30 Mar 2023 04:37:44 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 30 Mar 2023 04:37:44 GMT
USER varnish
# Thu, 30 Mar 2023 04:37:45 GMT
EXPOSE 80 8443
# Thu, 30 Mar 2023 04:37:45 GMT
CMD []
```

-	Layers:
	-	`sha256:0b40b0bd0da3095d93bf74233a1d0bf638b2511fee461df8f6a71aad5a038589`  
		Last Modified: Wed, 29 Mar 2023 18:17:38 GMT  
		Size: 2.8 MB (2813760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69361e01f667423c0f2d961984f6e7db1a81226574e2f2e13b25de56a1ed714d`  
		Last Modified: Thu, 30 Mar 2023 04:38:48 GMT  
		Size: 46.4 MB (46358574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b033b092d98a898fd606406859a2bdc093c0babde613a26ed82fff5736c9290`  
		Last Modified: Thu, 30 Mar 2023 04:38:37 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:cae32a9f29cd9997a1fe2ee6f8d0b8e3ff91c21e6213716d9ac34675317dc70d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47646967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e24f77bba538e7715318a014e47a2ab4183cd521c07f85ecc3a82ab13ed2830`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 29 Mar 2023 17:42:07 GMT
ADD file:5cf392863cd9a0735de88f9e7dab93c9e74aca59ca05b792943cf3b621ea2c59 in / 
# Wed, 29 Mar 2023 17:42:07 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 23:10:06 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Wed, 29 Mar 2023 23:10:06 GMT
ARG VARNISH_VERSION=7.2.1
# Wed, 29 Mar 2023 23:10:06 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Wed, 29 Mar 2023 23:10:06 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Wed, 29 Mar 2023 23:10:06 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Wed, 29 Mar 2023 23:10:06 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 29 Mar 2023 23:10:06 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Wed, 29 Mar 2023 23:10:06 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Wed, 29 Mar 2023 23:10:07 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 29 Mar 2023 23:10:07 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Wed, 29 Mar 2023 23:10:07 GMT
ENV VARNISH_SIZE=100M
# Wed, 29 Mar 2023 23:11:26 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Wed, 29 Mar 2023 23:11:28 GMT
WORKDIR /etc/varnish
# Wed, 29 Mar 2023 23:11:28 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 29 Mar 2023 23:11:28 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 29 Mar 2023 23:11:28 GMT
USER varnish
# Wed, 29 Mar 2023 23:11:28 GMT
EXPOSE 80 8443
# Wed, 29 Mar 2023 23:11:28 GMT
CMD []
```

-	Layers:
	-	`sha256:1536575ac9c5f5fff4522c60d4610af0a52be584c36e652080c6c0ad169d4f27`  
		Last Modified: Wed, 29 Mar 2023 17:42:42 GMT  
		Size: 2.6 MB (2610636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091447cbd58b57bbe1eb2edf62b5e2d9c06467104aebfc70c02d7cfafa01868c`  
		Last Modified: Wed, 29 Mar 2023 23:12:17 GMT  
		Size: 45.0 MB (45035834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390574d541f53e2036c226ec79255c18a2429053de04847092de875c4925890b`  
		Last Modified: Wed, 29 Mar 2023 23:12:12 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:stable`

```console
$ docker pull varnish@sha256:0e992a9c53300db59932059504d8df94b965ddf0c0db2a47c8bc83029b93f67e
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
$ docker pull varnish@sha256:f593b51393e4edffa20e5bb0fcfeef6bf09dd71a6ecd254ef9a055448e39d9ef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100660685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f821874ee374fc2690cc271a857a80cd79f288fa99c09daa13296016f8c6bc93`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:42:11 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 07:44:11 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 12 Apr 2023 07:44:11 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 07:44:11 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 12 Apr 2023 07:44:11 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 07:44:11 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 07:44:11 GMT
CMD []
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274c9ddef5cd48e2463d6b5bc111d79368c0f10f6a1040041952253bde9de5d8`  
		Last Modified: Wed, 12 Apr 2023 07:45:24 GMT  
		Size: 69.2 MB (69241757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d351ea0dbe4d60c605b1dc412d644d729517137393f865e66240a64582514b7e`  
		Last Modified: Wed, 12 Apr 2023 07:45:15 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; arm variant v7

```console
$ docker pull varnish@sha256:1eaf25f8067fb7f5f24129515c2d6043b571f15d7cb9b4f3082775fdebecbf4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77230907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b4d723caf3307762828942958dc505a55bb9d17a6a45d3a26652aa88fcabf4b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 11 Apr 2023 23:59:44 GMT
ADD file:e5f4777456ed4424053e9aa1f3d783f57da094c7a6c6d9d7a2fd315e00b5bbb0 in / 
# Tue, 11 Apr 2023 23:59:44 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 09:55:33 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 09:57:38 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 12 Apr 2023 09:57:38 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 09:57:38 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 12 Apr 2023 09:57:39 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 09:57:39 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 09:57:39 GMT
CMD []
```

-	Layers:
	-	`sha256:99c2a28b4a43ce341eb611e82106b886315f30a250473617f2293828e10d8fff`  
		Last Modified: Wed, 12 Apr 2023 00:03:19 GMT  
		Size: 26.6 MB (26579772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529f9895b0f9e006c21d373370b249b754e53c9c65c36ac74a7d119107e866d3`  
		Last Modified: Wed, 12 Apr 2023 09:58:37 GMT  
		Size: 50.7 MB (50650437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3dec06d3bbb4fa400129ccde514435125382ce56882357ccaac867c7ec5946c`  
		Last Modified: Wed, 12 Apr 2023 09:58:28 GMT  
		Size: 698.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:4497b8996cff43dd8a560c68964fe29e13a8db946473a82376e209dc0810beee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94717057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:007c8e618536b021221201d9958b4cd97558922fa549482bda3875fc2066dbcf`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 04:51:01 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 04:52:43 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 12 Apr 2023 04:52:44 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 04:52:44 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:52:44 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 04:52:44 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 04:52:44 GMT
CMD []
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:682527444ab1be7526396ac0bbb4f292068e8474d19254d67e495ea8f451be15`  
		Last Modified: Wed, 12 Apr 2023 04:53:48 GMT  
		Size: 64.7 MB (64652529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3454f24f83fdb3c9d4943c12fa0e06a0eeefe8b0012e9a5cae6dfcd89951dc1`  
		Last Modified: Wed, 12 Apr 2023 04:53:42 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; 386

```console
$ docker pull varnish@sha256:e3ae418f25ec73834e468b452e5b23e4d982b9cdcc0bdacaada801c58d054ba7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102083639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9c15e2d6a853229156a560e293584edb697596ab5e92252ab7b3a8f610c8a2b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:39:01 GMT
ADD file:42fc1b4536cdd6823499b0c94d799e9bfbcb280b7df55d8d6c9f6defd61ecb6e in / 
# Wed, 12 Apr 2023 00:39:01 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 04:22:01 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 04:24:29 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 12 Apr 2023 04:24:30 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 04:24:30 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:24:30 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 04:24:30 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 04:24:30 GMT
CMD []
```

-	Layers:
	-	`sha256:b2ee1f87789d52ef09851b4e5c9745fb8aceafa107b0d3452f9973f1abe65042`  
		Last Modified: Wed, 12 Apr 2023 00:42:45 GMT  
		Size: 32.4 MB (32398925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7355f41e5a426f8365e4578b296a964249f2359611192c75a22733eea31f2240`  
		Last Modified: Wed, 12 Apr 2023 04:25:52 GMT  
		Size: 69.7 MB (69684014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039d3b8c0e5dc9639808d5b8759e0ce0959c03ea06755da1fed6f9d662a4192d`  
		Last Modified: Wed, 12 Apr 2023 04:25:39 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; ppc64le

```console
$ docker pull varnish@sha256:18bd3322c2f9ccc96bfce197018af7ff9306a5913379476af9c84e061e770095
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.8 MB (99803629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27f0683fd328a003ec4c95f0c7d93bb88582d34cba7b9ea9a048b186914841c5`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:08:20 GMT
ADD file:63eb52aaff02c15bceabb87a78eb1b36389066ff4774cf8a754160ca7d509816 in / 
# Wed, 12 Apr 2023 00:08:23 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:06:51 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 01:16:48 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 12 Apr 2023 01:16:52 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 01:16:52 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 12 Apr 2023 01:16:53 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 01:16:53 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 01:16:54 GMT
CMD []
```

-	Layers:
	-	`sha256:5b41d5ec640939cf684959234ad3b80909268a32bfd520a31c6720a91521c2fa`  
		Last Modified: Wed, 12 Apr 2023 00:13:13 GMT  
		Size: 35.3 MB (35291995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c91ede6f2abd53adaec518fad85de307f689c38e8eab390a7359e142ae3a16`  
		Last Modified: Wed, 12 Apr 2023 01:18:31 GMT  
		Size: 64.5 MB (64510930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd33a842deca9de4a3e249248620b5666ab2fa35cae6fe8b10b79955f955c3e`  
		Last Modified: Wed, 12 Apr 2023 01:18:15 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; s390x

```console
$ docker pull varnish@sha256:91cf8dba2788f88ad8b8f188bb53c43d9b749547de652b93d26493f0c3cac63f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.0 MB (81006609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0df2b025628576f460505157da9b8f5f06d418c21686950786d49f881b8f9b2a`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:01:00 GMT
ADD file:b6463dba97ba9c0a29bacfafc4d67bc603ab57e80b75e23cd42d7ef4b0f8e6ae in / 
# Wed, 12 Apr 2023 00:01:04 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:50:27 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 07:52:14 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 12 Apr 2023 07:52:17 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 07:52:17 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 12 Apr 2023 07:52:17 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 07:52:17 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 07:52:17 GMT
CMD []
```

-	Layers:
	-	`sha256:97fe10bc7def58e7938e97e41eec4788ec7a45b6ef2cb1770cec02fa831fd19d`  
		Last Modified: Wed, 12 Apr 2023 00:05:18 GMT  
		Size: 29.7 MB (29653156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7822e42c3387f3cd91539d4e97252f558b188301244bec6480d7540b6a80882`  
		Last Modified: Wed, 12 Apr 2023 07:53:20 GMT  
		Size: 51.4 MB (51352752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750915994cfaac0ec2feb5390e1d622af471974ba829d7b86d1edf3d6b3beb0d`  
		Last Modified: Wed, 12 Apr 2023 07:53:13 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
