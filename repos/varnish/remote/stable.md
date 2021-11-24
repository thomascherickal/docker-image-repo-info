## `varnish:stable`

```console
$ docker pull varnish@sha256:6f0b97e1826376336d5e1ecfbd72ea519b4552fb1dd1d0ffa4d1a5babdfd038c
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
$ docker pull varnish@sha256:9cefaadb857e5484b4aa2aefd456415559aeaa9e8246e5eaa5545883e81bef5f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.5 MB (103503329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbff298becb88cba6a6af16ee6afb23063e4d42ddfadd3676c5811d0e11cd1b1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 17 Nov 2021 02:20:41 GMT
ADD file:a2405ebb9892d98be2eb585f6121864d12b3fd983ebf15e5f0b7486e106a79c6 in / 
# Wed, 17 Nov 2021 02:20:42 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:02:38 GMT
ENV VARNISH_SIZE=100M
# Wed, 17 Nov 2021 03:10:21 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.0.8.tgz -o $tmpdir/orig.tgz;     echo "73ed2f465ba3b11680b20a70633fc78da9b3eac68395f927b7ff02f4106b6cc92a2b395db2813a0605da2771530e5c4fc594eaf5a9a32bf2e42181b6dd90cf3f  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.8|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 17 Nov 2021 03:10:21 GMT
WORKDIR /etc/varnish
# Wed, 17 Nov 2021 03:10:22 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 17 Nov 2021 03:10:22 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 17 Nov 2021 03:10:22 GMT
EXPOSE 80 8443
# Wed, 17 Nov 2021 03:10:22 GMT
CMD []
```

-	Layers:
	-	`sha256:eff15d958d664f0874d16aee393cc44387031ee0a68ef8542d0056c747f378e8`  
		Last Modified: Wed, 17 Nov 2021 02:25:45 GMT  
		Size: 31.4 MB (31370267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d667ed58e129d383edb49de0c24e0a85f030ea5b33a927dea80a09e4b37adc`  
		Last Modified: Wed, 17 Nov 2021 03:11:49 GMT  
		Size: 72.1 MB (72132360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc4e85cd853d6ad107d240dfb745c2f2e0a9f9fb759998a8a7618bfa56f9d07`  
		Last Modified: Wed, 17 Nov 2021 03:11:39 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; arm variant v7

```console
$ docker pull varnish@sha256:c07401fbada8dcfb30316530b22680d446cb206090d92fe1530bc8244876d941
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80045960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0575bdb28c3e85f2bec56215667be87aed7cf9da82997ae6cf0388b9920d5c3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 17 Nov 2021 01:59:43 GMT
ADD file:cd2ac52107a2ea6657f23850a4b29366309eb39fa177321e0a9fd6d58562ae80 in / 
# Wed, 17 Nov 2021 01:59:44 GMT
CMD ["bash"]
# Thu, 18 Nov 2021 09:52:16 GMT
ENV VARNISH_SIZE=100M
# Thu, 18 Nov 2021 10:05:04 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.0.8.tgz -o $tmpdir/orig.tgz;     echo "73ed2f465ba3b11680b20a70633fc78da9b3eac68395f927b7ff02f4106b6cc92a2b395db2813a0605da2771530e5c4fc594eaf5a9a32bf2e42181b6dd90cf3f  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.8|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Thu, 18 Nov 2021 10:05:05 GMT
WORKDIR /etc/varnish
# Thu, 18 Nov 2021 10:05:05 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 18 Nov 2021 10:05:06 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 18 Nov 2021 10:05:06 GMT
EXPOSE 80 8443
# Thu, 18 Nov 2021 10:05:07 GMT
CMD []
```

-	Layers:
	-	`sha256:b6e5ca4da96841e58eb27c88695a059e5105fad5a066de803f4b94ae4002ba66`  
		Last Modified: Wed, 17 Nov 2021 02:15:13 GMT  
		Size: 26.6 MB (26573160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5736611207f9ab6e495c3a8258205db6cf5c8dd58bbba8cf9058a1c3271b70c5`  
		Last Modified: Thu, 18 Nov 2021 10:07:47 GMT  
		Size: 53.5 MB (53472100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b70a0546c868480d128124ce89dc7923b8ce3979c92d7887f34cbc043b2267e`  
		Last Modified: Thu, 18 Nov 2021 10:07:19 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:c928b550c26640919c0582045590d449f8ed4dde96d2aef96b9cc7c9ed409530
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.5 MB (97533085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04aad97694b8ac0c6fad4a40b9f56be76415697bd3c21381e912650779452d92`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 17 Nov 2021 02:40:15 GMT
ADD file:4203242b2b09a65239092c4780b59181da7b861b3c0be40810b3588aa200f72c in / 
# Wed, 17 Nov 2021 02:40:16 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 04:32:14 GMT
ENV VARNISH_SIZE=100M
# Wed, 17 Nov 2021 04:39:46 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.0.8.tgz -o $tmpdir/orig.tgz;     echo "73ed2f465ba3b11680b20a70633fc78da9b3eac68395f927b7ff02f4106b6cc92a2b395db2813a0605da2771530e5c4fc594eaf5a9a32bf2e42181b6dd90cf3f  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.8|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 17 Nov 2021 04:39:46 GMT
WORKDIR /etc/varnish
# Wed, 17 Nov 2021 04:39:48 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 17 Nov 2021 04:39:48 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 17 Nov 2021 04:39:49 GMT
EXPOSE 80 8443
# Wed, 17 Nov 2021 04:39:50 GMT
CMD []
```

-	Layers:
	-	`sha256:eb9a2845ed124d072b117aba4f0508e00c1ecd0d147dc324d14b00d24092046c`  
		Last Modified: Wed, 17 Nov 2021 02:47:17 GMT  
		Size: 30.1 MB (30056521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ccc34b59256b34a663b30483f48ffe180875b7b9ab652ca6c5f086239106d2`  
		Last Modified: Wed, 17 Nov 2021 04:41:37 GMT  
		Size: 67.5 MB (67475863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ee133477d1347e016652a50cf39a47c1d9b619e1bcdbaefe5f26097572c7d9`  
		Last Modified: Wed, 17 Nov 2021 04:41:27 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; 386

```console
$ docker pull varnish@sha256:5d755ac59fca0f6e2c886e91cd66e4a1c18fbf9f67acd0ad7da6ebd23c2f8288
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.8 MB (104751828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90279c337e591d81685afdb3579485a9d53623da5cbd404029951f6901d0f1ab`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 17 Nov 2021 02:39:53 GMT
ADD file:ff018048717c0f5aa1730480d0bfea1c2bf94d6e2dae2d7cef46d05ffb0d93e1 in / 
# Wed, 17 Nov 2021 02:39:53 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:10:10 GMT
ENV VARNISH_SIZE=100M
# Wed, 17 Nov 2021 03:17:14 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.0.8.tgz -o $tmpdir/orig.tgz;     echo "73ed2f465ba3b11680b20a70633fc78da9b3eac68395f927b7ff02f4106b6cc92a2b395db2813a0605da2771530e5c4fc594eaf5a9a32bf2e42181b6dd90cf3f  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.8|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 17 Nov 2021 03:17:17 GMT
WORKDIR /etc/varnish
# Wed, 17 Nov 2021 03:17:17 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 17 Nov 2021 03:17:17 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 17 Nov 2021 03:17:18 GMT
EXPOSE 80 8443
# Wed, 17 Nov 2021 03:17:18 GMT
CMD []
```

-	Layers:
	-	`sha256:0bae0e1d4cb1d56ffeb9d05de7a097d3157267eef07b6d8131344d99bd97c431`  
		Last Modified: Wed, 17 Nov 2021 02:47:49 GMT  
		Size: 32.4 MB (32380683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cff288a3cfecf3065cb555da4033fd5136fa00c1d1a3fbaf2d26d86a654a042`  
		Last Modified: Wed, 17 Nov 2021 03:18:50 GMT  
		Size: 72.4 MB (72370444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b900b861bf9ebaa2a7a820a6b65a8e534f39d694b28f38933e74e384026298cf`  
		Last Modified: Wed, 17 Nov 2021 03:18:35 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; ppc64le

```console
$ docker pull varnish@sha256:40cf090fa2b141c82b92a97999cb6e5edabfd8ca85ba937bd9d7b3634ce3f4bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.7 MB (102651397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3591e633f06d21eec5a59ce9510e2695cc4082370f3d317fbed87d9c6713794d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 17 Nov 2021 03:28:22 GMT
ADD file:5ed330f0fe1328f694fcaefb961cf4da4d8a4ff03100b21af718b69316168706 in / 
# Wed, 17 Nov 2021 03:28:38 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 06:04:25 GMT
ENV VARNISH_SIZE=100M
# Wed, 17 Nov 2021 07:36:01 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.0.8.tgz -o $tmpdir/orig.tgz;     echo "73ed2f465ba3b11680b20a70633fc78da9b3eac68395f927b7ff02f4106b6cc92a2b395db2813a0605da2771530e5c4fc594eaf5a9a32bf2e42181b6dd90cf3f  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.8|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 17 Nov 2021 07:36:07 GMT
WORKDIR /etc/varnish
# Wed, 17 Nov 2021 07:36:08 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 17 Nov 2021 07:36:09 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 17 Nov 2021 07:36:11 GMT
EXPOSE 80 8443
# Wed, 17 Nov 2021 07:36:14 GMT
CMD []
```

-	Layers:
	-	`sha256:258ff2a13858db8f51b65662e02137c0abcfd2528ca73e92b7a40061d938fb1e`  
		Last Modified: Wed, 17 Nov 2021 03:54:34 GMT  
		Size: 35.3 MB (35271382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd72144f4cad756c9443b3fe38a48bb132072f786b8b8cf5dd94d6aac00175f6`  
		Last Modified: Wed, 17 Nov 2021 07:38:13 GMT  
		Size: 67.4 MB (67379313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26b3cef66f6a2e490527b4897674457868ceb0a192e3f9876834133cbcede80`  
		Last Modified: Wed, 17 Nov 2021 07:38:00 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; s390x

```console
$ docker pull varnish@sha256:70f2c1561bd91312529d25d9060d1b6023f1e97a5d843a0af53f66845a91fcd4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.8 MB (83786925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71d59abd0994117eb46de293abdc871becc1c4e79fa1e2a7177865c1066f96ec`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 17 Nov 2021 02:42:27 GMT
ADD file:42f73dac307a6a5232e3100f3d3b36e8125f73a4ca504b106e60e2b66d242b2f in / 
# Wed, 17 Nov 2021 02:42:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 12:09:56 GMT
ENV VARNISH_SIZE=100M
# Wed, 24 Nov 2021 20:29:48 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-6.0.8.tgz -o $tmpdir/orig.tgz;     echo "73ed2f465ba3b11680b20a70633fc78da9b3eac68395f927b7ff02f4106b6cc92a2b395db2813a0605da2771530e5c4fc594eaf5a9a32bf2e42181b6dd90cf3f  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.8|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 24 Nov 2021 20:29:50 GMT
WORKDIR /etc/varnish
# Wed, 24 Nov 2021 20:29:50 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 24 Nov 2021 20:29:50 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 24 Nov 2021 20:29:50 GMT
EXPOSE 80 8443
# Wed, 24 Nov 2021 20:29:51 GMT
CMD []
```

-	Layers:
	-	`sha256:8d71e885edf612b507bbdcc48a970548d436b8709eeedfc2c98f6843a214b5e2`  
		Last Modified: Wed, 17 Nov 2021 02:48:25 GMT  
		Size: 29.7 MB (29650960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10c09fdaf917d59b135390e666871ffe70e2701d0e957686bdef300d8ccc837`  
		Last Modified: Wed, 24 Nov 2021 20:31:20 GMT  
		Size: 54.1 MB (54135264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e37af7af0efec3cdee9c3eaf78d448e442ebd292bd854fd2227521f177558b3`  
		Last Modified: Wed, 24 Nov 2021 20:31:13 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
