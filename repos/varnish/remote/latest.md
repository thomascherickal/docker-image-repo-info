## `varnish:latest`

```console
$ docker pull varnish@sha256:eb5fd055127f6f6bf35f8cb761dfd2a270aa09868069832e442b957fcea5aca1
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
$ docker pull varnish@sha256:a5b6776e15a60a90de100e46cc296417f4b107f7a3512528d87581c2b8c1c153
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.7 MB (104712402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9b9a40a2ae21bb5726b793e87ea41c2acad219217de0920f2b00b14b1812487`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 17 Nov 2021 02:20:41 GMT
ADD file:a2405ebb9892d98be2eb585f6121864d12b3fd983ebf15e5f0b7486e106a79c6 in / 
# Wed, 17 Nov 2021 02:20:42 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:02:38 GMT
ENV VARNISH_SIZE=100M
# Wed, 17 Nov 2021 03:05:15 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-7.0.0.tgz -o $tmpdir/orig.tgz;     echo "39c694db4ec7b35236d12fe2c03036260d6799395b1c8bb5a58e96fc88d67dcaa5eb8bc75643540d3aa0edc1a8924d7d839e88293b0521fadef4cd12f466fb4b  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.0|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 17 Nov 2021 03:05:15 GMT
WORKDIR /etc/varnish
# Wed, 17 Nov 2021 03:05:15 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Wed, 17 Nov 2021 03:05:16 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 17 Nov 2021 03:05:16 GMT
EXPOSE 80 8443
# Wed, 17 Nov 2021 03:05:16 GMT
CMD []
```

-	Layers:
	-	`sha256:eff15d958d664f0874d16aee393cc44387031ee0a68ef8542d0056c747f378e8`  
		Last Modified: Wed, 17 Nov 2021 02:25:45 GMT  
		Size: 31.4 MB (31370267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6fa98293da082b9eee03782128af01fc4e502e5b1765bdc65a2cd5385ff819`  
		Last Modified: Wed, 17 Nov 2021 03:10:59 GMT  
		Size: 73.3 MB (73341661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e15d9fe0b3aaca94c24ac1055f6b3da7d36d9ac6050be2ac11ce84e2218f61`  
		Last Modified: Wed, 17 Nov 2021 03:10:48 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; arm variant v7

```console
$ docker pull varnish@sha256:c240e795e9d62cb28f000d79d4217892527ccb7ba16c15956f46f84eeaa6a041
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.2 MB (81217264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fa82400ddb1489e132ea9fc08044a8414e5f6497bdd5d85f070d7213dd5d8be`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 17 Nov 2021 01:59:43 GMT
ADD file:cd2ac52107a2ea6657f23850a4b29366309eb39fa177321e0a9fd6d58562ae80 in / 
# Wed, 17 Nov 2021 01:59:44 GMT
CMD ["bash"]
# Thu, 18 Nov 2021 09:52:16 GMT
ENV VARNISH_SIZE=100M
# Thu, 18 Nov 2021 09:57:57 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-7.0.0.tgz -o $tmpdir/orig.tgz;     echo "39c694db4ec7b35236d12fe2c03036260d6799395b1c8bb5a58e96fc88d67dcaa5eb8bc75643540d3aa0edc1a8924d7d839e88293b0521fadef4cd12f466fb4b  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.0|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Thu, 18 Nov 2021 09:57:58 GMT
WORKDIR /etc/varnish
# Thu, 18 Nov 2021 09:57:58 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 18 Nov 2021 09:57:59 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 18 Nov 2021 09:57:59 GMT
EXPOSE 80 8443
# Thu, 18 Nov 2021 09:58:00 GMT
CMD []
```

-	Layers:
	-	`sha256:b6e5ca4da96841e58eb27c88695a059e5105fad5a066de803f4b94ae4002ba66`  
		Last Modified: Wed, 17 Nov 2021 02:15:13 GMT  
		Size: 26.6 MB (26573160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995a81b2cb29588b95194d051d0db4ad26537aaf524bed3daa994739dbb67e27`  
		Last Modified: Thu, 18 Nov 2021 10:06:50 GMT  
		Size: 54.6 MB (54643631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0ad718cf28c5982b42621ef4bf65053b627878d4c49c7dde6b3f1dcfbe9156`  
		Last Modified: Thu, 18 Nov 2021 10:06:21 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:331e3ee5311aa4b31e5f8faacca07b84bd9173bfe5ba1e19e47148f862f09b1e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.7 MB (98702970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a951c912ec6ea48924d63ee40547975645660c14694ee1af097a24ffce7b149`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 17 Nov 2021 02:40:15 GMT
ADD file:4203242b2b09a65239092c4780b59181da7b861b3c0be40810b3588aa200f72c in / 
# Wed, 17 Nov 2021 02:40:16 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 04:32:14 GMT
ENV VARNISH_SIZE=100M
# Wed, 17 Nov 2021 04:34:37 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-7.0.0.tgz -o $tmpdir/orig.tgz;     echo "39c694db4ec7b35236d12fe2c03036260d6799395b1c8bb5a58e96fc88d67dcaa5eb8bc75643540d3aa0edc1a8924d7d839e88293b0521fadef4cd12f466fb4b  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.0|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 17 Nov 2021 04:34:38 GMT
WORKDIR /etc/varnish
# Wed, 17 Nov 2021 04:34:39 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Wed, 17 Nov 2021 04:34:39 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 17 Nov 2021 04:34:40 GMT
EXPOSE 80 8443
# Wed, 17 Nov 2021 04:34:41 GMT
CMD []
```

-	Layers:
	-	`sha256:eb9a2845ed124d072b117aba4f0508e00c1ecd0d147dc324d14b00d24092046c`  
		Last Modified: Wed, 17 Nov 2021 02:47:17 GMT  
		Size: 30.1 MB (30056521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35eb9388ba1f805feffd8319d25466baeadd9f2d695f2aabc1b8444fc79cf250`  
		Last Modified: Wed, 17 Nov 2021 04:40:43 GMT  
		Size: 68.6 MB (68645975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e54176b0a037e66e61c824ba75ab82b47ba1e3e0fb2778c6a4e29c166e1a9a5`  
		Last Modified: Wed, 17 Nov 2021 04:40:33 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; 386

```console
$ docker pull varnish@sha256:50233d97f281820ca5abc37f58836a60ce0373326b786b9056f8171ce2d3f0f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.8 MB (105802766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93fc2c2a2308e428482a33014c6cd52b1e77773c168972e9636c857d2eacf078`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 17 Nov 2021 02:39:53 GMT
ADD file:ff018048717c0f5aa1730480d0bfea1c2bf94d6e2dae2d7cef46d05ffb0d93e1 in / 
# Wed, 17 Nov 2021 02:39:53 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:10:10 GMT
ENV VARNISH_SIZE=100M
# Wed, 17 Nov 2021 03:13:22 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-7.0.0.tgz -o $tmpdir/orig.tgz;     echo "39c694db4ec7b35236d12fe2c03036260d6799395b1c8bb5a58e96fc88d67dcaa5eb8bc75643540d3aa0edc1a8924d7d839e88293b0521fadef4cd12f466fb4b  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.0|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 17 Nov 2021 03:13:23 GMT
WORKDIR /etc/varnish
# Wed, 17 Nov 2021 03:13:23 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Wed, 17 Nov 2021 03:13:23 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 17 Nov 2021 03:13:24 GMT
EXPOSE 80 8443
# Wed, 17 Nov 2021 03:13:24 GMT
CMD []
```

-	Layers:
	-	`sha256:0bae0e1d4cb1d56ffeb9d05de7a097d3157267eef07b6d8131344d99bd97c431`  
		Last Modified: Wed, 17 Nov 2021 02:47:49 GMT  
		Size: 32.4 MB (32380683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6da7e8bf779c7a01eff42003ce0234602d48047066bdae20757149f130940e`  
		Last Modified: Wed, 17 Nov 2021 03:18:12 GMT  
		Size: 73.4 MB (73421610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737ddd62e39b33ec70b8bda30309091c785af357bd9dbab9e8b71408188bfc2c`  
		Last Modified: Wed, 17 Nov 2021 03:17:58 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; ppc64le

```console
$ docker pull varnish@sha256:9c1ea9b3990ca7a9106f0a8ec8b5cc38f4de5161912e2c2481a88b7459ba14f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.8 MB (103805146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75ea3420500395a52f3cbbaa26ea64adacb99d5dce8f2e24baa6d1583465061f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 17 Nov 2021 03:28:22 GMT
ADD file:5ed330f0fe1328f694fcaefb961cf4da4d8a4ff03100b21af718b69316168706 in / 
# Wed, 17 Nov 2021 03:28:38 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 06:04:25 GMT
ENV VARNISH_SIZE=100M
# Wed, 17 Nov 2021 06:33:48 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-7.0.0.tgz -o $tmpdir/orig.tgz;     echo "39c694db4ec7b35236d12fe2c03036260d6799395b1c8bb5a58e96fc88d67dcaa5eb8bc75643540d3aa0edc1a8924d7d839e88293b0521fadef4cd12f466fb4b  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.0|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 17 Nov 2021 06:34:03 GMT
WORKDIR /etc/varnish
# Wed, 17 Nov 2021 06:34:07 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Wed, 17 Nov 2021 06:34:11 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 17 Nov 2021 06:34:23 GMT
EXPOSE 80 8443
# Wed, 17 Nov 2021 06:34:29 GMT
CMD []
```

-	Layers:
	-	`sha256:258ff2a13858db8f51b65662e02137c0abcfd2528ca73e92b7a40061d938fb1e`  
		Last Modified: Wed, 17 Nov 2021 03:54:34 GMT  
		Size: 35.3 MB (35271382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede74025f453eb239899d64b9466f119dc2f664e82b1529db59b5385dca93f18`  
		Last Modified: Wed, 17 Nov 2021 07:37:12 GMT  
		Size: 68.5 MB (68533289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab465f900cffa890ba81f5102d4613ced3e455e7c2ee38240330afd97d791da1`  
		Last Modified: Wed, 17 Nov 2021 07:36:59 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; s390x

```console
$ docker pull varnish@sha256:e522646171effb2ec075821c7e8a8b1c60028f2d3203ed41d6b3da98e4e91dec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.0 MB (85001090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5981679e033a9ac77cd2b7a70bfbd08ca4c650d4dff4b879461ded143ea40d04`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 17 Nov 2021 02:42:27 GMT
ADD file:42f73dac307a6a5232e3100f3d3b36e8125f73a4ca504b106e60e2b66d242b2f in / 
# Wed, 17 Nov 2021 02:42:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 12:09:56 GMT
ENV VARNISH_SIZE=100M
# Wed, 17 Nov 2021 12:11:39 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-7.0.0.tgz -o $tmpdir/orig.tgz;     echo "39c694db4ec7b35236d12fe2c03036260d6799395b1c8bb5a58e96fc88d67dcaa5eb8bc75643540d3aa0edc1a8924d7d839e88293b0521fadef4cd12f466fb4b  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.0|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 17 Nov 2021 12:11:41 GMT
WORKDIR /etc/varnish
# Wed, 17 Nov 2021 12:11:41 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Wed, 17 Nov 2021 12:11:42 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 17 Nov 2021 12:11:42 GMT
EXPOSE 80 8443
# Wed, 17 Nov 2021 12:11:42 GMT
CMD []
```

-	Layers:
	-	`sha256:8d71e885edf612b507bbdcc48a970548d436b8709eeedfc2c98f6843a214b5e2`  
		Last Modified: Wed, 17 Nov 2021 02:48:25 GMT  
		Size: 29.7 MB (29650960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e14d21e5759658aedc62cd484439b3dc09cbdc979419679d402bd0a9409fbd`  
		Last Modified: Wed, 17 Nov 2021 12:13:55 GMT  
		Size: 55.3 MB (55349657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653d8908e660daa2a0615175ca8590b144cdd5aa6ee2652e83e6429ffee8cc47`  
		Last Modified: Wed, 17 Nov 2021 12:13:47 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
