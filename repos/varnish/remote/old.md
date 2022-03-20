## `varnish:old`

```console
$ docker pull varnish@sha256:53d615e2a6db98b9bf3c9303e5c29fc13786c7effda31f0dfc428c69f5241ab2
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
$ docker pull varnish@sha256:ceb0e5628b7fb4eb23217b2c7f116ca78daca2987e07900821afd94392533ead
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.1 MB (101113550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:820ecc12d5ee0330627735fc35c19eb32918ecb1c5b3eb73607caba1a8bfdd08`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 04:03:59 GMT
ADD file:36919ae6bb25e3269eff949443129a01a8a43fb967fe6563939ebe1e1e9b8228 in / 
# Thu, 17 Mar 2022 04:03:59 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:14:38 GMT
ENV VARNISH_SIZE=100M
# Sun, 20 Mar 2022 00:04:31 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.6.2.tgz -o $tmpdir/orig.tgz;     echo "8fa163678e2e454fcc959ba24f349de00e6c00357df55f37f12f0d3acbcb2799b2f376385cef2d40c14a4cc44a5eea1b5a3fbf6245961611d4fc3ea30699035d  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.6.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Sun, 20 Mar 2022 00:04:31 GMT
WORKDIR /etc/varnish
# Sun, 20 Mar 2022 00:04:31 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Sun, 20 Mar 2022 00:04:31 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sun, 20 Mar 2022 00:04:31 GMT
EXPOSE 80 8443
# Sun, 20 Mar 2022 00:04:32 GMT
CMD []
```

-	Layers:
	-	`sha256:ae13dd57832654086618a81dbc128846aa092489260c326ee95429b63c3cf213`  
		Last Modified: Thu, 17 Mar 2022 04:10:05 GMT  
		Size: 31.4 MB (31376572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57284e492bb6036061bdb17027b8e154cc8be30b44153241068791426c734d1c`  
		Last Modified: Sun, 20 Mar 2022 00:05:36 GMT  
		Size: 69.7 MB (69736276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59718dc58f2a3c7b3c625c9f1da93eaf95b0232302ac8f4f765f8e92bc20e1c1`  
		Last Modified: Sun, 20 Mar 2022 00:05:26 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; arm variant v7

```console
$ docker pull varnish@sha256:fa22cf9d36af5dbd164137be27784b5009102a6f0f33722da70cfcfab2a140d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.7 MB (77735741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fe6244f2128c994684ad2f6ca8ba4508bc1e1c35a888bd197b33a49d68b0bf8`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 09:31:03 GMT
ADD file:e52f9ee2dc3144d7b9eb3ec90c106aa2a094eb4c5c2aa8cbff5c520a5faaef43 in / 
# Thu, 17 Mar 2022 09:31:04 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 00:49:05 GMT
ENV VARNISH_SIZE=100M
# Sat, 19 Mar 2022 01:01:57 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.6.2.tgz -o $tmpdir/orig.tgz;     echo "8fa163678e2e454fcc959ba24f349de00e6c00357df55f37f12f0d3acbcb2799b2f376385cef2d40c14a4cc44a5eea1b5a3fbf6245961611d4fc3ea30699035d  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.6.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Sat, 19 Mar 2022 01:01:58 GMT
WORKDIR /etc/varnish
# Sat, 19 Mar 2022 01:01:59 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Sat, 19 Mar 2022 01:01:59 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sat, 19 Mar 2022 01:02:00 GMT
EXPOSE 80 8443
# Sat, 19 Mar 2022 01:02:00 GMT
CMD []
```

-	Layers:
	-	`sha256:5e5e708ee1f9fdbc69324391f7d1f816c657e6116eff09e7d2247fa9de3a076a`  
		Last Modified: Thu, 17 Mar 2022 09:46:33 GMT  
		Size: 26.6 MB (26575097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98cc1c8933053775de6779b877b7ca445f9a73c34096af1fdf3ca690ba7627d3`  
		Last Modified: Sat, 19 Mar 2022 01:12:50 GMT  
		Size: 51.2 MB (51159942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c386dfd96d2a48c53e2b42cc6c84b7a7e046246107d251112c15abc1616120b`  
		Last Modified: Sat, 19 Mar 2022 01:12:21 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:4f18b129c3f237da945b10951729b27cdd43bbf644808af5b78a4a3a8b0896ce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.2 MB (95219970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb1380a2e7a8df023e04df35e84a492a873bf9d3d4470f643294d3f59c677ec7`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 03:21:57 GMT
ADD file:e52e032f1ace6abd44b3647d43c1b8ae30bac6de804eef09c6ccd793057996fd in / 
# Thu, 17 Mar 2022 03:21:58 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 21:09:19 GMT
ENV VARNISH_SIZE=100M
# Thu, 17 Mar 2022 21:14:55 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.6.2.tgz -o $tmpdir/orig.tgz;     echo "8fa163678e2e454fcc959ba24f349de00e6c00357df55f37f12f0d3acbcb2799b2f376385cef2d40c14a4cc44a5eea1b5a3fbf6245961611d4fc3ea30699035d  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.6.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 17 Mar 2022 21:14:55 GMT
WORKDIR /etc/varnish
# Thu, 17 Mar 2022 21:14:57 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 17 Mar 2022 21:14:57 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 17 Mar 2022 21:14:58 GMT
EXPOSE 80 8443
# Thu, 17 Mar 2022 21:14:59 GMT
CMD []
```

-	Layers:
	-	`sha256:32252aec0777ac025a158bc2a8317650a4f2a0a875387011b1165013874f8723`  
		Last Modified: Thu, 17 Mar 2022 03:28:36 GMT  
		Size: 30.1 MB (30063013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298e67252967165ad63df145d2950c5d0b496743a71c9eb0c150d48dbe2fa10b`  
		Last Modified: Thu, 17 Mar 2022 21:20:07 GMT  
		Size: 65.2 MB (65156257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a48220cdf7996004e630e25fee6d2b87dabb049ba1139429994808ef9e9dc1d`  
		Last Modified: Thu, 17 Mar 2022 21:19:57 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; 386

```console
$ docker pull varnish@sha256:6528d701b7e8464cdcedc29c82c727f7e627da9fa81a656fe8ea8a6c0d256e32
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.5 MB (102513384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a34a67f6b92e0511d8c174ca13148538c3090403f89987b0436bec5801b0ee6`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 08:15:53 GMT
ADD file:2d6be3846f0e5fabd85bc9409b1e2223cad4c57c76f96e9f81489ba78a72a1f5 in / 
# Thu, 17 Mar 2022 08:15:54 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 21:41:42 GMT
ENV VARNISH_SIZE=100M
# Sat, 19 Mar 2022 05:24:23 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.6.2.tgz -o $tmpdir/orig.tgz;     echo "8fa163678e2e454fcc959ba24f349de00e6c00357df55f37f12f0d3acbcb2799b2f376385cef2d40c14a4cc44a5eea1b5a3fbf6245961611d4fc3ea30699035d  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.6.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Sat, 19 Mar 2022 05:24:23 GMT
WORKDIR /etc/varnish
# Sat, 19 Mar 2022 05:24:23 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Sat, 19 Mar 2022 05:24:23 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sat, 19 Mar 2022 05:24:24 GMT
EXPOSE 80 8443
# Sat, 19 Mar 2022 05:24:24 GMT
CMD []
```

-	Layers:
	-	`sha256:176085117cac9b2cf2cf57b3a10c9811dbd2773497fbac3086b5024070447e97`  
		Last Modified: Thu, 17 Mar 2022 08:24:00 GMT  
		Size: 32.4 MB (32386475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3167843a619d8f72ae3602484792c415d578d797c3692ec148af41204dcded6`  
		Last Modified: Sat, 19 Mar 2022 05:26:26 GMT  
		Size: 70.1 MB (70126207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51229296cf74bd0fd91a4f24297b07f9fa104444b5233a0bf943d5594d7c6ac8`  
		Last Modified: Sat, 19 Mar 2022 05:26:07 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; ppc64le

```console
$ docker pull varnish@sha256:516724df4877fb39004344774ed939277b60584e09e9423c81f3005fdbb748ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.3 MB (100295169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c68b32bd137597f8eae7b6a55b26d24d0b49ac0cd3b283e3c829f5edbdeffce`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 11:17:54 GMT
ADD file:e8555f1cb439a45786b92e929cfa154b51f668c5b4cd69e4ce98340c5998fe0c in / 
# Thu, 17 Mar 2022 11:18:00 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 11:39:46 GMT
ENV VARNISH_SIZE=100M
# Sun, 20 Mar 2022 04:22:26 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.6.2.tgz -o $tmpdir/orig.tgz;     echo "8fa163678e2e454fcc959ba24f349de00e6c00357df55f37f12f0d3acbcb2799b2f376385cef2d40c14a4cc44a5eea1b5a3fbf6245961611d4fc3ea30699035d  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.6.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Sun, 20 Mar 2022 04:22:30 GMT
WORKDIR /etc/varnish
# Sun, 20 Mar 2022 04:22:31 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Sun, 20 Mar 2022 04:22:32 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sun, 20 Mar 2022 04:22:35 GMT
EXPOSE 80 8443
# Sun, 20 Mar 2022 04:22:37 GMT
CMD []
```

-	Layers:
	-	`sha256:aec78dc45d7b3df12df0672d13e22005592b453f03ff2580efac2598dddd680b`  
		Last Modified: Thu, 17 Mar 2022 11:28:17 GMT  
		Size: 35.3 MB (35279758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732e774535572464a7e3f636a241080379d75daf8d17d6ebdf13f28b083670e9`  
		Last Modified: Sun, 20 Mar 2022 04:43:23 GMT  
		Size: 65.0 MB (65014708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945c446bfa438e027aa33106b918d07dac528cdb847b0dd1d47b37fc9fc3ec10`  
		Last Modified: Sun, 20 Mar 2022 04:43:10 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; s390x

```console
$ docker pull varnish@sha256:72473156a8a014edb1a6622972e152725615942a0d6015f793e2d63202abce15
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.5 MB (81547053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fd4df79691f660f8cd37211255e12fccd9054ccb341a3fe7b516058660382a2`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 03:06:58 GMT
ADD file:52f9267b4c57ac585a0d3d47a6f2ae1a71398264173ad4f190332957fa629c67 in / 
# Thu, 17 Mar 2022 03:07:01 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 16:51:29 GMT
ENV VARNISH_SIZE=100M
# Thu, 17 Mar 2022 16:56:24 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.6.2.tgz -o $tmpdir/orig.tgz;     echo "8fa163678e2e454fcc959ba24f349de00e6c00357df55f37f12f0d3acbcb2799b2f376385cef2d40c14a4cc44a5eea1b5a3fbf6245961611d4fc3ea30699035d  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.6.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 17 Mar 2022 16:56:28 GMT
WORKDIR /etc/varnish
# Thu, 17 Mar 2022 16:56:28 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 17 Mar 2022 16:56:28 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 17 Mar 2022 16:56:28 GMT
EXPOSE 80 8443
# Thu, 17 Mar 2022 16:56:28 GMT
CMD []
```

-	Layers:
	-	`sha256:d101968410e5005df630b0572aec03c88de55b8de81f3cf7e6a57e1ce2e5a8e5`  
		Last Modified: Thu, 17 Mar 2022 03:12:46 GMT  
		Size: 29.7 MB (29655795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08574022bcf84ce6f78055f37a17306764389ff02a8dcb4d1a6f114aee1773f3`  
		Last Modified: Thu, 17 Mar 2022 16:59:03 GMT  
		Size: 51.9 MB (51890556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71404eac9f53aeacdd8551ed9a037f3a2f0a3ff0082bb0b15c819ba00b4e69f8`  
		Last Modified: Thu, 17 Mar 2022 16:58:56 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
