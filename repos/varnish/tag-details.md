<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `varnish`

-	[`varnish:6.0`](#varnish60)
-	[`varnish:6.0.11`](#varnish6011)
-	[`varnish:7.1`](#varnish71)
-	[`varnish:7.1-alpine`](#varnish71-alpine)
-	[`varnish:7.1.2`](#varnish712)
-	[`varnish:7.1.2-alpine`](#varnish712-alpine)
-	[`varnish:7.2`](#varnish72)
-	[`varnish:7.2-alpine`](#varnish72-alpine)
-	[`varnish:7.2.1`](#varnish721)
-	[`varnish:7.2.1-alpine`](#varnish721-alpine)
-	[`varnish:alpine`](#varnishalpine)
-	[`varnish:fresh`](#varnishfresh)
-	[`varnish:fresh-alpine`](#varnishfresh-alpine)
-	[`varnish:latest`](#varnishlatest)
-	[`varnish:old`](#varnishold)
-	[`varnish:old-alpine`](#varnishold-alpine)
-	[`varnish:stable`](#varnishstable)

## `varnish:6.0`

```console
$ docker pull varnish@sha256:b0d247fec393954674a4157f3de84fa53a2ccb7717d0ee38b373422b62549668
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
$ docker pull varnish@sha256:e4cd2e7566f7b0bb6024b2bbc7afbcc0051578eda02a26f23e6eb0f2fb1d8b17
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100654177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a3021a46bbb249a168c045b9b28ed52b3080066ecd5c56949a13f602a883fe5`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:45:19 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 06:47:30 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 09 Feb 2023 06:47:31 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 06:47:31 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 09 Feb 2023 06:47:31 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 06:47:31 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 06:47:31 GMT
CMD []
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80050f63f771eb4efeb5c0520d8f026ffeb09052cc3d2e9ad6a21a0b9e421d9`  
		Last Modified: Thu, 09 Feb 2023 06:48:55 GMT  
		Size: 69.2 MB (69241665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6274344d07d3f36b703541c8cbd5a4af391685ca105a99b7428780321587d14`  
		Last Modified: Thu, 09 Feb 2023 06:48:46 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; arm variant v7

```console
$ docker pull varnish@sha256:0f77cb08adbcd607941b11e583028385baa63d283cc3ec0f6b2588b72963746a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77210486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67eb10f44de604385766a212cdf419e153376019a21700a8fca61efc445f1110`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Sat, 04 Feb 2023 09:59:36 GMT
ADD file:c3cb8f4527fa96e99a4741ecb398113f25f53389c173b74f6c2a5e39a6575c60 in / 
# Sat, 04 Feb 2023 09:59:36 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 21:26:03 GMT
ENV VARNISH_SIZE=100M
# Sat, 04 Feb 2023 21:28:15 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Sat, 04 Feb 2023 21:28:16 GMT
WORKDIR /etc/varnish
# Sat, 04 Feb 2023 21:28:16 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Sat, 04 Feb 2023 21:28:16 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sat, 04 Feb 2023 21:28:16 GMT
EXPOSE 80 8443
# Sat, 04 Feb 2023 21:28:16 GMT
CMD []
```

-	Layers:
	-	`sha256:bd25bcdfbaa165120ee21b6567df395fe7d7b38da3cca0bcecee55a190e04aab`  
		Last Modified: Sat, 04 Feb 2023 10:06:24 GMT  
		Size: 26.6 MB (26559474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333b4a031d92c063bed44bddd31488609edfb71d88110e3809d9651c51d6226f`  
		Last Modified: Sat, 04 Feb 2023 21:30:19 GMT  
		Size: 50.7 MB (50650309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3f7526ff1da106d69172301d1772476cef2a5485c2ad546e1ca910343be780`  
		Last Modified: Sat, 04 Feb 2023 21:30:11 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:c450ad79500ba96cc35dd3c52ad3599334e6b3041428c499f6be27e07f1d22c7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94715178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bcf86c429658bbe854449e54a0595d02f2cd4d0cd0a866950b73caa3b511092`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 08:49:30 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 08:51:12 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 09 Feb 2023 08:51:12 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 08:51:12 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 09 Feb 2023 08:51:12 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 08:51:12 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 08:51:12 GMT
CMD []
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf53fb8b108e21aca2703892f32fa2f2619b742b46646331e3de24ab29d2ff0`  
		Last Modified: Thu, 09 Feb 2023 08:52:40 GMT  
		Size: 64.7 MB (64651966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221a70689e8a24c44e0e2d2a614e95e20e58ad7b87f01b72f52870e353b77c63`  
		Last Modified: Thu, 09 Feb 2023 08:52:33 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; 386

```console
$ docker pull varnish@sha256:f56aa456fae0b77ca66bec4fe85700f8781a3884de98883c8ff959c9dd055f2d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102061249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de466f497ac50aeb90f89b48ee5a85c34f954ccb439cd58cafdc8cb74267e295`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Sat, 04 Feb 2023 07:49:22 GMT
ADD file:82af884aad6a87f5b309a7418aa1df69f92180a39818ae6d77d37d072cb6fecb in / 
# Sat, 04 Feb 2023 07:49:22 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 21:42:34 GMT
ENV VARNISH_SIZE=100M
# Sat, 04 Feb 2023 21:45:00 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Sat, 04 Feb 2023 21:45:00 GMT
WORKDIR /etc/varnish
# Sat, 04 Feb 2023 21:45:02 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Sat, 04 Feb 2023 21:45:02 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sat, 04 Feb 2023 21:45:03 GMT
EXPOSE 80 8443
# Sat, 04 Feb 2023 21:45:04 GMT
CMD []
```

-	Layers:
	-	`sha256:fb99e0a97d653ef9acb2bdac0d1d10a8655b789bd4e8924c4a1c4a2af8adbb4a`  
		Last Modified: Sat, 04 Feb 2023 07:55:04 GMT  
		Size: 32.4 MB (32375772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2e84e91a218f50a680c6e76813b7dc715f8531d7019f32602ffd231bc68c52`  
		Last Modified: Sat, 04 Feb 2023 21:46:29 GMT  
		Size: 69.7 MB (69684776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0caa57957b3cf341e896f98722d6ad32929b1ea6ddd1a3934ed40cdd62d247eb`  
		Last Modified: Sat, 04 Feb 2023 21:46:20 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; ppc64le

```console
$ docker pull varnish@sha256:193cbaeb322e0557f034c425514d885339d6668c4386aa513402721bd9c21133
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.8 MB (99799855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fda082de4c7749b8307345a3b8d4137b5dabdedcabcd421708578b85a9e9a489`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 06:21:49 GMT
ADD file:b09577b8131a90731fdfb00b824a97dc65ccb51d484cb9004382035d64a5741c in / 
# Thu, 09 Feb 2023 06:21:52 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:04:27 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 12:11:06 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 09 Feb 2023 12:11:08 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 12:11:09 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 09 Feb 2023 12:11:09 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 12:11:10 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 12:11:10 GMT
CMD []
```

-	Layers:
	-	`sha256:4ea90e1a094ae86c7950bbec99e7a79b08fae641ad5f3bc3af9081c925894c41`  
		Last Modified: Thu, 09 Feb 2023 06:28:27 GMT  
		Size: 35.3 MB (35289252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d53de417bdc50d62d7fdbeeea8e46800fabd0ed80370a9069c87147b7123ad5`  
		Last Modified: Thu, 09 Feb 2023 12:13:28 GMT  
		Size: 64.5 MB (64509900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622e78faebf5b8024d64bf97cbc1e0a1a2ef6e8ed2fddbb16abfc817471fc463`  
		Last Modified: Thu, 09 Feb 2023 12:13:11 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; s390x

```console
$ docker pull varnish@sha256:df592d2c04da7cb2ee2144d4d971e719e7a60555c989bb86dde0d6c56089a79f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.0 MB (81002185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73636281614290efddc6e2f074b73a8ae88c72ab5f8d5e59d9349b2e0b0203b4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 02:41:45 GMT
ADD file:dc3c16b50baeac5b9644e607c8df9606e9583f8598e3ba34bcdd69c669a5904c in / 
# Thu, 09 Feb 2023 02:41:46 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 04:36:52 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 04:41:52 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 09 Feb 2023 04:42:02 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 04:42:02 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 09 Feb 2023 04:42:03 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 04:42:03 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 04:42:04 GMT
CMD []
```

-	Layers:
	-	`sha256:c2f78940fdfbfc5ce5d1d3cff3c27a319451aeb3ec12ff2473073516907fbce9`  
		Last Modified: Thu, 09 Feb 2023 02:46:06 GMT  
		Size: 29.6 MB (29647513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745410423134e2a363bf94f19d54352747cc0d7d642545ec7a337ad28c334724`  
		Last Modified: Thu, 09 Feb 2023 04:43:20 GMT  
		Size: 51.4 MB (51353971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e967e8ebb718a1ca31b86298d62b3fdfdcf3fac94d321d34ba0754a9c55395`  
		Last Modified: Thu, 09 Feb 2023 04:43:14 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0.11`

```console
$ docker pull varnish@sha256:b0d247fec393954674a4157f3de84fa53a2ccb7717d0ee38b373422b62549668
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
$ docker pull varnish@sha256:e4cd2e7566f7b0bb6024b2bbc7afbcc0051578eda02a26f23e6eb0f2fb1d8b17
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100654177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a3021a46bbb249a168c045b9b28ed52b3080066ecd5c56949a13f602a883fe5`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:45:19 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 06:47:30 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 09 Feb 2023 06:47:31 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 06:47:31 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 09 Feb 2023 06:47:31 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 06:47:31 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 06:47:31 GMT
CMD []
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80050f63f771eb4efeb5c0520d8f026ffeb09052cc3d2e9ad6a21a0b9e421d9`  
		Last Modified: Thu, 09 Feb 2023 06:48:55 GMT  
		Size: 69.2 MB (69241665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6274344d07d3f36b703541c8cbd5a4af391685ca105a99b7428780321587d14`  
		Last Modified: Thu, 09 Feb 2023 06:48:46 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.11` - linux; arm variant v7

```console
$ docker pull varnish@sha256:0f77cb08adbcd607941b11e583028385baa63d283cc3ec0f6b2588b72963746a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77210486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67eb10f44de604385766a212cdf419e153376019a21700a8fca61efc445f1110`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Sat, 04 Feb 2023 09:59:36 GMT
ADD file:c3cb8f4527fa96e99a4741ecb398113f25f53389c173b74f6c2a5e39a6575c60 in / 
# Sat, 04 Feb 2023 09:59:36 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 21:26:03 GMT
ENV VARNISH_SIZE=100M
# Sat, 04 Feb 2023 21:28:15 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Sat, 04 Feb 2023 21:28:16 GMT
WORKDIR /etc/varnish
# Sat, 04 Feb 2023 21:28:16 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Sat, 04 Feb 2023 21:28:16 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sat, 04 Feb 2023 21:28:16 GMT
EXPOSE 80 8443
# Sat, 04 Feb 2023 21:28:16 GMT
CMD []
```

-	Layers:
	-	`sha256:bd25bcdfbaa165120ee21b6567df395fe7d7b38da3cca0bcecee55a190e04aab`  
		Last Modified: Sat, 04 Feb 2023 10:06:24 GMT  
		Size: 26.6 MB (26559474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333b4a031d92c063bed44bddd31488609edfb71d88110e3809d9651c51d6226f`  
		Last Modified: Sat, 04 Feb 2023 21:30:19 GMT  
		Size: 50.7 MB (50650309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3f7526ff1da106d69172301d1772476cef2a5485c2ad546e1ca910343be780`  
		Last Modified: Sat, 04 Feb 2023 21:30:11 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.11` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:c450ad79500ba96cc35dd3c52ad3599334e6b3041428c499f6be27e07f1d22c7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94715178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bcf86c429658bbe854449e54a0595d02f2cd4d0cd0a866950b73caa3b511092`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 08:49:30 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 08:51:12 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 09 Feb 2023 08:51:12 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 08:51:12 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 09 Feb 2023 08:51:12 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 08:51:12 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 08:51:12 GMT
CMD []
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf53fb8b108e21aca2703892f32fa2f2619b742b46646331e3de24ab29d2ff0`  
		Last Modified: Thu, 09 Feb 2023 08:52:40 GMT  
		Size: 64.7 MB (64651966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221a70689e8a24c44e0e2d2a614e95e20e58ad7b87f01b72f52870e353b77c63`  
		Last Modified: Thu, 09 Feb 2023 08:52:33 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.11` - linux; 386

```console
$ docker pull varnish@sha256:f56aa456fae0b77ca66bec4fe85700f8781a3884de98883c8ff959c9dd055f2d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102061249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de466f497ac50aeb90f89b48ee5a85c34f954ccb439cd58cafdc8cb74267e295`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Sat, 04 Feb 2023 07:49:22 GMT
ADD file:82af884aad6a87f5b309a7418aa1df69f92180a39818ae6d77d37d072cb6fecb in / 
# Sat, 04 Feb 2023 07:49:22 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 21:42:34 GMT
ENV VARNISH_SIZE=100M
# Sat, 04 Feb 2023 21:45:00 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Sat, 04 Feb 2023 21:45:00 GMT
WORKDIR /etc/varnish
# Sat, 04 Feb 2023 21:45:02 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Sat, 04 Feb 2023 21:45:02 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sat, 04 Feb 2023 21:45:03 GMT
EXPOSE 80 8443
# Sat, 04 Feb 2023 21:45:04 GMT
CMD []
```

-	Layers:
	-	`sha256:fb99e0a97d653ef9acb2bdac0d1d10a8655b789bd4e8924c4a1c4a2af8adbb4a`  
		Last Modified: Sat, 04 Feb 2023 07:55:04 GMT  
		Size: 32.4 MB (32375772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2e84e91a218f50a680c6e76813b7dc715f8531d7019f32602ffd231bc68c52`  
		Last Modified: Sat, 04 Feb 2023 21:46:29 GMT  
		Size: 69.7 MB (69684776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0caa57957b3cf341e896f98722d6ad32929b1ea6ddd1a3934ed40cdd62d247eb`  
		Last Modified: Sat, 04 Feb 2023 21:46:20 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.11` - linux; ppc64le

```console
$ docker pull varnish@sha256:193cbaeb322e0557f034c425514d885339d6668c4386aa513402721bd9c21133
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.8 MB (99799855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fda082de4c7749b8307345a3b8d4137b5dabdedcabcd421708578b85a9e9a489`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 06:21:49 GMT
ADD file:b09577b8131a90731fdfb00b824a97dc65ccb51d484cb9004382035d64a5741c in / 
# Thu, 09 Feb 2023 06:21:52 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:04:27 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 12:11:06 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 09 Feb 2023 12:11:08 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 12:11:09 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 09 Feb 2023 12:11:09 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 12:11:10 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 12:11:10 GMT
CMD []
```

-	Layers:
	-	`sha256:4ea90e1a094ae86c7950bbec99e7a79b08fae641ad5f3bc3af9081c925894c41`  
		Last Modified: Thu, 09 Feb 2023 06:28:27 GMT  
		Size: 35.3 MB (35289252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d53de417bdc50d62d7fdbeeea8e46800fabd0ed80370a9069c87147b7123ad5`  
		Last Modified: Thu, 09 Feb 2023 12:13:28 GMT  
		Size: 64.5 MB (64509900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622e78faebf5b8024d64bf97cbc1e0a1a2ef6e8ed2fddbb16abfc817471fc463`  
		Last Modified: Thu, 09 Feb 2023 12:13:11 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.11` - linux; s390x

```console
$ docker pull varnish@sha256:df592d2c04da7cb2ee2144d4d971e719e7a60555c989bb86dde0d6c56089a79f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.0 MB (81002185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73636281614290efddc6e2f074b73a8ae88c72ab5f8d5e59d9349b2e0b0203b4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 02:41:45 GMT
ADD file:dc3c16b50baeac5b9644e607c8df9606e9583f8598e3ba34bcdd69c669a5904c in / 
# Thu, 09 Feb 2023 02:41:46 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 04:36:52 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 04:41:52 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 09 Feb 2023 04:42:02 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 04:42:02 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 09 Feb 2023 04:42:03 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 04:42:03 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 04:42:04 GMT
CMD []
```

-	Layers:
	-	`sha256:c2f78940fdfbfc5ce5d1d3cff3c27a319451aeb3ec12ff2473073516907fbce9`  
		Last Modified: Thu, 09 Feb 2023 02:46:06 GMT  
		Size: 29.6 MB (29647513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745410423134e2a363bf94f19d54352747cc0d7d642545ec7a337ad28c334724`  
		Last Modified: Thu, 09 Feb 2023 04:43:20 GMT  
		Size: 51.4 MB (51353971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e967e8ebb718a1ca31b86298d62b3fdfdcf3fac94d321d34ba0754a9c55395`  
		Last Modified: Thu, 09 Feb 2023 04:43:14 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.1`

```console
$ docker pull varnish@sha256:e9456a472f77f375121d88078702733c80bccfa30f5ee471357f6c88d3193d8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:7.1` - linux; amd64

```console
$ docker pull varnish@sha256:86b5b917a68ee39dc513d1017569eb600357c1d773e0b29c7d7e936d41fdb968
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.5 MB (106537864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f711ef0df5359ec75fbc8ecfb0a6d7a3817bab883c77f1573ec780770b149fda`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:42:09 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 09 Feb 2023 06:42:09 GMT
ARG VARNISH_VERSION=7.1.2
# Thu, 09 Feb 2023 06:42:09 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Thu, 09 Feb 2023 06:42:09 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 09 Feb 2023 06:42:10 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 09 Feb 2023 06:42:10 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 09 Feb 2023 06:42:10 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 09 Feb 2023 06:42:10 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 09 Feb 2023 06:42:10 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 09 Feb 2023 06:42:10 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Thu, 09 Feb 2023 06:42:10 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 06:45:03 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.2.tgz -o $tmpdir/orig.tgz;     echo "e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 09 Feb 2023 06:45:03 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 06:45:03 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 09 Feb 2023 06:45:04 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 06:45:04 GMT
USER varnish
# Thu, 09 Feb 2023 06:45:04 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 06:45:04 GMT
CMD []
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45419548745e83c966d460c337d99ce0f8bc4197cd132a7152c2bee977289c2`  
		Last Modified: Thu, 09 Feb 2023 06:48:34 GMT  
		Size: 75.1 MB (75125563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9709f37aae9d1c1f49e6e2b5d00cfe737700ec9560876ea55e9f18b44cab188f`  
		Last Modified: Thu, 09 Feb 2023 06:48:24 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1` - linux; arm variant v7

```console
$ docker pull varnish@sha256:af440494a9fa63f6e01ab2de90f7511757acffa9f5a6a3d99091307b05143f7d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.9 MB (82883084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30142de2126bc95650930d00a49e560bf838c6bd56af0c704f1b89dd7277be67`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Sat, 04 Feb 2023 09:59:36 GMT
ADD file:c3cb8f4527fa96e99a4741ecb398113f25f53389c173b74f6c2a5e39a6575c60 in / 
# Sat, 04 Feb 2023 09:59:36 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 21:22:46 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Sat, 04 Feb 2023 21:22:46 GMT
ARG VARNISH_VERSION=7.1.2
# Sat, 04 Feb 2023 21:22:46 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Sat, 04 Feb 2023 21:22:46 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Sat, 04 Feb 2023 21:22:46 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Sat, 04 Feb 2023 21:22:46 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Sat, 04 Feb 2023 21:22:46 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Sat, 04 Feb 2023 21:22:46 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Sat, 04 Feb 2023 21:22:46 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Sat, 04 Feb 2023 21:22:46 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Sat, 04 Feb 2023 21:22:46 GMT
ENV VARNISH_SIZE=100M
# Sat, 04 Feb 2023 21:25:38 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.2.tgz -o $tmpdir/orig.tgz;     echo "e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Sat, 04 Feb 2023 21:25:39 GMT
WORKDIR /etc/varnish
# Sat, 04 Feb 2023 21:25:39 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Sat, 04 Feb 2023 21:25:39 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sat, 04 Feb 2023 21:25:39 GMT
USER varnish
# Sat, 04 Feb 2023 21:25:39 GMT
EXPOSE 80 8443
# Sat, 04 Feb 2023 21:25:39 GMT
CMD []
```

-	Layers:
	-	`sha256:bd25bcdfbaa165120ee21b6567df395fe7d7b38da3cca0bcecee55a190e04aab`  
		Last Modified: Sat, 04 Feb 2023 10:06:24 GMT  
		Size: 26.6 MB (26559474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a86cf7003c8f00c3a87657fb934e5c12a0414057288dcf7f8d1c94edb9d665`  
		Last Modified: Sat, 04 Feb 2023 21:29:54 GMT  
		Size: 56.3 MB (56323117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769df1d3e88475c39dda498ae716e7af2815967f933c5cede97335326f57ccaf`  
		Last Modified: Sat, 04 Feb 2023 21:29:45 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:0a30e53f8a879d0694179b1b1f4c333137a40a4b5f0c5333eb19073a96f2f37d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100553785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0280926bf0f5644eeb444f60b474c1f930ab6f2b993bef702237ef1acef0e39d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 08:47:05 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 09 Feb 2023 08:47:06 GMT
ARG VARNISH_VERSION=7.1.2
# Thu, 09 Feb 2023 08:47:06 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Thu, 09 Feb 2023 08:47:06 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 09 Feb 2023 08:47:06 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 09 Feb 2023 08:47:06 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 09 Feb 2023 08:47:06 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 09 Feb 2023 08:47:06 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 09 Feb 2023 08:47:06 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 09 Feb 2023 08:47:06 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Thu, 09 Feb 2023 08:47:06 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 08:49:24 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.2.tgz -o $tmpdir/orig.tgz;     echo "e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 09 Feb 2023 08:49:24 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 08:49:24 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 09 Feb 2023 08:49:24 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 08:49:24 GMT
USER varnish
# Thu, 09 Feb 2023 08:49:25 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 08:49:25 GMT
CMD []
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2d201a526e5c2cd221f64119321ea6485287d221c398880175d45ad922cac8`  
		Last Modified: Thu, 09 Feb 2023 08:52:21 GMT  
		Size: 70.5 MB (70490781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b57b0db05e8c4d5f84e5ec7882fce9b2d3f2e59ef0a762d685f38862463c76f`  
		Last Modified: Thu, 09 Feb 2023 08:52:13 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1` - linux; 386

```console
$ docker pull varnish@sha256:ca5c1980e1e095a68397f8b5823d53ebebeb77685c42b22e5e2c20ad2f87121a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.9 MB (107917601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43ff32c9d6df2db2894a8b138d4ed404865bd95b5ba4c2cf7db9d4795031ab1f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 05:12:53 GMT
ADD file:7740abd3129d33122ce51153c0b6c3323b9cbe9ea0e81672e16b2d7b210d24e3 in / 
# Thu, 09 Feb 2023 05:12:53 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 11:32:02 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 09 Feb 2023 11:32:03 GMT
ARG VARNISH_VERSION=7.1.2
# Thu, 09 Feb 2023 11:32:04 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Thu, 09 Feb 2023 11:32:05 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 09 Feb 2023 11:32:06 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 09 Feb 2023 11:32:07 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 09 Feb 2023 11:32:08 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 09 Feb 2023 11:32:09 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 09 Feb 2023 11:32:10 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 09 Feb 2023 11:32:11 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Thu, 09 Feb 2023 11:32:12 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 11:35:05 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.2.tgz -o $tmpdir/orig.tgz;     echo "e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 09 Feb 2023 11:35:05 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 11:35:07 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 09 Feb 2023 11:35:07 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 11:35:08 GMT
USER varnish
# Thu, 09 Feb 2023 11:35:09 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 11:35:10 GMT
CMD []
```

-	Layers:
	-	`sha256:20744f4988404b1dee2cd438157b288d16a89da472583c0f04332ed389b258f8`  
		Last Modified: Thu, 09 Feb 2023 05:18:42 GMT  
		Size: 32.4 MB (32396875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0573a6fdb6f67f86faa1dce42564d76e6997e8130436cdf49ba43e7953a4411`  
		Last Modified: Thu, 09 Feb 2023 11:37:10 GMT  
		Size: 75.5 MB (75520232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6184742911a33db3f684db4f78b9b476388a95e13bc7d5c92e880436dc0ba6`  
		Last Modified: Thu, 09 Feb 2023 11:37:01 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1` - linux; ppc64le

```console
$ docker pull varnish@sha256:a66bc11c56528ecd014a1e98d6ec8dc78342780cb7ee86f27e13fdaf727b578a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.8 MB (105819665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:564f0c4cff12c34e206ca62da60e6adc2167316b48e5be13d5879104a4cfd813`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 06:21:49 GMT
ADD file:b09577b8131a90731fdfb00b824a97dc65ccb51d484cb9004382035d64a5741c in / 
# Thu, 09 Feb 2023 06:21:52 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 11:56:55 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 09 Feb 2023 11:56:56 GMT
ARG VARNISH_VERSION=7.1.2
# Thu, 09 Feb 2023 11:56:56 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Thu, 09 Feb 2023 11:56:57 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 09 Feb 2023 11:56:57 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 09 Feb 2023 11:56:58 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 09 Feb 2023 11:56:58 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 09 Feb 2023 11:56:58 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 09 Feb 2023 11:56:59 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 09 Feb 2023 11:56:59 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Thu, 09 Feb 2023 11:56:59 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 12:04:06 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.2.tgz -o $tmpdir/orig.tgz;     echo "e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 09 Feb 2023 12:04:09 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 12:04:10 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 09 Feb 2023 12:04:10 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 12:04:11 GMT
USER varnish
# Thu, 09 Feb 2023 12:04:11 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 12:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:4ea90e1a094ae86c7950bbec99e7a79b08fae641ad5f3bc3af9081c925894c41`  
		Last Modified: Thu, 09 Feb 2023 06:28:27 GMT  
		Size: 35.3 MB (35289252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae58755fff07f0f195cbf87771a105e6741fe9dfeec0b41be3d8034b67cfbe9e`  
		Last Modified: Thu, 09 Feb 2023 12:12:56 GMT  
		Size: 70.5 MB (70529918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e616fbd77e4b0b793bea388a655624c763b53737dcaa1c492e7b39385e583c1`  
		Last Modified: Thu, 09 Feb 2023 12:12:38 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1` - linux; s390x

```console
$ docker pull varnish@sha256:e75e34fba93f3f32d106700d4e93c5c9707eb9eb32058da5f1328e8e4ad5d27c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.8 MB (86833950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aebf2a458caabeda0bd00d1cba9bbc14c65034713a39b9385e47c504a9ac5036`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:43:11 GMT
ADD file:c1d41928e802c0b63beb07130c33bcc6dbdeb380a7f47510163cb176891e682a in / 
# Wed, 21 Dec 2022 01:43:14 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 10:26:01 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Wed, 21 Dec 2022 10:26:02 GMT
ARG VARNISH_VERSION=7.1.2
# Wed, 21 Dec 2022 10:26:02 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Wed, 21 Dec 2022 10:26:02 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Wed, 21 Dec 2022 10:26:02 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Wed, 21 Dec 2022 10:26:02 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Wed, 21 Dec 2022 10:26:03 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Wed, 21 Dec 2022 10:26:03 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Wed, 21 Dec 2022 10:26:03 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 21 Dec 2022 10:26:03 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 21 Dec 2022 10:26:04 GMT
ENV VARNISH_SIZE=100M
# Tue, 10 Jan 2023 01:41:58 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.2.tgz -o $tmpdir/orig.tgz;     echo "e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 10 Jan 2023 01:42:07 GMT
WORKDIR /etc/varnish
# Tue, 10 Jan 2023 01:42:07 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 10 Jan 2023 01:42:08 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 10 Jan 2023 01:42:08 GMT
USER varnish
# Tue, 10 Jan 2023 01:42:09 GMT
EXPOSE 80 8443
# Tue, 10 Jan 2023 01:42:09 GMT
CMD []
```

-	Layers:
	-	`sha256:197dcf20f55386b4c3f5fbace4720b64b5b0b606658b4ea9925121b9dbe7d638`  
		Last Modified: Wed, 21 Dec 2022 01:49:12 GMT  
		Size: 29.6 MB (29629760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d4c9c347e9b7f6ec4e2913f77427f763121ee4c5c1581c98442b5f1196eaa1`  
		Last Modified: Tue, 10 Jan 2023 01:43:26 GMT  
		Size: 57.2 MB (57203697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44b8332de2d27a2172b14f1b3da08d4945e94d884acb16dc735410d206be275`  
		Last Modified: Tue, 10 Jan 2023 01:43:18 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.1-alpine`

```console
$ docker pull varnish@sha256:3331356f8f0755e4e3ed11e499aede3598eb762db833fc1d8061c11327c9c212
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:7.1-alpine` - linux; amd64

```console
$ docker pull varnish@sha256:bfc65610836fc2c37e08b84bb6f240889b355da18b842eb9348067d7750f04ce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.1 MB (59090797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3cdb897373eeab8d7f7fc2ff61e7991f4a238437ede05a3ff5bf9848fc43411`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:24:33 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 08 Nov 2022 19:01:38 GMT
ARG VARNISH_VERSION=7.1.2
# Tue, 08 Nov 2022 19:01:38 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Tue, 08 Nov 2022 19:01:38 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 08 Nov 2022 19:01:38 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 08 Nov 2022 19:01:38 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 08 Nov 2022 19:01:39 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 08 Nov 2022 19:01:39 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 08 Nov 2022 19:01:39 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 08 Nov 2022 19:01:39 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Tue, 08 Nov 2022 19:01:39 GMT
ENV VARNISH_SIZE=100M
# Tue, 08 Nov 2022 19:02:55 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Tue, 08 Nov 2022 19:02:55 GMT
WORKDIR /etc/varnish
# Tue, 08 Nov 2022 19:02:55 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 08 Nov 2022 19:02:55 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 08 Nov 2022 19:02:55 GMT
USER varnish
# Tue, 08 Nov 2022 19:02:55 GMT
EXPOSE 80 8443
# Tue, 08 Nov 2022 19:02:56 GMT
CMD []
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670d3e80e9abfb3a928cc7c4731595397e55cb0ce688957e59cfd484638c4232`  
		Last Modified: Tue, 08 Nov 2022 19:07:01 GMT  
		Size: 56.3 MB (56266789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c2c314e27890a793acce697402def118c2653924d827e52bbf967c8bda1928`  
		Last Modified: Tue, 08 Nov 2022 19:06:54 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:e4973a41b8c02a57dea2fbde4bf421a8a8ffdb78fb88965bd67696865b0d0f22
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44857379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7619084158717a1a17c4ed5501e554e505399f0a94aab05362677d3a16b044fd`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 10 Nov 2022 19:57:41 GMT
ADD file:0bd18306f21937a9572e68c768f05f4a9d8341b40c2379a7bfcb857c77734a14 in / 
# Thu, 10 Nov 2022 19:57:41 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 13:53:37 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Fri, 11 Nov 2022 13:53:37 GMT
ARG VARNISH_VERSION=7.1.2
# Fri, 11 Nov 2022 13:53:37 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Fri, 11 Nov 2022 13:53:37 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Fri, 11 Nov 2022 13:53:37 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Fri, 11 Nov 2022 13:53:37 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 11 Nov 2022 13:53:37 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Fri, 11 Nov 2022 13:53:37 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Fri, 11 Nov 2022 13:53:38 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 11 Nov 2022 13:53:38 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Fri, 11 Nov 2022 13:53:38 GMT
ENV VARNISH_SIZE=100M
# Fri, 11 Nov 2022 13:54:56 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 11 Nov 2022 13:54:56 GMT
WORKDIR /etc/varnish
# Fri, 11 Nov 2022 13:54:56 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 11 Nov 2022 13:54:56 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 11 Nov 2022 13:54:56 GMT
USER varnish
# Fri, 11 Nov 2022 13:54:57 GMT
EXPOSE 80 8443
# Fri, 11 Nov 2022 13:54:57 GMT
CMD []
```

-	Layers:
	-	`sha256:59775c20a906b1a49edcdc41a700a795998979d6ecf8f8d9cd7cbdf45e686d81`  
		Last Modified: Tue, 09 Aug 2022 16:59:12 GMT  
		Size: 2.4 MB (2435092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2419579e60811439aabf58796ee9d89983cd314305eeeab0808489234c9db1a7`  
		Last Modified: Fri, 11 Nov 2022 13:56:32 GMT  
		Size: 42.4 MB (42421790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55eae22e1ead549cfa2f80d74a145fa6455e60c7660da0ca8752ec2383251fd9`  
		Last Modified: Fri, 11 Nov 2022 13:56:26 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:6f2a92bc4631e45fdf46e30ca2a678fc18d69a796794c78081fdfb2177539796
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51821334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef8b0ea598ca779a5b17a6cfc945f5fb7924556f05fb2363b5f9036b0e174ad4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:11:27 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Fri, 11 Nov 2022 11:11:27 GMT
ARG VARNISH_VERSION=7.1.2
# Fri, 11 Nov 2022 11:11:27 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Fri, 11 Nov 2022 11:11:27 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Fri, 11 Nov 2022 11:11:27 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Fri, 11 Nov 2022 11:11:27 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 11 Nov 2022 11:11:27 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Fri, 11 Nov 2022 11:11:27 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Fri, 11 Nov 2022 11:11:27 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 11 Nov 2022 11:11:27 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Fri, 11 Nov 2022 11:11:27 GMT
ENV VARNISH_SIZE=100M
# Fri, 11 Nov 2022 11:12:31 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 11 Nov 2022 11:12:31 GMT
WORKDIR /etc/varnish
# Fri, 11 Nov 2022 11:12:31 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 11 Nov 2022 11:12:31 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 11 Nov 2022 11:12:32 GMT
USER varnish
# Fri, 11 Nov 2022 11:12:32 GMT
EXPOSE 80 8443
# Fri, 11 Nov 2022 11:12:32 GMT
CMD []
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc75e4f36dbe8d71a5eaf0e56fba0e90226526c5e3759babf17ba6a3e553ce47`  
		Last Modified: Fri, 11 Nov 2022 11:12:57 GMT  
		Size: 49.1 MB (49102395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6324f8809992cfd331bdcf3e0f499b98535fbf7427ae9168308687cf0567305a`  
		Last Modified: Fri, 11 Nov 2022 11:12:51 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1-alpine` - linux; 386

```console
$ docker pull varnish@sha256:b3f5feb5d221bd9c13b856c10cb0120b95291c7e4f7fdb927fe08ec4ad1e88ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.3 MB (59279274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67b581c96ccf8b2633e4f6c79db5ce762a929d95d479de81e844126a865f8c8d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 02:12:55 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 08 Nov 2022 18:44:36 GMT
ARG VARNISH_VERSION=7.1.2
# Tue, 08 Nov 2022 18:44:37 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Tue, 08 Nov 2022 18:44:38 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 08 Nov 2022 18:44:39 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 08 Nov 2022 18:44:40 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 08 Nov 2022 18:44:41 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 08 Nov 2022 18:44:42 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 08 Nov 2022 18:44:43 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 08 Nov 2022 18:44:44 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Tue, 08 Nov 2022 18:44:45 GMT
ENV VARNISH_SIZE=100M
# Tue, 08 Nov 2022 18:46:00 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Tue, 08 Nov 2022 18:46:00 GMT
WORKDIR /etc/varnish
# Tue, 08 Nov 2022 18:46:02 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 08 Nov 2022 18:46:02 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 08 Nov 2022 18:46:03 GMT
USER varnish
# Tue, 08 Nov 2022 18:46:04 GMT
EXPOSE 80 8443
# Tue, 08 Nov 2022 18:46:05 GMT
CMD []
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b7b64086583adaf8e717a764baa8e1e5518939598e37bfbd3d5d8a10b16099`  
		Last Modified: Tue, 08 Nov 2022 18:48:14 GMT  
		Size: 56.5 MB (56450259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e960ed7e731a3a4de714a5163ea0b5b051db544035426db396aede8d60d4a2`  
		Last Modified: Tue, 08 Nov 2022 18:48:07 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:fd13ff160f58772d17c34ea5366635adea6934f90965f814bbff7809a81e1956
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48891152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14848d3913a9ba32f1c0a797e633fd7c7b24673f71f8b6d95ff4f31c6a8cb674`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:17:20 GMT
ADD file:be31abb0aba89ed5ff9200736a1c46091abc3845d0e332efd5e5c874ef2c99d1 in / 
# Tue, 09 Aug 2022 17:17:21 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:52:54 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 08 Nov 2022 22:32:34 GMT
ARG VARNISH_VERSION=7.1.2
# Tue, 08 Nov 2022 22:32:35 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Tue, 08 Nov 2022 22:32:35 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 08 Nov 2022 22:32:35 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 08 Nov 2022 22:32:35 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 08 Nov 2022 22:32:36 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 08 Nov 2022 22:32:37 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 08 Nov 2022 22:32:37 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 08 Nov 2022 22:32:38 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Tue, 08 Nov 2022 22:32:38 GMT
ENV VARNISH_SIZE=100M
# Tue, 08 Nov 2022 22:34:25 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Tue, 08 Nov 2022 22:34:27 GMT
WORKDIR /etc/varnish
# Tue, 08 Nov 2022 22:34:27 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 08 Nov 2022 22:34:28 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 08 Nov 2022 22:34:28 GMT
USER varnish
# Tue, 08 Nov 2022 22:34:29 GMT
EXPOSE 80 8443
# Tue, 08 Nov 2022 22:34:29 GMT
CMD []
```

-	Layers:
	-	`sha256:deb7065b3304c3a9834f31b8a53e8d6089060e9c6522668abd22f1f4d9f52ca7`  
		Last Modified: Tue, 09 Aug 2022 17:18:45 GMT  
		Size: 2.8 MB (2812989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fa6b482f0aa86974b6985a7ec840d7f1efd96cf825f3b458d93f6957be2dc2`  
		Last Modified: Tue, 08 Nov 2022 22:41:17 GMT  
		Size: 46.1 MB (46077664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d52f90e5fa0cbf3d9c1dcc9b50fba21e6e1c849ed28b7dba4cccc2caea937c`  
		Last Modified: Tue, 08 Nov 2022 22:41:05 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:cd614f6294b6623abcc8e6b95a192e7bbcf1ee7eb7fde1c7fb8b25c5caeaa136
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.3 MB (47345351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39158646bb7f7dd43a83f88c405b6e61369cb1d9ca741da81aa7660e3efe3720`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 10:18:49 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 08 Nov 2022 18:22:21 GMT
ARG VARNISH_VERSION=7.1.2
# Tue, 08 Nov 2022 18:22:22 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Tue, 08 Nov 2022 18:22:22 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 08 Nov 2022 18:22:23 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 08 Nov 2022 18:22:24 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 08 Nov 2022 18:22:24 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 08 Nov 2022 18:22:25 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 08 Nov 2022 18:22:25 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 08 Nov 2022 18:22:26 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Tue, 08 Nov 2022 18:22:26 GMT
ENV VARNISH_SIZE=100M
# Tue, 08 Nov 2022 18:25:11 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Tue, 08 Nov 2022 18:25:17 GMT
WORKDIR /etc/varnish
# Tue, 08 Nov 2022 18:25:18 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 08 Nov 2022 18:25:19 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 08 Nov 2022 18:25:19 GMT
USER varnish
# Tue, 08 Nov 2022 18:25:20 GMT
EXPOSE 80 8443
# Tue, 08 Nov 2022 18:25:21 GMT
CMD []
```

-	Layers:
	-	`sha256:cdf710f5b7ee39c5124c50c753228dc9b8b1c1c0a1a38f1413487548565445c3`  
		Last Modified: Tue, 09 Aug 2022 17:42:56 GMT  
		Size: 2.6 MB (2606087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9702764c9fb92996851b17f3da01efeb6e89bafbae74f375e28b8be5391f2ace`  
		Last Modified: Tue, 08 Nov 2022 18:27:39 GMT  
		Size: 44.7 MB (44738766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e185d30ef72fbdb2cf68aded1268dc798f233bdb4dddb8e273a4c909f52bb5`  
		Last Modified: Tue, 08 Nov 2022 18:27:34 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.1.2`

```console
$ docker pull varnish@sha256:e9456a472f77f375121d88078702733c80bccfa30f5ee471357f6c88d3193d8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:7.1.2` - linux; amd64

```console
$ docker pull varnish@sha256:86b5b917a68ee39dc513d1017569eb600357c1d773e0b29c7d7e936d41fdb968
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.5 MB (106537864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f711ef0df5359ec75fbc8ecfb0a6d7a3817bab883c77f1573ec780770b149fda`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:42:09 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 09 Feb 2023 06:42:09 GMT
ARG VARNISH_VERSION=7.1.2
# Thu, 09 Feb 2023 06:42:09 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Thu, 09 Feb 2023 06:42:09 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 09 Feb 2023 06:42:10 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 09 Feb 2023 06:42:10 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 09 Feb 2023 06:42:10 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 09 Feb 2023 06:42:10 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 09 Feb 2023 06:42:10 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 09 Feb 2023 06:42:10 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Thu, 09 Feb 2023 06:42:10 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 06:45:03 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.2.tgz -o $tmpdir/orig.tgz;     echo "e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 09 Feb 2023 06:45:03 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 06:45:03 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 09 Feb 2023 06:45:04 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 06:45:04 GMT
USER varnish
# Thu, 09 Feb 2023 06:45:04 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 06:45:04 GMT
CMD []
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45419548745e83c966d460c337d99ce0f8bc4197cd132a7152c2bee977289c2`  
		Last Modified: Thu, 09 Feb 2023 06:48:34 GMT  
		Size: 75.1 MB (75125563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9709f37aae9d1c1f49e6e2b5d00cfe737700ec9560876ea55e9f18b44cab188f`  
		Last Modified: Thu, 09 Feb 2023 06:48:24 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1.2` - linux; arm variant v7

```console
$ docker pull varnish@sha256:af440494a9fa63f6e01ab2de90f7511757acffa9f5a6a3d99091307b05143f7d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.9 MB (82883084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30142de2126bc95650930d00a49e560bf838c6bd56af0c704f1b89dd7277be67`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Sat, 04 Feb 2023 09:59:36 GMT
ADD file:c3cb8f4527fa96e99a4741ecb398113f25f53389c173b74f6c2a5e39a6575c60 in / 
# Sat, 04 Feb 2023 09:59:36 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 21:22:46 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Sat, 04 Feb 2023 21:22:46 GMT
ARG VARNISH_VERSION=7.1.2
# Sat, 04 Feb 2023 21:22:46 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Sat, 04 Feb 2023 21:22:46 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Sat, 04 Feb 2023 21:22:46 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Sat, 04 Feb 2023 21:22:46 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Sat, 04 Feb 2023 21:22:46 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Sat, 04 Feb 2023 21:22:46 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Sat, 04 Feb 2023 21:22:46 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Sat, 04 Feb 2023 21:22:46 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Sat, 04 Feb 2023 21:22:46 GMT
ENV VARNISH_SIZE=100M
# Sat, 04 Feb 2023 21:25:38 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.2.tgz -o $tmpdir/orig.tgz;     echo "e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Sat, 04 Feb 2023 21:25:39 GMT
WORKDIR /etc/varnish
# Sat, 04 Feb 2023 21:25:39 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Sat, 04 Feb 2023 21:25:39 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sat, 04 Feb 2023 21:25:39 GMT
USER varnish
# Sat, 04 Feb 2023 21:25:39 GMT
EXPOSE 80 8443
# Sat, 04 Feb 2023 21:25:39 GMT
CMD []
```

-	Layers:
	-	`sha256:bd25bcdfbaa165120ee21b6567df395fe7d7b38da3cca0bcecee55a190e04aab`  
		Last Modified: Sat, 04 Feb 2023 10:06:24 GMT  
		Size: 26.6 MB (26559474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a86cf7003c8f00c3a87657fb934e5c12a0414057288dcf7f8d1c94edb9d665`  
		Last Modified: Sat, 04 Feb 2023 21:29:54 GMT  
		Size: 56.3 MB (56323117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769df1d3e88475c39dda498ae716e7af2815967f933c5cede97335326f57ccaf`  
		Last Modified: Sat, 04 Feb 2023 21:29:45 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1.2` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:0a30e53f8a879d0694179b1b1f4c333137a40a4b5f0c5333eb19073a96f2f37d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100553785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0280926bf0f5644eeb444f60b474c1f930ab6f2b993bef702237ef1acef0e39d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 08:47:05 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 09 Feb 2023 08:47:06 GMT
ARG VARNISH_VERSION=7.1.2
# Thu, 09 Feb 2023 08:47:06 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Thu, 09 Feb 2023 08:47:06 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 09 Feb 2023 08:47:06 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 09 Feb 2023 08:47:06 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 09 Feb 2023 08:47:06 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 09 Feb 2023 08:47:06 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 09 Feb 2023 08:47:06 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 09 Feb 2023 08:47:06 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Thu, 09 Feb 2023 08:47:06 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 08:49:24 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.2.tgz -o $tmpdir/orig.tgz;     echo "e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 09 Feb 2023 08:49:24 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 08:49:24 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 09 Feb 2023 08:49:24 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 08:49:24 GMT
USER varnish
# Thu, 09 Feb 2023 08:49:25 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 08:49:25 GMT
CMD []
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2d201a526e5c2cd221f64119321ea6485287d221c398880175d45ad922cac8`  
		Last Modified: Thu, 09 Feb 2023 08:52:21 GMT  
		Size: 70.5 MB (70490781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b57b0db05e8c4d5f84e5ec7882fce9b2d3f2e59ef0a762d685f38862463c76f`  
		Last Modified: Thu, 09 Feb 2023 08:52:13 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1.2` - linux; 386

```console
$ docker pull varnish@sha256:ca5c1980e1e095a68397f8b5823d53ebebeb77685c42b22e5e2c20ad2f87121a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.9 MB (107917601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43ff32c9d6df2db2894a8b138d4ed404865bd95b5ba4c2cf7db9d4795031ab1f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 05:12:53 GMT
ADD file:7740abd3129d33122ce51153c0b6c3323b9cbe9ea0e81672e16b2d7b210d24e3 in / 
# Thu, 09 Feb 2023 05:12:53 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 11:32:02 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 09 Feb 2023 11:32:03 GMT
ARG VARNISH_VERSION=7.1.2
# Thu, 09 Feb 2023 11:32:04 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Thu, 09 Feb 2023 11:32:05 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 09 Feb 2023 11:32:06 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 09 Feb 2023 11:32:07 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 09 Feb 2023 11:32:08 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 09 Feb 2023 11:32:09 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 09 Feb 2023 11:32:10 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 09 Feb 2023 11:32:11 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Thu, 09 Feb 2023 11:32:12 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 11:35:05 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.2.tgz -o $tmpdir/orig.tgz;     echo "e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 09 Feb 2023 11:35:05 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 11:35:07 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 09 Feb 2023 11:35:07 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 11:35:08 GMT
USER varnish
# Thu, 09 Feb 2023 11:35:09 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 11:35:10 GMT
CMD []
```

-	Layers:
	-	`sha256:20744f4988404b1dee2cd438157b288d16a89da472583c0f04332ed389b258f8`  
		Last Modified: Thu, 09 Feb 2023 05:18:42 GMT  
		Size: 32.4 MB (32396875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0573a6fdb6f67f86faa1dce42564d76e6997e8130436cdf49ba43e7953a4411`  
		Last Modified: Thu, 09 Feb 2023 11:37:10 GMT  
		Size: 75.5 MB (75520232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6184742911a33db3f684db4f78b9b476388a95e13bc7d5c92e880436dc0ba6`  
		Last Modified: Thu, 09 Feb 2023 11:37:01 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1.2` - linux; ppc64le

```console
$ docker pull varnish@sha256:a66bc11c56528ecd014a1e98d6ec8dc78342780cb7ee86f27e13fdaf727b578a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.8 MB (105819665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:564f0c4cff12c34e206ca62da60e6adc2167316b48e5be13d5879104a4cfd813`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 06:21:49 GMT
ADD file:b09577b8131a90731fdfb00b824a97dc65ccb51d484cb9004382035d64a5741c in / 
# Thu, 09 Feb 2023 06:21:52 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 11:56:55 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 09 Feb 2023 11:56:56 GMT
ARG VARNISH_VERSION=7.1.2
# Thu, 09 Feb 2023 11:56:56 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Thu, 09 Feb 2023 11:56:57 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 09 Feb 2023 11:56:57 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 09 Feb 2023 11:56:58 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 09 Feb 2023 11:56:58 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 09 Feb 2023 11:56:58 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 09 Feb 2023 11:56:59 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 09 Feb 2023 11:56:59 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Thu, 09 Feb 2023 11:56:59 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 12:04:06 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.2.tgz -o $tmpdir/orig.tgz;     echo "e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 09 Feb 2023 12:04:09 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 12:04:10 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 09 Feb 2023 12:04:10 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 12:04:11 GMT
USER varnish
# Thu, 09 Feb 2023 12:04:11 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 12:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:4ea90e1a094ae86c7950bbec99e7a79b08fae641ad5f3bc3af9081c925894c41`  
		Last Modified: Thu, 09 Feb 2023 06:28:27 GMT  
		Size: 35.3 MB (35289252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae58755fff07f0f195cbf87771a105e6741fe9dfeec0b41be3d8034b67cfbe9e`  
		Last Modified: Thu, 09 Feb 2023 12:12:56 GMT  
		Size: 70.5 MB (70529918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e616fbd77e4b0b793bea388a655624c763b53737dcaa1c492e7b39385e583c1`  
		Last Modified: Thu, 09 Feb 2023 12:12:38 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1.2` - linux; s390x

```console
$ docker pull varnish@sha256:e75e34fba93f3f32d106700d4e93c5c9707eb9eb32058da5f1328e8e4ad5d27c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.8 MB (86833950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aebf2a458caabeda0bd00d1cba9bbc14c65034713a39b9385e47c504a9ac5036`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:43:11 GMT
ADD file:c1d41928e802c0b63beb07130c33bcc6dbdeb380a7f47510163cb176891e682a in / 
# Wed, 21 Dec 2022 01:43:14 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 10:26:01 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Wed, 21 Dec 2022 10:26:02 GMT
ARG VARNISH_VERSION=7.1.2
# Wed, 21 Dec 2022 10:26:02 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Wed, 21 Dec 2022 10:26:02 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Wed, 21 Dec 2022 10:26:02 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Wed, 21 Dec 2022 10:26:02 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Wed, 21 Dec 2022 10:26:03 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Wed, 21 Dec 2022 10:26:03 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Wed, 21 Dec 2022 10:26:03 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 21 Dec 2022 10:26:03 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 21 Dec 2022 10:26:04 GMT
ENV VARNISH_SIZE=100M
# Tue, 10 Jan 2023 01:41:58 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.2.tgz -o $tmpdir/orig.tgz;     echo "e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 10 Jan 2023 01:42:07 GMT
WORKDIR /etc/varnish
# Tue, 10 Jan 2023 01:42:07 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 10 Jan 2023 01:42:08 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 10 Jan 2023 01:42:08 GMT
USER varnish
# Tue, 10 Jan 2023 01:42:09 GMT
EXPOSE 80 8443
# Tue, 10 Jan 2023 01:42:09 GMT
CMD []
```

-	Layers:
	-	`sha256:197dcf20f55386b4c3f5fbace4720b64b5b0b606658b4ea9925121b9dbe7d638`  
		Last Modified: Wed, 21 Dec 2022 01:49:12 GMT  
		Size: 29.6 MB (29629760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d4c9c347e9b7f6ec4e2913f77427f763121ee4c5c1581c98442b5f1196eaa1`  
		Last Modified: Tue, 10 Jan 2023 01:43:26 GMT  
		Size: 57.2 MB (57203697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44b8332de2d27a2172b14f1b3da08d4945e94d884acb16dc735410d206be275`  
		Last Modified: Tue, 10 Jan 2023 01:43:18 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.1.2-alpine`

```console
$ docker pull varnish@sha256:3331356f8f0755e4e3ed11e499aede3598eb762db833fc1d8061c11327c9c212
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:7.1.2-alpine` - linux; amd64

```console
$ docker pull varnish@sha256:bfc65610836fc2c37e08b84bb6f240889b355da18b842eb9348067d7750f04ce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.1 MB (59090797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3cdb897373eeab8d7f7fc2ff61e7991f4a238437ede05a3ff5bf9848fc43411`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:24:33 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 08 Nov 2022 19:01:38 GMT
ARG VARNISH_VERSION=7.1.2
# Tue, 08 Nov 2022 19:01:38 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Tue, 08 Nov 2022 19:01:38 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 08 Nov 2022 19:01:38 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 08 Nov 2022 19:01:38 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 08 Nov 2022 19:01:39 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 08 Nov 2022 19:01:39 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 08 Nov 2022 19:01:39 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 08 Nov 2022 19:01:39 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Tue, 08 Nov 2022 19:01:39 GMT
ENV VARNISH_SIZE=100M
# Tue, 08 Nov 2022 19:02:55 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Tue, 08 Nov 2022 19:02:55 GMT
WORKDIR /etc/varnish
# Tue, 08 Nov 2022 19:02:55 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 08 Nov 2022 19:02:55 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 08 Nov 2022 19:02:55 GMT
USER varnish
# Tue, 08 Nov 2022 19:02:55 GMT
EXPOSE 80 8443
# Tue, 08 Nov 2022 19:02:56 GMT
CMD []
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670d3e80e9abfb3a928cc7c4731595397e55cb0ce688957e59cfd484638c4232`  
		Last Modified: Tue, 08 Nov 2022 19:07:01 GMT  
		Size: 56.3 MB (56266789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c2c314e27890a793acce697402def118c2653924d827e52bbf967c8bda1928`  
		Last Modified: Tue, 08 Nov 2022 19:06:54 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1.2-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:e4973a41b8c02a57dea2fbde4bf421a8a8ffdb78fb88965bd67696865b0d0f22
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44857379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7619084158717a1a17c4ed5501e554e505399f0a94aab05362677d3a16b044fd`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 10 Nov 2022 19:57:41 GMT
ADD file:0bd18306f21937a9572e68c768f05f4a9d8341b40c2379a7bfcb857c77734a14 in / 
# Thu, 10 Nov 2022 19:57:41 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 13:53:37 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Fri, 11 Nov 2022 13:53:37 GMT
ARG VARNISH_VERSION=7.1.2
# Fri, 11 Nov 2022 13:53:37 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Fri, 11 Nov 2022 13:53:37 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Fri, 11 Nov 2022 13:53:37 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Fri, 11 Nov 2022 13:53:37 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 11 Nov 2022 13:53:37 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Fri, 11 Nov 2022 13:53:37 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Fri, 11 Nov 2022 13:53:38 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 11 Nov 2022 13:53:38 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Fri, 11 Nov 2022 13:53:38 GMT
ENV VARNISH_SIZE=100M
# Fri, 11 Nov 2022 13:54:56 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 11 Nov 2022 13:54:56 GMT
WORKDIR /etc/varnish
# Fri, 11 Nov 2022 13:54:56 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 11 Nov 2022 13:54:56 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 11 Nov 2022 13:54:56 GMT
USER varnish
# Fri, 11 Nov 2022 13:54:57 GMT
EXPOSE 80 8443
# Fri, 11 Nov 2022 13:54:57 GMT
CMD []
```

-	Layers:
	-	`sha256:59775c20a906b1a49edcdc41a700a795998979d6ecf8f8d9cd7cbdf45e686d81`  
		Last Modified: Tue, 09 Aug 2022 16:59:12 GMT  
		Size: 2.4 MB (2435092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2419579e60811439aabf58796ee9d89983cd314305eeeab0808489234c9db1a7`  
		Last Modified: Fri, 11 Nov 2022 13:56:32 GMT  
		Size: 42.4 MB (42421790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55eae22e1ead549cfa2f80d74a145fa6455e60c7660da0ca8752ec2383251fd9`  
		Last Modified: Fri, 11 Nov 2022 13:56:26 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1.2-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:6f2a92bc4631e45fdf46e30ca2a678fc18d69a796794c78081fdfb2177539796
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51821334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef8b0ea598ca779a5b17a6cfc945f5fb7924556f05fb2363b5f9036b0e174ad4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:11:27 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Fri, 11 Nov 2022 11:11:27 GMT
ARG VARNISH_VERSION=7.1.2
# Fri, 11 Nov 2022 11:11:27 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Fri, 11 Nov 2022 11:11:27 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Fri, 11 Nov 2022 11:11:27 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Fri, 11 Nov 2022 11:11:27 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 11 Nov 2022 11:11:27 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Fri, 11 Nov 2022 11:11:27 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Fri, 11 Nov 2022 11:11:27 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 11 Nov 2022 11:11:27 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Fri, 11 Nov 2022 11:11:27 GMT
ENV VARNISH_SIZE=100M
# Fri, 11 Nov 2022 11:12:31 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 11 Nov 2022 11:12:31 GMT
WORKDIR /etc/varnish
# Fri, 11 Nov 2022 11:12:31 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 11 Nov 2022 11:12:31 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 11 Nov 2022 11:12:32 GMT
USER varnish
# Fri, 11 Nov 2022 11:12:32 GMT
EXPOSE 80 8443
# Fri, 11 Nov 2022 11:12:32 GMT
CMD []
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc75e4f36dbe8d71a5eaf0e56fba0e90226526c5e3759babf17ba6a3e553ce47`  
		Last Modified: Fri, 11 Nov 2022 11:12:57 GMT  
		Size: 49.1 MB (49102395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6324f8809992cfd331bdcf3e0f499b98535fbf7427ae9168308687cf0567305a`  
		Last Modified: Fri, 11 Nov 2022 11:12:51 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1.2-alpine` - linux; 386

```console
$ docker pull varnish@sha256:b3f5feb5d221bd9c13b856c10cb0120b95291c7e4f7fdb927fe08ec4ad1e88ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.3 MB (59279274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67b581c96ccf8b2633e4f6c79db5ce762a929d95d479de81e844126a865f8c8d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 02:12:55 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 08 Nov 2022 18:44:36 GMT
ARG VARNISH_VERSION=7.1.2
# Tue, 08 Nov 2022 18:44:37 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Tue, 08 Nov 2022 18:44:38 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 08 Nov 2022 18:44:39 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 08 Nov 2022 18:44:40 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 08 Nov 2022 18:44:41 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 08 Nov 2022 18:44:42 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 08 Nov 2022 18:44:43 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 08 Nov 2022 18:44:44 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Tue, 08 Nov 2022 18:44:45 GMT
ENV VARNISH_SIZE=100M
# Tue, 08 Nov 2022 18:46:00 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Tue, 08 Nov 2022 18:46:00 GMT
WORKDIR /etc/varnish
# Tue, 08 Nov 2022 18:46:02 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 08 Nov 2022 18:46:02 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 08 Nov 2022 18:46:03 GMT
USER varnish
# Tue, 08 Nov 2022 18:46:04 GMT
EXPOSE 80 8443
# Tue, 08 Nov 2022 18:46:05 GMT
CMD []
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b7b64086583adaf8e717a764baa8e1e5518939598e37bfbd3d5d8a10b16099`  
		Last Modified: Tue, 08 Nov 2022 18:48:14 GMT  
		Size: 56.5 MB (56450259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e960ed7e731a3a4de714a5163ea0b5b051db544035426db396aede8d60d4a2`  
		Last Modified: Tue, 08 Nov 2022 18:48:07 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1.2-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:fd13ff160f58772d17c34ea5366635adea6934f90965f814bbff7809a81e1956
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48891152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14848d3913a9ba32f1c0a797e633fd7c7b24673f71f8b6d95ff4f31c6a8cb674`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:17:20 GMT
ADD file:be31abb0aba89ed5ff9200736a1c46091abc3845d0e332efd5e5c874ef2c99d1 in / 
# Tue, 09 Aug 2022 17:17:21 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:52:54 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 08 Nov 2022 22:32:34 GMT
ARG VARNISH_VERSION=7.1.2
# Tue, 08 Nov 2022 22:32:35 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Tue, 08 Nov 2022 22:32:35 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 08 Nov 2022 22:32:35 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 08 Nov 2022 22:32:35 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 08 Nov 2022 22:32:36 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 08 Nov 2022 22:32:37 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 08 Nov 2022 22:32:37 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 08 Nov 2022 22:32:38 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Tue, 08 Nov 2022 22:32:38 GMT
ENV VARNISH_SIZE=100M
# Tue, 08 Nov 2022 22:34:25 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Tue, 08 Nov 2022 22:34:27 GMT
WORKDIR /etc/varnish
# Tue, 08 Nov 2022 22:34:27 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 08 Nov 2022 22:34:28 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 08 Nov 2022 22:34:28 GMT
USER varnish
# Tue, 08 Nov 2022 22:34:29 GMT
EXPOSE 80 8443
# Tue, 08 Nov 2022 22:34:29 GMT
CMD []
```

-	Layers:
	-	`sha256:deb7065b3304c3a9834f31b8a53e8d6089060e9c6522668abd22f1f4d9f52ca7`  
		Last Modified: Tue, 09 Aug 2022 17:18:45 GMT  
		Size: 2.8 MB (2812989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fa6b482f0aa86974b6985a7ec840d7f1efd96cf825f3b458d93f6957be2dc2`  
		Last Modified: Tue, 08 Nov 2022 22:41:17 GMT  
		Size: 46.1 MB (46077664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d52f90e5fa0cbf3d9c1dcc9b50fba21e6e1c849ed28b7dba4cccc2caea937c`  
		Last Modified: Tue, 08 Nov 2022 22:41:05 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1.2-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:cd614f6294b6623abcc8e6b95a192e7bbcf1ee7eb7fde1c7fb8b25c5caeaa136
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.3 MB (47345351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39158646bb7f7dd43a83f88c405b6e61369cb1d9ca741da81aa7660e3efe3720`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 10:18:49 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 08 Nov 2022 18:22:21 GMT
ARG VARNISH_VERSION=7.1.2
# Tue, 08 Nov 2022 18:22:22 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Tue, 08 Nov 2022 18:22:22 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 08 Nov 2022 18:22:23 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 08 Nov 2022 18:22:24 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 08 Nov 2022 18:22:24 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 08 Nov 2022 18:22:25 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 08 Nov 2022 18:22:25 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 08 Nov 2022 18:22:26 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Tue, 08 Nov 2022 18:22:26 GMT
ENV VARNISH_SIZE=100M
# Tue, 08 Nov 2022 18:25:11 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Tue, 08 Nov 2022 18:25:17 GMT
WORKDIR /etc/varnish
# Tue, 08 Nov 2022 18:25:18 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 08 Nov 2022 18:25:19 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 08 Nov 2022 18:25:19 GMT
USER varnish
# Tue, 08 Nov 2022 18:25:20 GMT
EXPOSE 80 8443
# Tue, 08 Nov 2022 18:25:21 GMT
CMD []
```

-	Layers:
	-	`sha256:cdf710f5b7ee39c5124c50c753228dc9b8b1c1c0a1a38f1413487548565445c3`  
		Last Modified: Tue, 09 Aug 2022 17:42:56 GMT  
		Size: 2.6 MB (2606087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9702764c9fb92996851b17f3da01efeb6e89bafbae74f375e28b8be5391f2ace`  
		Last Modified: Tue, 08 Nov 2022 18:27:39 GMT  
		Size: 44.7 MB (44738766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e185d30ef72fbdb2cf68aded1268dc798f233bdb4dddb8e273a4c909f52bb5`  
		Last Modified: Tue, 08 Nov 2022 18:27:34 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.2`

```console
$ docker pull varnish@sha256:3feac23caf88ff28673bcb4aa81ae8dd316e4476c260af1a2c6e201cfcf4786e
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
$ docker pull varnish@sha256:d64ca9b7756cb3a0eda02971eba4e2006311fc85c52ccd6e992475366ac5790a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106843191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16576fb65a911c2195ae8bb7ea33bf084f41b7348f2d20473af354a42e4f6761`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:38:29 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 09 Feb 2023 06:38:29 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 09 Feb 2023 06:38:29 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 09 Feb 2023 06:38:29 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 09 Feb 2023 06:38:29 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 09 Feb 2023 06:38:29 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 09 Feb 2023 06:38:29 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 09 Feb 2023 06:38:29 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 09 Feb 2023 06:38:30 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 09 Feb 2023 06:38:30 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Thu, 09 Feb 2023 06:38:30 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 06:41:50 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 09 Feb 2023 06:41:51 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 06:41:51 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 09 Feb 2023 06:41:51 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 06:41:51 GMT
USER varnish
# Thu, 09 Feb 2023 06:41:51 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 06:41:51 GMT
CMD []
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5849700d1633b0858d2a64844bb0fdd45c87607fcf429d07dbcacf1835ff2e0f`  
		Last Modified: Thu, 09 Feb 2023 06:48:10 GMT  
		Size: 75.4 MB (75430887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819e8388a2fe25ed89691731d6a3f4a2feb9a30cf8db8de9a72ef699909ea329`  
		Last Modified: Thu, 09 Feb 2023 06:48:00 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2` - linux; arm variant v7

```console
$ docker pull varnish@sha256:667101f4287db71b7a21b99ed03b1190bf6ffec44a07c12406fac8f710cf287a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.2 MB (83169412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:293472e275cc824b762c201d32db85c29c22ad7c0462959504240f5c74f3f3b9`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Sat, 04 Feb 2023 09:59:36 GMT
ADD file:c3cb8f4527fa96e99a4741ecb398113f25f53389c173b74f6c2a5e39a6575c60 in / 
# Sat, 04 Feb 2023 09:59:36 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 21:19:28 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Sat, 04 Feb 2023 21:19:28 GMT
ARG VARNISH_VERSION=7.2.1
# Sat, 04 Feb 2023 21:19:28 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Sat, 04 Feb 2023 21:19:28 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Sat, 04 Feb 2023 21:19:29 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Sat, 04 Feb 2023 21:19:29 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Sat, 04 Feb 2023 21:19:29 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Sat, 04 Feb 2023 21:19:29 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Sat, 04 Feb 2023 21:19:29 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Sat, 04 Feb 2023 21:19:29 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Sat, 04 Feb 2023 21:19:29 GMT
ENV VARNISH_SIZE=100M
# Sat, 04 Feb 2023 21:22:30 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Sat, 04 Feb 2023 21:22:31 GMT
WORKDIR /etc/varnish
# Sat, 04 Feb 2023 21:22:31 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Sat, 04 Feb 2023 21:22:31 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sat, 04 Feb 2023 21:22:31 GMT
USER varnish
# Sat, 04 Feb 2023 21:22:31 GMT
EXPOSE 80 8443
# Sat, 04 Feb 2023 21:22:31 GMT
CMD []
```

-	Layers:
	-	`sha256:bd25bcdfbaa165120ee21b6567df395fe7d7b38da3cca0bcecee55a190e04aab`  
		Last Modified: Sat, 04 Feb 2023 10:06:24 GMT  
		Size: 26.6 MB (26559474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32aa6224c75d142f0a76142fa8ebabe4a311fc4ce23351e0248c29b47989d8f6`  
		Last Modified: Sat, 04 Feb 2023 21:29:24 GMT  
		Size: 56.6 MB (56609446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67957e16f03a30cd49c3c133970df3e4af0ca6c1d3517ade7f271caf5c636dbf`  
		Last Modified: Sat, 04 Feb 2023 21:29:15 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:070c65da2b8faf580eec672e0db795ded6285b428e1d39254f88244f6d2ba8fe
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.9 MB (100867420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa825a96e8e9266a3bf0501d85a6d0b2d4176c29895bd7b07085738e302fe068`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 08:43:56 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 09 Feb 2023 08:43:56 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 09 Feb 2023 08:43:56 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 09 Feb 2023 08:43:56 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 09 Feb 2023 08:43:56 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 09 Feb 2023 08:43:56 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 09 Feb 2023 08:43:56 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 09 Feb 2023 08:43:56 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 09 Feb 2023 08:43:57 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 09 Feb 2023 08:43:57 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Thu, 09 Feb 2023 08:43:57 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 08:46:49 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 09 Feb 2023 08:46:50 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 08:46:50 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 09 Feb 2023 08:46:50 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 08:46:50 GMT
USER varnish
# Thu, 09 Feb 2023 08:46:50 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 08:46:50 GMT
CMD []
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd593e410516ba146ca282d48deef73a7e2eaef76c1020ca6e524bc5aa4a6078`  
		Last Modified: Thu, 09 Feb 2023 08:51:51 GMT  
		Size: 70.8 MB (70804416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4459f721e7b5112ddc4a759e70ea9f389dbe7ea84abed0cf252d75110b8a00b1`  
		Last Modified: Thu, 09 Feb 2023 08:51:45 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2` - linux; 386

```console
$ docker pull varnish@sha256:32e374f738c01546453d2edad6a6797b7eef8d9b4145e3a8f7cbb00886bf9aca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.2 MB (108223049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0847bbcdf260fc907bc7fc41a1e8607b6bab32fff55ecc9738733798c6d219e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 05:12:53 GMT
ADD file:7740abd3129d33122ce51153c0b6c3323b9cbe9ea0e81672e16b2d7b210d24e3 in / 
# Thu, 09 Feb 2023 05:12:53 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 11:28:46 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 09 Feb 2023 11:28:46 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 09 Feb 2023 11:28:47 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 09 Feb 2023 11:28:48 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 09 Feb 2023 11:28:49 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 09 Feb 2023 11:28:50 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 09 Feb 2023 11:28:51 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 09 Feb 2023 11:28:52 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 09 Feb 2023 11:28:53 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 09 Feb 2023 11:28:54 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Thu, 09 Feb 2023 11:28:55 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 11:31:41 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 09 Feb 2023 11:31:41 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 11:31:43 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 09 Feb 2023 11:31:43 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 11:31:44 GMT
USER varnish
# Thu, 09 Feb 2023 11:31:45 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 11:31:46 GMT
CMD []
```

-	Layers:
	-	`sha256:20744f4988404b1dee2cd438157b288d16a89da472583c0f04332ed389b258f8`  
		Last Modified: Thu, 09 Feb 2023 05:18:42 GMT  
		Size: 32.4 MB (32396875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f716893955fc8687049630d836de419a9ee4e31f969ac4c63da2c5780fa54c73`  
		Last Modified: Thu, 09 Feb 2023 11:36:33 GMT  
		Size: 75.8 MB (75825680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d3ab9c1eaecbdfad280dc92f39431564c14053c2af1d58d5b720a303be22c1`  
		Last Modified: Thu, 09 Feb 2023 11:36:23 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2` - linux; ppc64le

```console
$ docker pull varnish@sha256:456e1ab0c95e2025140b7ad74c5f8f784cf929a523d49cf8572e57edd918828d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.1 MB (106108350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbf49277a8a95baf5ea51cfb4eb767ca3cb1a463eb7dd260477154c2407e4074`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 06:21:49 GMT
ADD file:b09577b8131a90731fdfb00b824a97dc65ccb51d484cb9004382035d64a5741c in / 
# Thu, 09 Feb 2023 06:21:52 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 11:49:24 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 09 Feb 2023 11:49:24 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 09 Feb 2023 11:49:25 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 09 Feb 2023 11:49:25 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 09 Feb 2023 11:49:26 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 09 Feb 2023 11:49:26 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 09 Feb 2023 11:49:26 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 09 Feb 2023 11:49:26 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 09 Feb 2023 11:49:27 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 09 Feb 2023 11:49:27 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Thu, 09 Feb 2023 11:49:27 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 11:56:31 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 09 Feb 2023 11:56:35 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 11:56:35 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 09 Feb 2023 11:56:36 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 11:56:38 GMT
USER varnish
# Thu, 09 Feb 2023 11:56:38 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 11:56:38 GMT
CMD []
```

-	Layers:
	-	`sha256:4ea90e1a094ae86c7950bbec99e7a79b08fae641ad5f3bc3af9081c925894c41`  
		Last Modified: Thu, 09 Feb 2023 06:28:27 GMT  
		Size: 35.3 MB (35289252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e5d4b8afc29eb5a60b400a5a3ed200436b51055825af9d162bd04699491d76`  
		Last Modified: Thu, 09 Feb 2023 12:12:18 GMT  
		Size: 70.8 MB (70818605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab21c5070a377ef6e57bbe6990d1043689f75fbc0c8b7e1f7050f1ec7268642`  
		Last Modified: Thu, 09 Feb 2023 12:12:00 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2` - linux; s390x

```console
$ docker pull varnish@sha256:91374e1e9cf49dbdc947ad7908b9c4677f92abc06083dce76d8eab0e80814022
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.1 MB (87139320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c46fabb8d3b70dba47fcba3a588f2266fb2f5f72c7bf3eaa7306e997891f41ad`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 02:41:45 GMT
ADD file:dc3c16b50baeac5b9644e607c8df9606e9583f8598e3ba34bcdd69c669a5904c in / 
# Thu, 09 Feb 2023 02:41:46 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 04:31:11 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 09 Feb 2023 04:31:11 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 09 Feb 2023 04:31:11 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 09 Feb 2023 04:31:11 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 09 Feb 2023 04:31:11 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 09 Feb 2023 04:31:11 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 09 Feb 2023 04:31:12 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 09 Feb 2023 04:31:12 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 09 Feb 2023 04:31:12 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 09 Feb 2023 04:31:12 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Thu, 09 Feb 2023 04:31:12 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 04:35:02 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 09 Feb 2023 04:35:10 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 04:35:10 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 09 Feb 2023 04:35:11 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 04:35:12 GMT
USER varnish
# Thu, 09 Feb 2023 04:35:12 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 04:35:13 GMT
CMD []
```

-	Layers:
	-	`sha256:c2f78940fdfbfc5ce5d1d3cff3c27a319451aeb3ec12ff2473073516907fbce9`  
		Last Modified: Thu, 09 Feb 2023 02:46:06 GMT  
		Size: 29.6 MB (29647513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6956ec29c8de529c99c757cf901e5f2c77d691fc70707c44e776970c0071db9e`  
		Last Modified: Thu, 09 Feb 2023 04:42:56 GMT  
		Size: 57.5 MB (57491314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a38481f200bfa9b450cc4cebc812b08de7de18c35f4b7de12a835c601f2436`  
		Last Modified: Thu, 09 Feb 2023 04:42:49 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.2-alpine`

```console
$ docker pull varnish@sha256:0ae1260686d231b721e1dffba7ec421c95ab49f698e9b48fed675744fe144a4a
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
$ docker pull varnish@sha256:c6a7b674fa2e9a53c5ae0eadc57e835a1ed24ad81a717c76ba3c128a8d72db71
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.4 MB (59397542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:290f2c7d09415f1025c46ef26451df3246a538941b7f8b84ebe9a4918754c6f1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:23:08 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Tue, 08 Nov 2022 18:57:07 GMT
ARG VARNISH_VERSION=7.2.1
# Tue, 08 Nov 2022 18:57:07 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Tue, 08 Nov 2022 18:57:07 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Tue, 08 Nov 2022 18:57:07 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 09 Dec 2022 18:24:03 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Fri, 09 Dec 2022 18:24:04 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Fri, 09 Dec 2022 18:24:04 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Fri, 09 Dec 2022 18:24:04 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 09 Dec 2022 18:24:04 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Fri, 09 Dec 2022 18:24:04 GMT
ENV VARNISH_SIZE=100M
# Fri, 09 Dec 2022 18:25:19 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 09 Dec 2022 18:25:19 GMT
WORKDIR /etc/varnish
# Fri, 09 Dec 2022 18:25:19 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 09 Dec 2022 18:25:19 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 09 Dec 2022 18:25:20 GMT
USER varnish
# Fri, 09 Dec 2022 18:25:20 GMT
EXPOSE 80 8443
# Fri, 09 Dec 2022 18:25:20 GMT
CMD []
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cede921e2d42724a2365b66b858821b35b7e20527a43e585feaded18776e29e`  
		Last Modified: Fri, 09 Dec 2022 18:26:22 GMT  
		Size: 56.6 MB (56573532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26aa4aafc5f3e04e142b38aed4c4ab5be40fb074cbad3020e08b29142598b57c`  
		Last Modified: Fri, 09 Dec 2022 18:26:14 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:e66d31b1d8b6e119d0f044c545f8edaabb45276cfea6577928a19d9bc578b773
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45149649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfc50568e3c1ccdf4c5c1c666d75d7667f04ab218bf8a5b59f37d52fa054bcde`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 10 Nov 2022 19:57:41 GMT
ADD file:0bd18306f21937a9572e68c768f05f4a9d8341b40c2379a7bfcb857c77734a14 in / 
# Thu, 10 Nov 2022 19:57:41 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 13:51:48 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Fri, 11 Nov 2022 13:51:49 GMT
ARG VARNISH_VERSION=7.2.1
# Fri, 11 Nov 2022 13:51:49 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Fri, 11 Nov 2022 13:51:49 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Fri, 11 Nov 2022 13:51:49 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 09 Dec 2022 18:14:58 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Fri, 09 Dec 2022 18:14:58 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Fri, 09 Dec 2022 18:14:58 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Fri, 09 Dec 2022 18:14:58 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 09 Dec 2022 18:14:58 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Fri, 09 Dec 2022 18:14:59 GMT
ENV VARNISH_SIZE=100M
# Fri, 09 Dec 2022 18:16:25 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 09 Dec 2022 18:16:25 GMT
WORKDIR /etc/varnish
# Fri, 09 Dec 2022 18:16:25 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 09 Dec 2022 18:16:25 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 09 Dec 2022 18:16:25 GMT
USER varnish
# Fri, 09 Dec 2022 18:16:25 GMT
EXPOSE 80 8443
# Fri, 09 Dec 2022 18:16:25 GMT
CMD []
```

-	Layers:
	-	`sha256:59775c20a906b1a49edcdc41a700a795998979d6ecf8f8d9cd7cbdf45e686d81`  
		Last Modified: Tue, 09 Aug 2022 16:59:12 GMT  
		Size: 2.4 MB (2435092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f59a293f1456cae4428183939900b44f083b6bd1724fb73b56eab4c22f73c84`  
		Last Modified: Fri, 09 Dec 2022 18:18:21 GMT  
		Size: 42.7 MB (42714062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9188a361ad4c027cd69a7ccfc3bb2b141caf9024edc09c7742b0070d5fff8e`  
		Last Modified: Fri, 09 Dec 2022 18:18:14 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:9fde738bd7a1792db975b2f43f532b894aed6e28fd982814c09f52f93b9c0bb8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52133505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b3875632d7c932d6d21178f71d8d5e814ed41f152159ceea19652219c63e115`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Tue, 15 Nov 2022 11:44:18 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Tue, 15 Nov 2022 11:44:18 GMT
ARG VARNISH_VERSION=7.2.1
# Tue, 15 Nov 2022 11:44:18 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Tue, 15 Nov 2022 11:44:18 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Tue, 15 Nov 2022 11:44:18 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 09 Dec 2022 17:50:18 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Fri, 09 Dec 2022 17:50:18 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Fri, 09 Dec 2022 17:50:19 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Fri, 09 Dec 2022 17:50:19 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 09 Dec 2022 17:50:19 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Fri, 09 Dec 2022 17:50:19 GMT
ENV VARNISH_SIZE=100M
# Fri, 09 Dec 2022 17:51:24 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 09 Dec 2022 17:51:25 GMT
WORKDIR /etc/varnish
# Fri, 09 Dec 2022 17:51:25 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 09 Dec 2022 17:51:25 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 09 Dec 2022 17:51:25 GMT
USER varnish
# Fri, 09 Dec 2022 17:51:25 GMT
EXPOSE 80 8443
# Fri, 09 Dec 2022 17:51:25 GMT
CMD []
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d55913ffdb6c1584033b1dc44e04a7da2c51610e945c943b3bda4f7103ddcb`  
		Last Modified: Fri, 09 Dec 2022 17:52:18 GMT  
		Size: 49.4 MB (49414568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12636ca6c95502ab17e340d2f6b112367aba4ac1e20f7ab8163b4b68fcb66602`  
		Last Modified: Fri, 09 Dec 2022 17:52:13 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2-alpine` - linux; 386

```console
$ docker pull varnish@sha256:27b8ea22e0b98f3d370da0d7b28926290fd3cc2096166cd9814a9191f978457c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.6 MB (59569325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bea02470a3246fa42ff058293f436786cc663210bee1fbcbec1b9576d4074e24`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 02:07:46 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Tue, 08 Nov 2022 18:42:10 GMT
ARG VARNISH_VERSION=7.2.1
# Tue, 08 Nov 2022 18:42:11 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Tue, 08 Nov 2022 18:42:12 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Tue, 08 Nov 2022 18:42:13 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 09 Dec 2022 17:42:21 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Fri, 09 Dec 2022 17:42:22 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Fri, 09 Dec 2022 17:42:23 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Fri, 09 Dec 2022 17:42:24 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 09 Dec 2022 17:42:25 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Fri, 09 Dec 2022 17:42:26 GMT
ENV VARNISH_SIZE=100M
# Fri, 09 Dec 2022 17:46:33 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 09 Dec 2022 17:46:33 GMT
WORKDIR /etc/varnish
# Fri, 09 Dec 2022 17:46:35 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 09 Dec 2022 17:46:35 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 09 Dec 2022 17:46:36 GMT
USER varnish
# Fri, 09 Dec 2022 17:46:37 GMT
EXPOSE 80 8443
# Fri, 09 Dec 2022 17:46:38 GMT
CMD []
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355d74fc07dbf50689ac17b0f5e0fbec1a8af7b1f9dcee17d46f5eff1976e107`  
		Last Modified: Fri, 09 Dec 2022 17:51:03 GMT  
		Size: 56.7 MB (56740309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca599fa8915fde7ecc73fd114e3d10d5de8df77430cab928b8d3de0fa748660`  
		Last Modified: Fri, 09 Dec 2022 17:50:56 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:d9b9fe178087cfb51751f8639988a578f97ea1fba591014f45c9e97105af44e1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49171305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d291f0165a1bba74dd02443b07f16dbd3610099d07f5b35b6db221e683c44db1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:17:20 GMT
ADD file:be31abb0aba89ed5ff9200736a1c46091abc3845d0e332efd5e5c874ef2c99d1 in / 
# Tue, 09 Aug 2022 17:17:21 GMT
CMD ["/bin/sh"]
# Tue, 15 Nov 2022 18:45:59 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Tue, 15 Nov 2022 18:45:59 GMT
ARG VARNISH_VERSION=7.2.1
# Tue, 15 Nov 2022 18:45:59 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Tue, 15 Nov 2022 18:46:00 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Tue, 15 Nov 2022 18:46:01 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 09 Dec 2022 18:23:43 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Fri, 09 Dec 2022 18:23:43 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Fri, 09 Dec 2022 18:23:44 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Fri, 09 Dec 2022 18:23:44 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 09 Dec 2022 18:23:44 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Fri, 09 Dec 2022 18:23:45 GMT
ENV VARNISH_SIZE=100M
# Fri, 09 Dec 2022 18:26:49 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 09 Dec 2022 18:26:50 GMT
WORKDIR /etc/varnish
# Fri, 09 Dec 2022 18:26:51 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 09 Dec 2022 18:26:51 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 09 Dec 2022 18:26:51 GMT
USER varnish
# Fri, 09 Dec 2022 18:26:52 GMT
EXPOSE 80 8443
# Fri, 09 Dec 2022 18:26:52 GMT
CMD []
```

-	Layers:
	-	`sha256:deb7065b3304c3a9834f31b8a53e8d6089060e9c6522668abd22f1f4d9f52ca7`  
		Last Modified: Tue, 09 Aug 2022 17:18:45 GMT  
		Size: 2.8 MB (2812989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03574054a01f0f8826848eadc2b4868a9b65c93aeea02a7c772806cb0685c5b`  
		Last Modified: Fri, 09 Dec 2022 18:28:45 GMT  
		Size: 46.4 MB (46357815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247857fc893c2b18ff450e4ccb0737d8ef6102933f4676e64a56141d824bd241`  
		Last Modified: Fri, 09 Dec 2022 18:28:32 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:76127ff5d6570cf73bc4581690b687ed086bbdb9133031e768c158ed63d0670f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47639610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69d9ab461e74d3101ebf2639b6b85153995bd23a2c1aa8a28b04010ad87841f0`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Tue, 15 Nov 2022 13:45:26 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Tue, 15 Nov 2022 13:45:27 GMT
ARG VARNISH_VERSION=7.2.1
# Tue, 15 Nov 2022 13:45:28 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Tue, 15 Nov 2022 13:45:28 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Tue, 15 Nov 2022 13:45:29 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 09 Dec 2022 17:47:41 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Fri, 09 Dec 2022 17:47:42 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Fri, 09 Dec 2022 17:47:42 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Fri, 09 Dec 2022 17:47:42 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 09 Dec 2022 17:47:43 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Fri, 09 Dec 2022 17:47:43 GMT
ENV VARNISH_SIZE=100M
# Fri, 09 Dec 2022 17:50:02 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 09 Dec 2022 17:50:07 GMT
WORKDIR /etc/varnish
# Fri, 09 Dec 2022 17:50:07 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 09 Dec 2022 17:50:08 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 09 Dec 2022 17:50:08 GMT
USER varnish
# Fri, 09 Dec 2022 17:50:09 GMT
EXPOSE 80 8443
# Fri, 09 Dec 2022 17:50:09 GMT
CMD []
```

-	Layers:
	-	`sha256:cdf710f5b7ee39c5124c50c753228dc9b8b1c1c0a1a38f1413487548565445c3`  
		Last Modified: Tue, 09 Aug 2022 17:42:56 GMT  
		Size: 2.6 MB (2606087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6af5a3cf679c345cb17179d345e3eb2554e532099f5c4f9e9fab9aa7e9427a`  
		Last Modified: Fri, 09 Dec 2022 17:59:52 GMT  
		Size: 45.0 MB (45033026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936f6bf8d89d854c95fd8761e729b493edaa1757fa875c933ce1da1a392f805c`  
		Last Modified: Fri, 09 Dec 2022 17:59:47 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.2.1`

```console
$ docker pull varnish@sha256:3feac23caf88ff28673bcb4aa81ae8dd316e4476c260af1a2c6e201cfcf4786e
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
$ docker pull varnish@sha256:d64ca9b7756cb3a0eda02971eba4e2006311fc85c52ccd6e992475366ac5790a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106843191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16576fb65a911c2195ae8bb7ea33bf084f41b7348f2d20473af354a42e4f6761`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:38:29 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 09 Feb 2023 06:38:29 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 09 Feb 2023 06:38:29 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 09 Feb 2023 06:38:29 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 09 Feb 2023 06:38:29 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 09 Feb 2023 06:38:29 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 09 Feb 2023 06:38:29 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 09 Feb 2023 06:38:29 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 09 Feb 2023 06:38:30 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 09 Feb 2023 06:38:30 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Thu, 09 Feb 2023 06:38:30 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 06:41:50 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 09 Feb 2023 06:41:51 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 06:41:51 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 09 Feb 2023 06:41:51 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 06:41:51 GMT
USER varnish
# Thu, 09 Feb 2023 06:41:51 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 06:41:51 GMT
CMD []
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5849700d1633b0858d2a64844bb0fdd45c87607fcf429d07dbcacf1835ff2e0f`  
		Last Modified: Thu, 09 Feb 2023 06:48:10 GMT  
		Size: 75.4 MB (75430887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819e8388a2fe25ed89691731d6a3f4a2feb9a30cf8db8de9a72ef699909ea329`  
		Last Modified: Thu, 09 Feb 2023 06:48:00 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2.1` - linux; arm variant v7

```console
$ docker pull varnish@sha256:667101f4287db71b7a21b99ed03b1190bf6ffec44a07c12406fac8f710cf287a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.2 MB (83169412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:293472e275cc824b762c201d32db85c29c22ad7c0462959504240f5c74f3f3b9`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Sat, 04 Feb 2023 09:59:36 GMT
ADD file:c3cb8f4527fa96e99a4741ecb398113f25f53389c173b74f6c2a5e39a6575c60 in / 
# Sat, 04 Feb 2023 09:59:36 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 21:19:28 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Sat, 04 Feb 2023 21:19:28 GMT
ARG VARNISH_VERSION=7.2.1
# Sat, 04 Feb 2023 21:19:28 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Sat, 04 Feb 2023 21:19:28 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Sat, 04 Feb 2023 21:19:29 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Sat, 04 Feb 2023 21:19:29 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Sat, 04 Feb 2023 21:19:29 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Sat, 04 Feb 2023 21:19:29 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Sat, 04 Feb 2023 21:19:29 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Sat, 04 Feb 2023 21:19:29 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Sat, 04 Feb 2023 21:19:29 GMT
ENV VARNISH_SIZE=100M
# Sat, 04 Feb 2023 21:22:30 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Sat, 04 Feb 2023 21:22:31 GMT
WORKDIR /etc/varnish
# Sat, 04 Feb 2023 21:22:31 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Sat, 04 Feb 2023 21:22:31 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sat, 04 Feb 2023 21:22:31 GMT
USER varnish
# Sat, 04 Feb 2023 21:22:31 GMT
EXPOSE 80 8443
# Sat, 04 Feb 2023 21:22:31 GMT
CMD []
```

-	Layers:
	-	`sha256:bd25bcdfbaa165120ee21b6567df395fe7d7b38da3cca0bcecee55a190e04aab`  
		Last Modified: Sat, 04 Feb 2023 10:06:24 GMT  
		Size: 26.6 MB (26559474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32aa6224c75d142f0a76142fa8ebabe4a311fc4ce23351e0248c29b47989d8f6`  
		Last Modified: Sat, 04 Feb 2023 21:29:24 GMT  
		Size: 56.6 MB (56609446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67957e16f03a30cd49c3c133970df3e4af0ca6c1d3517ade7f271caf5c636dbf`  
		Last Modified: Sat, 04 Feb 2023 21:29:15 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2.1` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:070c65da2b8faf580eec672e0db795ded6285b428e1d39254f88244f6d2ba8fe
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.9 MB (100867420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa825a96e8e9266a3bf0501d85a6d0b2d4176c29895bd7b07085738e302fe068`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 08:43:56 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 09 Feb 2023 08:43:56 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 09 Feb 2023 08:43:56 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 09 Feb 2023 08:43:56 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 09 Feb 2023 08:43:56 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 09 Feb 2023 08:43:56 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 09 Feb 2023 08:43:56 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 09 Feb 2023 08:43:56 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 09 Feb 2023 08:43:57 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 09 Feb 2023 08:43:57 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Thu, 09 Feb 2023 08:43:57 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 08:46:49 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 09 Feb 2023 08:46:50 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 08:46:50 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 09 Feb 2023 08:46:50 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 08:46:50 GMT
USER varnish
# Thu, 09 Feb 2023 08:46:50 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 08:46:50 GMT
CMD []
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd593e410516ba146ca282d48deef73a7e2eaef76c1020ca6e524bc5aa4a6078`  
		Last Modified: Thu, 09 Feb 2023 08:51:51 GMT  
		Size: 70.8 MB (70804416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4459f721e7b5112ddc4a759e70ea9f389dbe7ea84abed0cf252d75110b8a00b1`  
		Last Modified: Thu, 09 Feb 2023 08:51:45 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2.1` - linux; 386

```console
$ docker pull varnish@sha256:32e374f738c01546453d2edad6a6797b7eef8d9b4145e3a8f7cbb00886bf9aca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.2 MB (108223049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0847bbcdf260fc907bc7fc41a1e8607b6bab32fff55ecc9738733798c6d219e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 05:12:53 GMT
ADD file:7740abd3129d33122ce51153c0b6c3323b9cbe9ea0e81672e16b2d7b210d24e3 in / 
# Thu, 09 Feb 2023 05:12:53 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 11:28:46 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 09 Feb 2023 11:28:46 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 09 Feb 2023 11:28:47 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 09 Feb 2023 11:28:48 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 09 Feb 2023 11:28:49 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 09 Feb 2023 11:28:50 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 09 Feb 2023 11:28:51 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 09 Feb 2023 11:28:52 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 09 Feb 2023 11:28:53 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 09 Feb 2023 11:28:54 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Thu, 09 Feb 2023 11:28:55 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 11:31:41 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 09 Feb 2023 11:31:41 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 11:31:43 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 09 Feb 2023 11:31:43 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 11:31:44 GMT
USER varnish
# Thu, 09 Feb 2023 11:31:45 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 11:31:46 GMT
CMD []
```

-	Layers:
	-	`sha256:20744f4988404b1dee2cd438157b288d16a89da472583c0f04332ed389b258f8`  
		Last Modified: Thu, 09 Feb 2023 05:18:42 GMT  
		Size: 32.4 MB (32396875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f716893955fc8687049630d836de419a9ee4e31f969ac4c63da2c5780fa54c73`  
		Last Modified: Thu, 09 Feb 2023 11:36:33 GMT  
		Size: 75.8 MB (75825680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d3ab9c1eaecbdfad280dc92f39431564c14053c2af1d58d5b720a303be22c1`  
		Last Modified: Thu, 09 Feb 2023 11:36:23 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2.1` - linux; ppc64le

```console
$ docker pull varnish@sha256:456e1ab0c95e2025140b7ad74c5f8f784cf929a523d49cf8572e57edd918828d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.1 MB (106108350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbf49277a8a95baf5ea51cfb4eb767ca3cb1a463eb7dd260477154c2407e4074`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 06:21:49 GMT
ADD file:b09577b8131a90731fdfb00b824a97dc65ccb51d484cb9004382035d64a5741c in / 
# Thu, 09 Feb 2023 06:21:52 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 11:49:24 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 09 Feb 2023 11:49:24 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 09 Feb 2023 11:49:25 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 09 Feb 2023 11:49:25 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 09 Feb 2023 11:49:26 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 09 Feb 2023 11:49:26 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 09 Feb 2023 11:49:26 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 09 Feb 2023 11:49:26 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 09 Feb 2023 11:49:27 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 09 Feb 2023 11:49:27 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Thu, 09 Feb 2023 11:49:27 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 11:56:31 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 09 Feb 2023 11:56:35 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 11:56:35 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 09 Feb 2023 11:56:36 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 11:56:38 GMT
USER varnish
# Thu, 09 Feb 2023 11:56:38 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 11:56:38 GMT
CMD []
```

-	Layers:
	-	`sha256:4ea90e1a094ae86c7950bbec99e7a79b08fae641ad5f3bc3af9081c925894c41`  
		Last Modified: Thu, 09 Feb 2023 06:28:27 GMT  
		Size: 35.3 MB (35289252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e5d4b8afc29eb5a60b400a5a3ed200436b51055825af9d162bd04699491d76`  
		Last Modified: Thu, 09 Feb 2023 12:12:18 GMT  
		Size: 70.8 MB (70818605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab21c5070a377ef6e57bbe6990d1043689f75fbc0c8b7e1f7050f1ec7268642`  
		Last Modified: Thu, 09 Feb 2023 12:12:00 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2.1` - linux; s390x

```console
$ docker pull varnish@sha256:91374e1e9cf49dbdc947ad7908b9c4677f92abc06083dce76d8eab0e80814022
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.1 MB (87139320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c46fabb8d3b70dba47fcba3a588f2266fb2f5f72c7bf3eaa7306e997891f41ad`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 02:41:45 GMT
ADD file:dc3c16b50baeac5b9644e607c8df9606e9583f8598e3ba34bcdd69c669a5904c in / 
# Thu, 09 Feb 2023 02:41:46 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 04:31:11 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 09 Feb 2023 04:31:11 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 09 Feb 2023 04:31:11 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 09 Feb 2023 04:31:11 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 09 Feb 2023 04:31:11 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 09 Feb 2023 04:31:11 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 09 Feb 2023 04:31:12 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 09 Feb 2023 04:31:12 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 09 Feb 2023 04:31:12 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 09 Feb 2023 04:31:12 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Thu, 09 Feb 2023 04:31:12 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 04:35:02 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 09 Feb 2023 04:35:10 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 04:35:10 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 09 Feb 2023 04:35:11 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 04:35:12 GMT
USER varnish
# Thu, 09 Feb 2023 04:35:12 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 04:35:13 GMT
CMD []
```

-	Layers:
	-	`sha256:c2f78940fdfbfc5ce5d1d3cff3c27a319451aeb3ec12ff2473073516907fbce9`  
		Last Modified: Thu, 09 Feb 2023 02:46:06 GMT  
		Size: 29.6 MB (29647513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6956ec29c8de529c99c757cf901e5f2c77d691fc70707c44e776970c0071db9e`  
		Last Modified: Thu, 09 Feb 2023 04:42:56 GMT  
		Size: 57.5 MB (57491314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a38481f200bfa9b450cc4cebc812b08de7de18c35f4b7de12a835c601f2436`  
		Last Modified: Thu, 09 Feb 2023 04:42:49 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.2.1-alpine`

```console
$ docker pull varnish@sha256:0ae1260686d231b721e1dffba7ec421c95ab49f698e9b48fed675744fe144a4a
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
$ docker pull varnish@sha256:c6a7b674fa2e9a53c5ae0eadc57e835a1ed24ad81a717c76ba3c128a8d72db71
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.4 MB (59397542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:290f2c7d09415f1025c46ef26451df3246a538941b7f8b84ebe9a4918754c6f1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:23:08 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Tue, 08 Nov 2022 18:57:07 GMT
ARG VARNISH_VERSION=7.2.1
# Tue, 08 Nov 2022 18:57:07 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Tue, 08 Nov 2022 18:57:07 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Tue, 08 Nov 2022 18:57:07 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 09 Dec 2022 18:24:03 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Fri, 09 Dec 2022 18:24:04 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Fri, 09 Dec 2022 18:24:04 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Fri, 09 Dec 2022 18:24:04 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 09 Dec 2022 18:24:04 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Fri, 09 Dec 2022 18:24:04 GMT
ENV VARNISH_SIZE=100M
# Fri, 09 Dec 2022 18:25:19 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 09 Dec 2022 18:25:19 GMT
WORKDIR /etc/varnish
# Fri, 09 Dec 2022 18:25:19 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 09 Dec 2022 18:25:19 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 09 Dec 2022 18:25:20 GMT
USER varnish
# Fri, 09 Dec 2022 18:25:20 GMT
EXPOSE 80 8443
# Fri, 09 Dec 2022 18:25:20 GMT
CMD []
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cede921e2d42724a2365b66b858821b35b7e20527a43e585feaded18776e29e`  
		Last Modified: Fri, 09 Dec 2022 18:26:22 GMT  
		Size: 56.6 MB (56573532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26aa4aafc5f3e04e142b38aed4c4ab5be40fb074cbad3020e08b29142598b57c`  
		Last Modified: Fri, 09 Dec 2022 18:26:14 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2.1-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:e66d31b1d8b6e119d0f044c545f8edaabb45276cfea6577928a19d9bc578b773
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45149649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfc50568e3c1ccdf4c5c1c666d75d7667f04ab218bf8a5b59f37d52fa054bcde`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 10 Nov 2022 19:57:41 GMT
ADD file:0bd18306f21937a9572e68c768f05f4a9d8341b40c2379a7bfcb857c77734a14 in / 
# Thu, 10 Nov 2022 19:57:41 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 13:51:48 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Fri, 11 Nov 2022 13:51:49 GMT
ARG VARNISH_VERSION=7.2.1
# Fri, 11 Nov 2022 13:51:49 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Fri, 11 Nov 2022 13:51:49 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Fri, 11 Nov 2022 13:51:49 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 09 Dec 2022 18:14:58 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Fri, 09 Dec 2022 18:14:58 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Fri, 09 Dec 2022 18:14:58 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Fri, 09 Dec 2022 18:14:58 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 09 Dec 2022 18:14:58 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Fri, 09 Dec 2022 18:14:59 GMT
ENV VARNISH_SIZE=100M
# Fri, 09 Dec 2022 18:16:25 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 09 Dec 2022 18:16:25 GMT
WORKDIR /etc/varnish
# Fri, 09 Dec 2022 18:16:25 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 09 Dec 2022 18:16:25 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 09 Dec 2022 18:16:25 GMT
USER varnish
# Fri, 09 Dec 2022 18:16:25 GMT
EXPOSE 80 8443
# Fri, 09 Dec 2022 18:16:25 GMT
CMD []
```

-	Layers:
	-	`sha256:59775c20a906b1a49edcdc41a700a795998979d6ecf8f8d9cd7cbdf45e686d81`  
		Last Modified: Tue, 09 Aug 2022 16:59:12 GMT  
		Size: 2.4 MB (2435092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f59a293f1456cae4428183939900b44f083b6bd1724fb73b56eab4c22f73c84`  
		Last Modified: Fri, 09 Dec 2022 18:18:21 GMT  
		Size: 42.7 MB (42714062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9188a361ad4c027cd69a7ccfc3bb2b141caf9024edc09c7742b0070d5fff8e`  
		Last Modified: Fri, 09 Dec 2022 18:18:14 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2.1-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:9fde738bd7a1792db975b2f43f532b894aed6e28fd982814c09f52f93b9c0bb8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52133505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b3875632d7c932d6d21178f71d8d5e814ed41f152159ceea19652219c63e115`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Tue, 15 Nov 2022 11:44:18 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Tue, 15 Nov 2022 11:44:18 GMT
ARG VARNISH_VERSION=7.2.1
# Tue, 15 Nov 2022 11:44:18 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Tue, 15 Nov 2022 11:44:18 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Tue, 15 Nov 2022 11:44:18 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 09 Dec 2022 17:50:18 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Fri, 09 Dec 2022 17:50:18 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Fri, 09 Dec 2022 17:50:19 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Fri, 09 Dec 2022 17:50:19 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 09 Dec 2022 17:50:19 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Fri, 09 Dec 2022 17:50:19 GMT
ENV VARNISH_SIZE=100M
# Fri, 09 Dec 2022 17:51:24 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 09 Dec 2022 17:51:25 GMT
WORKDIR /etc/varnish
# Fri, 09 Dec 2022 17:51:25 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 09 Dec 2022 17:51:25 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 09 Dec 2022 17:51:25 GMT
USER varnish
# Fri, 09 Dec 2022 17:51:25 GMT
EXPOSE 80 8443
# Fri, 09 Dec 2022 17:51:25 GMT
CMD []
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d55913ffdb6c1584033b1dc44e04a7da2c51610e945c943b3bda4f7103ddcb`  
		Last Modified: Fri, 09 Dec 2022 17:52:18 GMT  
		Size: 49.4 MB (49414568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12636ca6c95502ab17e340d2f6b112367aba4ac1e20f7ab8163b4b68fcb66602`  
		Last Modified: Fri, 09 Dec 2022 17:52:13 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2.1-alpine` - linux; 386

```console
$ docker pull varnish@sha256:27b8ea22e0b98f3d370da0d7b28926290fd3cc2096166cd9814a9191f978457c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.6 MB (59569325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bea02470a3246fa42ff058293f436786cc663210bee1fbcbec1b9576d4074e24`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 02:07:46 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Tue, 08 Nov 2022 18:42:10 GMT
ARG VARNISH_VERSION=7.2.1
# Tue, 08 Nov 2022 18:42:11 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Tue, 08 Nov 2022 18:42:12 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Tue, 08 Nov 2022 18:42:13 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 09 Dec 2022 17:42:21 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Fri, 09 Dec 2022 17:42:22 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Fri, 09 Dec 2022 17:42:23 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Fri, 09 Dec 2022 17:42:24 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 09 Dec 2022 17:42:25 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Fri, 09 Dec 2022 17:42:26 GMT
ENV VARNISH_SIZE=100M
# Fri, 09 Dec 2022 17:46:33 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 09 Dec 2022 17:46:33 GMT
WORKDIR /etc/varnish
# Fri, 09 Dec 2022 17:46:35 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 09 Dec 2022 17:46:35 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 09 Dec 2022 17:46:36 GMT
USER varnish
# Fri, 09 Dec 2022 17:46:37 GMT
EXPOSE 80 8443
# Fri, 09 Dec 2022 17:46:38 GMT
CMD []
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355d74fc07dbf50689ac17b0f5e0fbec1a8af7b1f9dcee17d46f5eff1976e107`  
		Last Modified: Fri, 09 Dec 2022 17:51:03 GMT  
		Size: 56.7 MB (56740309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca599fa8915fde7ecc73fd114e3d10d5de8df77430cab928b8d3de0fa748660`  
		Last Modified: Fri, 09 Dec 2022 17:50:56 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2.1-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:d9b9fe178087cfb51751f8639988a578f97ea1fba591014f45c9e97105af44e1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49171305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d291f0165a1bba74dd02443b07f16dbd3610099d07f5b35b6db221e683c44db1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:17:20 GMT
ADD file:be31abb0aba89ed5ff9200736a1c46091abc3845d0e332efd5e5c874ef2c99d1 in / 
# Tue, 09 Aug 2022 17:17:21 GMT
CMD ["/bin/sh"]
# Tue, 15 Nov 2022 18:45:59 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Tue, 15 Nov 2022 18:45:59 GMT
ARG VARNISH_VERSION=7.2.1
# Tue, 15 Nov 2022 18:45:59 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Tue, 15 Nov 2022 18:46:00 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Tue, 15 Nov 2022 18:46:01 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 09 Dec 2022 18:23:43 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Fri, 09 Dec 2022 18:23:43 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Fri, 09 Dec 2022 18:23:44 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Fri, 09 Dec 2022 18:23:44 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 09 Dec 2022 18:23:44 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Fri, 09 Dec 2022 18:23:45 GMT
ENV VARNISH_SIZE=100M
# Fri, 09 Dec 2022 18:26:49 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 09 Dec 2022 18:26:50 GMT
WORKDIR /etc/varnish
# Fri, 09 Dec 2022 18:26:51 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 09 Dec 2022 18:26:51 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 09 Dec 2022 18:26:51 GMT
USER varnish
# Fri, 09 Dec 2022 18:26:52 GMT
EXPOSE 80 8443
# Fri, 09 Dec 2022 18:26:52 GMT
CMD []
```

-	Layers:
	-	`sha256:deb7065b3304c3a9834f31b8a53e8d6089060e9c6522668abd22f1f4d9f52ca7`  
		Last Modified: Tue, 09 Aug 2022 17:18:45 GMT  
		Size: 2.8 MB (2812989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03574054a01f0f8826848eadc2b4868a9b65c93aeea02a7c772806cb0685c5b`  
		Last Modified: Fri, 09 Dec 2022 18:28:45 GMT  
		Size: 46.4 MB (46357815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247857fc893c2b18ff450e4ccb0737d8ef6102933f4676e64a56141d824bd241`  
		Last Modified: Fri, 09 Dec 2022 18:28:32 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2.1-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:76127ff5d6570cf73bc4581690b687ed086bbdb9133031e768c158ed63d0670f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47639610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69d9ab461e74d3101ebf2639b6b85153995bd23a2c1aa8a28b04010ad87841f0`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Tue, 15 Nov 2022 13:45:26 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Tue, 15 Nov 2022 13:45:27 GMT
ARG VARNISH_VERSION=7.2.1
# Tue, 15 Nov 2022 13:45:28 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Tue, 15 Nov 2022 13:45:28 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Tue, 15 Nov 2022 13:45:29 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 09 Dec 2022 17:47:41 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Fri, 09 Dec 2022 17:47:42 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Fri, 09 Dec 2022 17:47:42 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Fri, 09 Dec 2022 17:47:42 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 09 Dec 2022 17:47:43 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Fri, 09 Dec 2022 17:47:43 GMT
ENV VARNISH_SIZE=100M
# Fri, 09 Dec 2022 17:50:02 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 09 Dec 2022 17:50:07 GMT
WORKDIR /etc/varnish
# Fri, 09 Dec 2022 17:50:07 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 09 Dec 2022 17:50:08 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 09 Dec 2022 17:50:08 GMT
USER varnish
# Fri, 09 Dec 2022 17:50:09 GMT
EXPOSE 80 8443
# Fri, 09 Dec 2022 17:50:09 GMT
CMD []
```

-	Layers:
	-	`sha256:cdf710f5b7ee39c5124c50c753228dc9b8b1c1c0a1a38f1413487548565445c3`  
		Last Modified: Tue, 09 Aug 2022 17:42:56 GMT  
		Size: 2.6 MB (2606087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6af5a3cf679c345cb17179d345e3eb2554e532099f5c4f9e9fab9aa7e9427a`  
		Last Modified: Fri, 09 Dec 2022 17:59:52 GMT  
		Size: 45.0 MB (45033026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936f6bf8d89d854c95fd8761e729b493edaa1757fa875c933ce1da1a392f805c`  
		Last Modified: Fri, 09 Dec 2022 17:59:47 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:alpine`

```console
$ docker pull varnish@sha256:0ae1260686d231b721e1dffba7ec421c95ab49f698e9b48fed675744fe144a4a
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
$ docker pull varnish@sha256:c6a7b674fa2e9a53c5ae0eadc57e835a1ed24ad81a717c76ba3c128a8d72db71
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.4 MB (59397542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:290f2c7d09415f1025c46ef26451df3246a538941b7f8b84ebe9a4918754c6f1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:23:08 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Tue, 08 Nov 2022 18:57:07 GMT
ARG VARNISH_VERSION=7.2.1
# Tue, 08 Nov 2022 18:57:07 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Tue, 08 Nov 2022 18:57:07 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Tue, 08 Nov 2022 18:57:07 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 09 Dec 2022 18:24:03 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Fri, 09 Dec 2022 18:24:04 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Fri, 09 Dec 2022 18:24:04 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Fri, 09 Dec 2022 18:24:04 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 09 Dec 2022 18:24:04 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Fri, 09 Dec 2022 18:24:04 GMT
ENV VARNISH_SIZE=100M
# Fri, 09 Dec 2022 18:25:19 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 09 Dec 2022 18:25:19 GMT
WORKDIR /etc/varnish
# Fri, 09 Dec 2022 18:25:19 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 09 Dec 2022 18:25:19 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 09 Dec 2022 18:25:20 GMT
USER varnish
# Fri, 09 Dec 2022 18:25:20 GMT
EXPOSE 80 8443
# Fri, 09 Dec 2022 18:25:20 GMT
CMD []
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cede921e2d42724a2365b66b858821b35b7e20527a43e585feaded18776e29e`  
		Last Modified: Fri, 09 Dec 2022 18:26:22 GMT  
		Size: 56.6 MB (56573532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26aa4aafc5f3e04e142b38aed4c4ab5be40fb074cbad3020e08b29142598b57c`  
		Last Modified: Fri, 09 Dec 2022 18:26:14 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:e66d31b1d8b6e119d0f044c545f8edaabb45276cfea6577928a19d9bc578b773
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45149649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfc50568e3c1ccdf4c5c1c666d75d7667f04ab218bf8a5b59f37d52fa054bcde`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 10 Nov 2022 19:57:41 GMT
ADD file:0bd18306f21937a9572e68c768f05f4a9d8341b40c2379a7bfcb857c77734a14 in / 
# Thu, 10 Nov 2022 19:57:41 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 13:51:48 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Fri, 11 Nov 2022 13:51:49 GMT
ARG VARNISH_VERSION=7.2.1
# Fri, 11 Nov 2022 13:51:49 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Fri, 11 Nov 2022 13:51:49 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Fri, 11 Nov 2022 13:51:49 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 09 Dec 2022 18:14:58 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Fri, 09 Dec 2022 18:14:58 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Fri, 09 Dec 2022 18:14:58 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Fri, 09 Dec 2022 18:14:58 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 09 Dec 2022 18:14:58 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Fri, 09 Dec 2022 18:14:59 GMT
ENV VARNISH_SIZE=100M
# Fri, 09 Dec 2022 18:16:25 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 09 Dec 2022 18:16:25 GMT
WORKDIR /etc/varnish
# Fri, 09 Dec 2022 18:16:25 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 09 Dec 2022 18:16:25 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 09 Dec 2022 18:16:25 GMT
USER varnish
# Fri, 09 Dec 2022 18:16:25 GMT
EXPOSE 80 8443
# Fri, 09 Dec 2022 18:16:25 GMT
CMD []
```

-	Layers:
	-	`sha256:59775c20a906b1a49edcdc41a700a795998979d6ecf8f8d9cd7cbdf45e686d81`  
		Last Modified: Tue, 09 Aug 2022 16:59:12 GMT  
		Size: 2.4 MB (2435092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f59a293f1456cae4428183939900b44f083b6bd1724fb73b56eab4c22f73c84`  
		Last Modified: Fri, 09 Dec 2022 18:18:21 GMT  
		Size: 42.7 MB (42714062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9188a361ad4c027cd69a7ccfc3bb2b141caf9024edc09c7742b0070d5fff8e`  
		Last Modified: Fri, 09 Dec 2022 18:18:14 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:9fde738bd7a1792db975b2f43f532b894aed6e28fd982814c09f52f93b9c0bb8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52133505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b3875632d7c932d6d21178f71d8d5e814ed41f152159ceea19652219c63e115`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Tue, 15 Nov 2022 11:44:18 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Tue, 15 Nov 2022 11:44:18 GMT
ARG VARNISH_VERSION=7.2.1
# Tue, 15 Nov 2022 11:44:18 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Tue, 15 Nov 2022 11:44:18 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Tue, 15 Nov 2022 11:44:18 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 09 Dec 2022 17:50:18 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Fri, 09 Dec 2022 17:50:18 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Fri, 09 Dec 2022 17:50:19 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Fri, 09 Dec 2022 17:50:19 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 09 Dec 2022 17:50:19 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Fri, 09 Dec 2022 17:50:19 GMT
ENV VARNISH_SIZE=100M
# Fri, 09 Dec 2022 17:51:24 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 09 Dec 2022 17:51:25 GMT
WORKDIR /etc/varnish
# Fri, 09 Dec 2022 17:51:25 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 09 Dec 2022 17:51:25 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 09 Dec 2022 17:51:25 GMT
USER varnish
# Fri, 09 Dec 2022 17:51:25 GMT
EXPOSE 80 8443
# Fri, 09 Dec 2022 17:51:25 GMT
CMD []
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d55913ffdb6c1584033b1dc44e04a7da2c51610e945c943b3bda4f7103ddcb`  
		Last Modified: Fri, 09 Dec 2022 17:52:18 GMT  
		Size: 49.4 MB (49414568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12636ca6c95502ab17e340d2f6b112367aba4ac1e20f7ab8163b4b68fcb66602`  
		Last Modified: Fri, 09 Dec 2022 17:52:13 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; 386

```console
$ docker pull varnish@sha256:27b8ea22e0b98f3d370da0d7b28926290fd3cc2096166cd9814a9191f978457c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.6 MB (59569325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bea02470a3246fa42ff058293f436786cc663210bee1fbcbec1b9576d4074e24`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 02:07:46 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Tue, 08 Nov 2022 18:42:10 GMT
ARG VARNISH_VERSION=7.2.1
# Tue, 08 Nov 2022 18:42:11 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Tue, 08 Nov 2022 18:42:12 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Tue, 08 Nov 2022 18:42:13 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 09 Dec 2022 17:42:21 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Fri, 09 Dec 2022 17:42:22 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Fri, 09 Dec 2022 17:42:23 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Fri, 09 Dec 2022 17:42:24 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 09 Dec 2022 17:42:25 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Fri, 09 Dec 2022 17:42:26 GMT
ENV VARNISH_SIZE=100M
# Fri, 09 Dec 2022 17:46:33 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 09 Dec 2022 17:46:33 GMT
WORKDIR /etc/varnish
# Fri, 09 Dec 2022 17:46:35 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 09 Dec 2022 17:46:35 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 09 Dec 2022 17:46:36 GMT
USER varnish
# Fri, 09 Dec 2022 17:46:37 GMT
EXPOSE 80 8443
# Fri, 09 Dec 2022 17:46:38 GMT
CMD []
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355d74fc07dbf50689ac17b0f5e0fbec1a8af7b1f9dcee17d46f5eff1976e107`  
		Last Modified: Fri, 09 Dec 2022 17:51:03 GMT  
		Size: 56.7 MB (56740309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca599fa8915fde7ecc73fd114e3d10d5de8df77430cab928b8d3de0fa748660`  
		Last Modified: Fri, 09 Dec 2022 17:50:56 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:d9b9fe178087cfb51751f8639988a578f97ea1fba591014f45c9e97105af44e1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49171305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d291f0165a1bba74dd02443b07f16dbd3610099d07f5b35b6db221e683c44db1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:17:20 GMT
ADD file:be31abb0aba89ed5ff9200736a1c46091abc3845d0e332efd5e5c874ef2c99d1 in / 
# Tue, 09 Aug 2022 17:17:21 GMT
CMD ["/bin/sh"]
# Tue, 15 Nov 2022 18:45:59 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Tue, 15 Nov 2022 18:45:59 GMT
ARG VARNISH_VERSION=7.2.1
# Tue, 15 Nov 2022 18:45:59 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Tue, 15 Nov 2022 18:46:00 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Tue, 15 Nov 2022 18:46:01 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 09 Dec 2022 18:23:43 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Fri, 09 Dec 2022 18:23:43 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Fri, 09 Dec 2022 18:23:44 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Fri, 09 Dec 2022 18:23:44 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 09 Dec 2022 18:23:44 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Fri, 09 Dec 2022 18:23:45 GMT
ENV VARNISH_SIZE=100M
# Fri, 09 Dec 2022 18:26:49 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 09 Dec 2022 18:26:50 GMT
WORKDIR /etc/varnish
# Fri, 09 Dec 2022 18:26:51 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 09 Dec 2022 18:26:51 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 09 Dec 2022 18:26:51 GMT
USER varnish
# Fri, 09 Dec 2022 18:26:52 GMT
EXPOSE 80 8443
# Fri, 09 Dec 2022 18:26:52 GMT
CMD []
```

-	Layers:
	-	`sha256:deb7065b3304c3a9834f31b8a53e8d6089060e9c6522668abd22f1f4d9f52ca7`  
		Last Modified: Tue, 09 Aug 2022 17:18:45 GMT  
		Size: 2.8 MB (2812989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03574054a01f0f8826848eadc2b4868a9b65c93aeea02a7c772806cb0685c5b`  
		Last Modified: Fri, 09 Dec 2022 18:28:45 GMT  
		Size: 46.4 MB (46357815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247857fc893c2b18ff450e4ccb0737d8ef6102933f4676e64a56141d824bd241`  
		Last Modified: Fri, 09 Dec 2022 18:28:32 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; s390x

```console
$ docker pull varnish@sha256:76127ff5d6570cf73bc4581690b687ed086bbdb9133031e768c158ed63d0670f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47639610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69d9ab461e74d3101ebf2639b6b85153995bd23a2c1aa8a28b04010ad87841f0`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Tue, 15 Nov 2022 13:45:26 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Tue, 15 Nov 2022 13:45:27 GMT
ARG VARNISH_VERSION=7.2.1
# Tue, 15 Nov 2022 13:45:28 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Tue, 15 Nov 2022 13:45:28 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Tue, 15 Nov 2022 13:45:29 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 09 Dec 2022 17:47:41 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Fri, 09 Dec 2022 17:47:42 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Fri, 09 Dec 2022 17:47:42 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Fri, 09 Dec 2022 17:47:42 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 09 Dec 2022 17:47:43 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Fri, 09 Dec 2022 17:47:43 GMT
ENV VARNISH_SIZE=100M
# Fri, 09 Dec 2022 17:50:02 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 09 Dec 2022 17:50:07 GMT
WORKDIR /etc/varnish
# Fri, 09 Dec 2022 17:50:07 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 09 Dec 2022 17:50:08 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 09 Dec 2022 17:50:08 GMT
USER varnish
# Fri, 09 Dec 2022 17:50:09 GMT
EXPOSE 80 8443
# Fri, 09 Dec 2022 17:50:09 GMT
CMD []
```

-	Layers:
	-	`sha256:cdf710f5b7ee39c5124c50c753228dc9b8b1c1c0a1a38f1413487548565445c3`  
		Last Modified: Tue, 09 Aug 2022 17:42:56 GMT  
		Size: 2.6 MB (2606087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6af5a3cf679c345cb17179d345e3eb2554e532099f5c4f9e9fab9aa7e9427a`  
		Last Modified: Fri, 09 Dec 2022 17:59:52 GMT  
		Size: 45.0 MB (45033026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936f6bf8d89d854c95fd8761e729b493edaa1757fa875c933ce1da1a392f805c`  
		Last Modified: Fri, 09 Dec 2022 17:59:47 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:fresh`

```console
$ docker pull varnish@sha256:3feac23caf88ff28673bcb4aa81ae8dd316e4476c260af1a2c6e201cfcf4786e
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
$ docker pull varnish@sha256:d64ca9b7756cb3a0eda02971eba4e2006311fc85c52ccd6e992475366ac5790a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106843191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16576fb65a911c2195ae8bb7ea33bf084f41b7348f2d20473af354a42e4f6761`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:38:29 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 09 Feb 2023 06:38:29 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 09 Feb 2023 06:38:29 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 09 Feb 2023 06:38:29 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 09 Feb 2023 06:38:29 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 09 Feb 2023 06:38:29 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 09 Feb 2023 06:38:29 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 09 Feb 2023 06:38:29 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 09 Feb 2023 06:38:30 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 09 Feb 2023 06:38:30 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Thu, 09 Feb 2023 06:38:30 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 06:41:50 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 09 Feb 2023 06:41:51 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 06:41:51 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 09 Feb 2023 06:41:51 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 06:41:51 GMT
USER varnish
# Thu, 09 Feb 2023 06:41:51 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 06:41:51 GMT
CMD []
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5849700d1633b0858d2a64844bb0fdd45c87607fcf429d07dbcacf1835ff2e0f`  
		Last Modified: Thu, 09 Feb 2023 06:48:10 GMT  
		Size: 75.4 MB (75430887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819e8388a2fe25ed89691731d6a3f4a2feb9a30cf8db8de9a72ef699909ea329`  
		Last Modified: Thu, 09 Feb 2023 06:48:00 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; arm variant v7

```console
$ docker pull varnish@sha256:667101f4287db71b7a21b99ed03b1190bf6ffec44a07c12406fac8f710cf287a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.2 MB (83169412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:293472e275cc824b762c201d32db85c29c22ad7c0462959504240f5c74f3f3b9`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Sat, 04 Feb 2023 09:59:36 GMT
ADD file:c3cb8f4527fa96e99a4741ecb398113f25f53389c173b74f6c2a5e39a6575c60 in / 
# Sat, 04 Feb 2023 09:59:36 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 21:19:28 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Sat, 04 Feb 2023 21:19:28 GMT
ARG VARNISH_VERSION=7.2.1
# Sat, 04 Feb 2023 21:19:28 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Sat, 04 Feb 2023 21:19:28 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Sat, 04 Feb 2023 21:19:29 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Sat, 04 Feb 2023 21:19:29 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Sat, 04 Feb 2023 21:19:29 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Sat, 04 Feb 2023 21:19:29 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Sat, 04 Feb 2023 21:19:29 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Sat, 04 Feb 2023 21:19:29 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Sat, 04 Feb 2023 21:19:29 GMT
ENV VARNISH_SIZE=100M
# Sat, 04 Feb 2023 21:22:30 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Sat, 04 Feb 2023 21:22:31 GMT
WORKDIR /etc/varnish
# Sat, 04 Feb 2023 21:22:31 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Sat, 04 Feb 2023 21:22:31 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sat, 04 Feb 2023 21:22:31 GMT
USER varnish
# Sat, 04 Feb 2023 21:22:31 GMT
EXPOSE 80 8443
# Sat, 04 Feb 2023 21:22:31 GMT
CMD []
```

-	Layers:
	-	`sha256:bd25bcdfbaa165120ee21b6567df395fe7d7b38da3cca0bcecee55a190e04aab`  
		Last Modified: Sat, 04 Feb 2023 10:06:24 GMT  
		Size: 26.6 MB (26559474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32aa6224c75d142f0a76142fa8ebabe4a311fc4ce23351e0248c29b47989d8f6`  
		Last Modified: Sat, 04 Feb 2023 21:29:24 GMT  
		Size: 56.6 MB (56609446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67957e16f03a30cd49c3c133970df3e4af0ca6c1d3517ade7f271caf5c636dbf`  
		Last Modified: Sat, 04 Feb 2023 21:29:15 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:070c65da2b8faf580eec672e0db795ded6285b428e1d39254f88244f6d2ba8fe
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.9 MB (100867420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa825a96e8e9266a3bf0501d85a6d0b2d4176c29895bd7b07085738e302fe068`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 08:43:56 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 09 Feb 2023 08:43:56 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 09 Feb 2023 08:43:56 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 09 Feb 2023 08:43:56 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 09 Feb 2023 08:43:56 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 09 Feb 2023 08:43:56 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 09 Feb 2023 08:43:56 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 09 Feb 2023 08:43:56 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 09 Feb 2023 08:43:57 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 09 Feb 2023 08:43:57 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Thu, 09 Feb 2023 08:43:57 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 08:46:49 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 09 Feb 2023 08:46:50 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 08:46:50 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 09 Feb 2023 08:46:50 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 08:46:50 GMT
USER varnish
# Thu, 09 Feb 2023 08:46:50 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 08:46:50 GMT
CMD []
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd593e410516ba146ca282d48deef73a7e2eaef76c1020ca6e524bc5aa4a6078`  
		Last Modified: Thu, 09 Feb 2023 08:51:51 GMT  
		Size: 70.8 MB (70804416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4459f721e7b5112ddc4a759e70ea9f389dbe7ea84abed0cf252d75110b8a00b1`  
		Last Modified: Thu, 09 Feb 2023 08:51:45 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; 386

```console
$ docker pull varnish@sha256:32e374f738c01546453d2edad6a6797b7eef8d9b4145e3a8f7cbb00886bf9aca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.2 MB (108223049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0847bbcdf260fc907bc7fc41a1e8607b6bab32fff55ecc9738733798c6d219e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 05:12:53 GMT
ADD file:7740abd3129d33122ce51153c0b6c3323b9cbe9ea0e81672e16b2d7b210d24e3 in / 
# Thu, 09 Feb 2023 05:12:53 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 11:28:46 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 09 Feb 2023 11:28:46 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 09 Feb 2023 11:28:47 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 09 Feb 2023 11:28:48 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 09 Feb 2023 11:28:49 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 09 Feb 2023 11:28:50 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 09 Feb 2023 11:28:51 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 09 Feb 2023 11:28:52 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 09 Feb 2023 11:28:53 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 09 Feb 2023 11:28:54 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Thu, 09 Feb 2023 11:28:55 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 11:31:41 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 09 Feb 2023 11:31:41 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 11:31:43 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 09 Feb 2023 11:31:43 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 11:31:44 GMT
USER varnish
# Thu, 09 Feb 2023 11:31:45 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 11:31:46 GMT
CMD []
```

-	Layers:
	-	`sha256:20744f4988404b1dee2cd438157b288d16a89da472583c0f04332ed389b258f8`  
		Last Modified: Thu, 09 Feb 2023 05:18:42 GMT  
		Size: 32.4 MB (32396875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f716893955fc8687049630d836de419a9ee4e31f969ac4c63da2c5780fa54c73`  
		Last Modified: Thu, 09 Feb 2023 11:36:33 GMT  
		Size: 75.8 MB (75825680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d3ab9c1eaecbdfad280dc92f39431564c14053c2af1d58d5b720a303be22c1`  
		Last Modified: Thu, 09 Feb 2023 11:36:23 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; ppc64le

```console
$ docker pull varnish@sha256:456e1ab0c95e2025140b7ad74c5f8f784cf929a523d49cf8572e57edd918828d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.1 MB (106108350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbf49277a8a95baf5ea51cfb4eb767ca3cb1a463eb7dd260477154c2407e4074`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 06:21:49 GMT
ADD file:b09577b8131a90731fdfb00b824a97dc65ccb51d484cb9004382035d64a5741c in / 
# Thu, 09 Feb 2023 06:21:52 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 11:49:24 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 09 Feb 2023 11:49:24 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 09 Feb 2023 11:49:25 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 09 Feb 2023 11:49:25 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 09 Feb 2023 11:49:26 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 09 Feb 2023 11:49:26 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 09 Feb 2023 11:49:26 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 09 Feb 2023 11:49:26 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 09 Feb 2023 11:49:27 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 09 Feb 2023 11:49:27 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Thu, 09 Feb 2023 11:49:27 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 11:56:31 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 09 Feb 2023 11:56:35 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 11:56:35 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 09 Feb 2023 11:56:36 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 11:56:38 GMT
USER varnish
# Thu, 09 Feb 2023 11:56:38 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 11:56:38 GMT
CMD []
```

-	Layers:
	-	`sha256:4ea90e1a094ae86c7950bbec99e7a79b08fae641ad5f3bc3af9081c925894c41`  
		Last Modified: Thu, 09 Feb 2023 06:28:27 GMT  
		Size: 35.3 MB (35289252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e5d4b8afc29eb5a60b400a5a3ed200436b51055825af9d162bd04699491d76`  
		Last Modified: Thu, 09 Feb 2023 12:12:18 GMT  
		Size: 70.8 MB (70818605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab21c5070a377ef6e57bbe6990d1043689f75fbc0c8b7e1f7050f1ec7268642`  
		Last Modified: Thu, 09 Feb 2023 12:12:00 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; s390x

```console
$ docker pull varnish@sha256:91374e1e9cf49dbdc947ad7908b9c4677f92abc06083dce76d8eab0e80814022
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.1 MB (87139320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c46fabb8d3b70dba47fcba3a588f2266fb2f5f72c7bf3eaa7306e997891f41ad`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 02:41:45 GMT
ADD file:dc3c16b50baeac5b9644e607c8df9606e9583f8598e3ba34bcdd69c669a5904c in / 
# Thu, 09 Feb 2023 02:41:46 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 04:31:11 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 09 Feb 2023 04:31:11 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 09 Feb 2023 04:31:11 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 09 Feb 2023 04:31:11 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 09 Feb 2023 04:31:11 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 09 Feb 2023 04:31:11 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 09 Feb 2023 04:31:12 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 09 Feb 2023 04:31:12 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 09 Feb 2023 04:31:12 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 09 Feb 2023 04:31:12 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Thu, 09 Feb 2023 04:31:12 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 04:35:02 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 09 Feb 2023 04:35:10 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 04:35:10 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 09 Feb 2023 04:35:11 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 04:35:12 GMT
USER varnish
# Thu, 09 Feb 2023 04:35:12 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 04:35:13 GMT
CMD []
```

-	Layers:
	-	`sha256:c2f78940fdfbfc5ce5d1d3cff3c27a319451aeb3ec12ff2473073516907fbce9`  
		Last Modified: Thu, 09 Feb 2023 02:46:06 GMT  
		Size: 29.6 MB (29647513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6956ec29c8de529c99c757cf901e5f2c77d691fc70707c44e776970c0071db9e`  
		Last Modified: Thu, 09 Feb 2023 04:42:56 GMT  
		Size: 57.5 MB (57491314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a38481f200bfa9b450cc4cebc812b08de7de18c35f4b7de12a835c601f2436`  
		Last Modified: Thu, 09 Feb 2023 04:42:49 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:fresh-alpine`

```console
$ docker pull varnish@sha256:0ae1260686d231b721e1dffba7ec421c95ab49f698e9b48fed675744fe144a4a
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
$ docker pull varnish@sha256:c6a7b674fa2e9a53c5ae0eadc57e835a1ed24ad81a717c76ba3c128a8d72db71
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.4 MB (59397542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:290f2c7d09415f1025c46ef26451df3246a538941b7f8b84ebe9a4918754c6f1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:23:08 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Tue, 08 Nov 2022 18:57:07 GMT
ARG VARNISH_VERSION=7.2.1
# Tue, 08 Nov 2022 18:57:07 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Tue, 08 Nov 2022 18:57:07 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Tue, 08 Nov 2022 18:57:07 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 09 Dec 2022 18:24:03 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Fri, 09 Dec 2022 18:24:04 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Fri, 09 Dec 2022 18:24:04 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Fri, 09 Dec 2022 18:24:04 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 09 Dec 2022 18:24:04 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Fri, 09 Dec 2022 18:24:04 GMT
ENV VARNISH_SIZE=100M
# Fri, 09 Dec 2022 18:25:19 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 09 Dec 2022 18:25:19 GMT
WORKDIR /etc/varnish
# Fri, 09 Dec 2022 18:25:19 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 09 Dec 2022 18:25:19 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 09 Dec 2022 18:25:20 GMT
USER varnish
# Fri, 09 Dec 2022 18:25:20 GMT
EXPOSE 80 8443
# Fri, 09 Dec 2022 18:25:20 GMT
CMD []
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cede921e2d42724a2365b66b858821b35b7e20527a43e585feaded18776e29e`  
		Last Modified: Fri, 09 Dec 2022 18:26:22 GMT  
		Size: 56.6 MB (56573532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26aa4aafc5f3e04e142b38aed4c4ab5be40fb074cbad3020e08b29142598b57c`  
		Last Modified: Fri, 09 Dec 2022 18:26:14 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:e66d31b1d8b6e119d0f044c545f8edaabb45276cfea6577928a19d9bc578b773
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45149649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfc50568e3c1ccdf4c5c1c666d75d7667f04ab218bf8a5b59f37d52fa054bcde`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 10 Nov 2022 19:57:41 GMT
ADD file:0bd18306f21937a9572e68c768f05f4a9d8341b40c2379a7bfcb857c77734a14 in / 
# Thu, 10 Nov 2022 19:57:41 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 13:51:48 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Fri, 11 Nov 2022 13:51:49 GMT
ARG VARNISH_VERSION=7.2.1
# Fri, 11 Nov 2022 13:51:49 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Fri, 11 Nov 2022 13:51:49 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Fri, 11 Nov 2022 13:51:49 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 09 Dec 2022 18:14:58 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Fri, 09 Dec 2022 18:14:58 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Fri, 09 Dec 2022 18:14:58 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Fri, 09 Dec 2022 18:14:58 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 09 Dec 2022 18:14:58 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Fri, 09 Dec 2022 18:14:59 GMT
ENV VARNISH_SIZE=100M
# Fri, 09 Dec 2022 18:16:25 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 09 Dec 2022 18:16:25 GMT
WORKDIR /etc/varnish
# Fri, 09 Dec 2022 18:16:25 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 09 Dec 2022 18:16:25 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 09 Dec 2022 18:16:25 GMT
USER varnish
# Fri, 09 Dec 2022 18:16:25 GMT
EXPOSE 80 8443
# Fri, 09 Dec 2022 18:16:25 GMT
CMD []
```

-	Layers:
	-	`sha256:59775c20a906b1a49edcdc41a700a795998979d6ecf8f8d9cd7cbdf45e686d81`  
		Last Modified: Tue, 09 Aug 2022 16:59:12 GMT  
		Size: 2.4 MB (2435092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f59a293f1456cae4428183939900b44f083b6bd1724fb73b56eab4c22f73c84`  
		Last Modified: Fri, 09 Dec 2022 18:18:21 GMT  
		Size: 42.7 MB (42714062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9188a361ad4c027cd69a7ccfc3bb2b141caf9024edc09c7742b0070d5fff8e`  
		Last Modified: Fri, 09 Dec 2022 18:18:14 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:9fde738bd7a1792db975b2f43f532b894aed6e28fd982814c09f52f93b9c0bb8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52133505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b3875632d7c932d6d21178f71d8d5e814ed41f152159ceea19652219c63e115`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Tue, 15 Nov 2022 11:44:18 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Tue, 15 Nov 2022 11:44:18 GMT
ARG VARNISH_VERSION=7.2.1
# Tue, 15 Nov 2022 11:44:18 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Tue, 15 Nov 2022 11:44:18 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Tue, 15 Nov 2022 11:44:18 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 09 Dec 2022 17:50:18 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Fri, 09 Dec 2022 17:50:18 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Fri, 09 Dec 2022 17:50:19 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Fri, 09 Dec 2022 17:50:19 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 09 Dec 2022 17:50:19 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Fri, 09 Dec 2022 17:50:19 GMT
ENV VARNISH_SIZE=100M
# Fri, 09 Dec 2022 17:51:24 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 09 Dec 2022 17:51:25 GMT
WORKDIR /etc/varnish
# Fri, 09 Dec 2022 17:51:25 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 09 Dec 2022 17:51:25 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 09 Dec 2022 17:51:25 GMT
USER varnish
# Fri, 09 Dec 2022 17:51:25 GMT
EXPOSE 80 8443
# Fri, 09 Dec 2022 17:51:25 GMT
CMD []
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d55913ffdb6c1584033b1dc44e04a7da2c51610e945c943b3bda4f7103ddcb`  
		Last Modified: Fri, 09 Dec 2022 17:52:18 GMT  
		Size: 49.4 MB (49414568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12636ca6c95502ab17e340d2f6b112367aba4ac1e20f7ab8163b4b68fcb66602`  
		Last Modified: Fri, 09 Dec 2022 17:52:13 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; 386

```console
$ docker pull varnish@sha256:27b8ea22e0b98f3d370da0d7b28926290fd3cc2096166cd9814a9191f978457c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.6 MB (59569325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bea02470a3246fa42ff058293f436786cc663210bee1fbcbec1b9576d4074e24`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 02:07:46 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Tue, 08 Nov 2022 18:42:10 GMT
ARG VARNISH_VERSION=7.2.1
# Tue, 08 Nov 2022 18:42:11 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Tue, 08 Nov 2022 18:42:12 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Tue, 08 Nov 2022 18:42:13 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 09 Dec 2022 17:42:21 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Fri, 09 Dec 2022 17:42:22 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Fri, 09 Dec 2022 17:42:23 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Fri, 09 Dec 2022 17:42:24 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 09 Dec 2022 17:42:25 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Fri, 09 Dec 2022 17:42:26 GMT
ENV VARNISH_SIZE=100M
# Fri, 09 Dec 2022 17:46:33 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 09 Dec 2022 17:46:33 GMT
WORKDIR /etc/varnish
# Fri, 09 Dec 2022 17:46:35 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 09 Dec 2022 17:46:35 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 09 Dec 2022 17:46:36 GMT
USER varnish
# Fri, 09 Dec 2022 17:46:37 GMT
EXPOSE 80 8443
# Fri, 09 Dec 2022 17:46:38 GMT
CMD []
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355d74fc07dbf50689ac17b0f5e0fbec1a8af7b1f9dcee17d46f5eff1976e107`  
		Last Modified: Fri, 09 Dec 2022 17:51:03 GMT  
		Size: 56.7 MB (56740309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca599fa8915fde7ecc73fd114e3d10d5de8df77430cab928b8d3de0fa748660`  
		Last Modified: Fri, 09 Dec 2022 17:50:56 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:d9b9fe178087cfb51751f8639988a578f97ea1fba591014f45c9e97105af44e1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49171305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d291f0165a1bba74dd02443b07f16dbd3610099d07f5b35b6db221e683c44db1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:17:20 GMT
ADD file:be31abb0aba89ed5ff9200736a1c46091abc3845d0e332efd5e5c874ef2c99d1 in / 
# Tue, 09 Aug 2022 17:17:21 GMT
CMD ["/bin/sh"]
# Tue, 15 Nov 2022 18:45:59 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Tue, 15 Nov 2022 18:45:59 GMT
ARG VARNISH_VERSION=7.2.1
# Tue, 15 Nov 2022 18:45:59 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Tue, 15 Nov 2022 18:46:00 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Tue, 15 Nov 2022 18:46:01 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 09 Dec 2022 18:23:43 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Fri, 09 Dec 2022 18:23:43 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Fri, 09 Dec 2022 18:23:44 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Fri, 09 Dec 2022 18:23:44 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 09 Dec 2022 18:23:44 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Fri, 09 Dec 2022 18:23:45 GMT
ENV VARNISH_SIZE=100M
# Fri, 09 Dec 2022 18:26:49 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 09 Dec 2022 18:26:50 GMT
WORKDIR /etc/varnish
# Fri, 09 Dec 2022 18:26:51 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 09 Dec 2022 18:26:51 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 09 Dec 2022 18:26:51 GMT
USER varnish
# Fri, 09 Dec 2022 18:26:52 GMT
EXPOSE 80 8443
# Fri, 09 Dec 2022 18:26:52 GMT
CMD []
```

-	Layers:
	-	`sha256:deb7065b3304c3a9834f31b8a53e8d6089060e9c6522668abd22f1f4d9f52ca7`  
		Last Modified: Tue, 09 Aug 2022 17:18:45 GMT  
		Size: 2.8 MB (2812989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03574054a01f0f8826848eadc2b4868a9b65c93aeea02a7c772806cb0685c5b`  
		Last Modified: Fri, 09 Dec 2022 18:28:45 GMT  
		Size: 46.4 MB (46357815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247857fc893c2b18ff450e4ccb0737d8ef6102933f4676e64a56141d824bd241`  
		Last Modified: Fri, 09 Dec 2022 18:28:32 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:76127ff5d6570cf73bc4581690b687ed086bbdb9133031e768c158ed63d0670f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47639610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69d9ab461e74d3101ebf2639b6b85153995bd23a2c1aa8a28b04010ad87841f0`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Tue, 15 Nov 2022 13:45:26 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Tue, 15 Nov 2022 13:45:27 GMT
ARG VARNISH_VERSION=7.2.1
# Tue, 15 Nov 2022 13:45:28 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Tue, 15 Nov 2022 13:45:28 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Tue, 15 Nov 2022 13:45:29 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 09 Dec 2022 17:47:41 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Fri, 09 Dec 2022 17:47:42 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Fri, 09 Dec 2022 17:47:42 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Fri, 09 Dec 2022 17:47:42 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 09 Dec 2022 17:47:43 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Fri, 09 Dec 2022 17:47:43 GMT
ENV VARNISH_SIZE=100M
# Fri, 09 Dec 2022 17:50:02 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 09 Dec 2022 17:50:07 GMT
WORKDIR /etc/varnish
# Fri, 09 Dec 2022 17:50:07 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 09 Dec 2022 17:50:08 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 09 Dec 2022 17:50:08 GMT
USER varnish
# Fri, 09 Dec 2022 17:50:09 GMT
EXPOSE 80 8443
# Fri, 09 Dec 2022 17:50:09 GMT
CMD []
```

-	Layers:
	-	`sha256:cdf710f5b7ee39c5124c50c753228dc9b8b1c1c0a1a38f1413487548565445c3`  
		Last Modified: Tue, 09 Aug 2022 17:42:56 GMT  
		Size: 2.6 MB (2606087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6af5a3cf679c345cb17179d345e3eb2554e532099f5c4f9e9fab9aa7e9427a`  
		Last Modified: Fri, 09 Dec 2022 17:59:52 GMT  
		Size: 45.0 MB (45033026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936f6bf8d89d854c95fd8761e729b493edaa1757fa875c933ce1da1a392f805c`  
		Last Modified: Fri, 09 Dec 2022 17:59:47 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:latest`

```console
$ docker pull varnish@sha256:3feac23caf88ff28673bcb4aa81ae8dd316e4476c260af1a2c6e201cfcf4786e
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
$ docker pull varnish@sha256:d64ca9b7756cb3a0eda02971eba4e2006311fc85c52ccd6e992475366ac5790a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106843191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16576fb65a911c2195ae8bb7ea33bf084f41b7348f2d20473af354a42e4f6761`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:38:29 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 09 Feb 2023 06:38:29 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 09 Feb 2023 06:38:29 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 09 Feb 2023 06:38:29 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 09 Feb 2023 06:38:29 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 09 Feb 2023 06:38:29 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 09 Feb 2023 06:38:29 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 09 Feb 2023 06:38:29 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 09 Feb 2023 06:38:30 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 09 Feb 2023 06:38:30 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Thu, 09 Feb 2023 06:38:30 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 06:41:50 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 09 Feb 2023 06:41:51 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 06:41:51 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 09 Feb 2023 06:41:51 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 06:41:51 GMT
USER varnish
# Thu, 09 Feb 2023 06:41:51 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 06:41:51 GMT
CMD []
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5849700d1633b0858d2a64844bb0fdd45c87607fcf429d07dbcacf1835ff2e0f`  
		Last Modified: Thu, 09 Feb 2023 06:48:10 GMT  
		Size: 75.4 MB (75430887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819e8388a2fe25ed89691731d6a3f4a2feb9a30cf8db8de9a72ef699909ea329`  
		Last Modified: Thu, 09 Feb 2023 06:48:00 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; arm variant v7

```console
$ docker pull varnish@sha256:667101f4287db71b7a21b99ed03b1190bf6ffec44a07c12406fac8f710cf287a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.2 MB (83169412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:293472e275cc824b762c201d32db85c29c22ad7c0462959504240f5c74f3f3b9`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Sat, 04 Feb 2023 09:59:36 GMT
ADD file:c3cb8f4527fa96e99a4741ecb398113f25f53389c173b74f6c2a5e39a6575c60 in / 
# Sat, 04 Feb 2023 09:59:36 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 21:19:28 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Sat, 04 Feb 2023 21:19:28 GMT
ARG VARNISH_VERSION=7.2.1
# Sat, 04 Feb 2023 21:19:28 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Sat, 04 Feb 2023 21:19:28 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Sat, 04 Feb 2023 21:19:29 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Sat, 04 Feb 2023 21:19:29 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Sat, 04 Feb 2023 21:19:29 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Sat, 04 Feb 2023 21:19:29 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Sat, 04 Feb 2023 21:19:29 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Sat, 04 Feb 2023 21:19:29 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Sat, 04 Feb 2023 21:19:29 GMT
ENV VARNISH_SIZE=100M
# Sat, 04 Feb 2023 21:22:30 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Sat, 04 Feb 2023 21:22:31 GMT
WORKDIR /etc/varnish
# Sat, 04 Feb 2023 21:22:31 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Sat, 04 Feb 2023 21:22:31 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sat, 04 Feb 2023 21:22:31 GMT
USER varnish
# Sat, 04 Feb 2023 21:22:31 GMT
EXPOSE 80 8443
# Sat, 04 Feb 2023 21:22:31 GMT
CMD []
```

-	Layers:
	-	`sha256:bd25bcdfbaa165120ee21b6567df395fe7d7b38da3cca0bcecee55a190e04aab`  
		Last Modified: Sat, 04 Feb 2023 10:06:24 GMT  
		Size: 26.6 MB (26559474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32aa6224c75d142f0a76142fa8ebabe4a311fc4ce23351e0248c29b47989d8f6`  
		Last Modified: Sat, 04 Feb 2023 21:29:24 GMT  
		Size: 56.6 MB (56609446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67957e16f03a30cd49c3c133970df3e4af0ca6c1d3517ade7f271caf5c636dbf`  
		Last Modified: Sat, 04 Feb 2023 21:29:15 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:070c65da2b8faf580eec672e0db795ded6285b428e1d39254f88244f6d2ba8fe
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.9 MB (100867420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa825a96e8e9266a3bf0501d85a6d0b2d4176c29895bd7b07085738e302fe068`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 08:43:56 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 09 Feb 2023 08:43:56 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 09 Feb 2023 08:43:56 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 09 Feb 2023 08:43:56 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 09 Feb 2023 08:43:56 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 09 Feb 2023 08:43:56 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 09 Feb 2023 08:43:56 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 09 Feb 2023 08:43:56 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 09 Feb 2023 08:43:57 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 09 Feb 2023 08:43:57 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Thu, 09 Feb 2023 08:43:57 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 08:46:49 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 09 Feb 2023 08:46:50 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 08:46:50 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 09 Feb 2023 08:46:50 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 08:46:50 GMT
USER varnish
# Thu, 09 Feb 2023 08:46:50 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 08:46:50 GMT
CMD []
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd593e410516ba146ca282d48deef73a7e2eaef76c1020ca6e524bc5aa4a6078`  
		Last Modified: Thu, 09 Feb 2023 08:51:51 GMT  
		Size: 70.8 MB (70804416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4459f721e7b5112ddc4a759e70ea9f389dbe7ea84abed0cf252d75110b8a00b1`  
		Last Modified: Thu, 09 Feb 2023 08:51:45 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; 386

```console
$ docker pull varnish@sha256:32e374f738c01546453d2edad6a6797b7eef8d9b4145e3a8f7cbb00886bf9aca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.2 MB (108223049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0847bbcdf260fc907bc7fc41a1e8607b6bab32fff55ecc9738733798c6d219e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 05:12:53 GMT
ADD file:7740abd3129d33122ce51153c0b6c3323b9cbe9ea0e81672e16b2d7b210d24e3 in / 
# Thu, 09 Feb 2023 05:12:53 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 11:28:46 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 09 Feb 2023 11:28:46 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 09 Feb 2023 11:28:47 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 09 Feb 2023 11:28:48 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 09 Feb 2023 11:28:49 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 09 Feb 2023 11:28:50 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 09 Feb 2023 11:28:51 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 09 Feb 2023 11:28:52 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 09 Feb 2023 11:28:53 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 09 Feb 2023 11:28:54 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Thu, 09 Feb 2023 11:28:55 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 11:31:41 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 09 Feb 2023 11:31:41 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 11:31:43 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 09 Feb 2023 11:31:43 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 11:31:44 GMT
USER varnish
# Thu, 09 Feb 2023 11:31:45 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 11:31:46 GMT
CMD []
```

-	Layers:
	-	`sha256:20744f4988404b1dee2cd438157b288d16a89da472583c0f04332ed389b258f8`  
		Last Modified: Thu, 09 Feb 2023 05:18:42 GMT  
		Size: 32.4 MB (32396875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f716893955fc8687049630d836de419a9ee4e31f969ac4c63da2c5780fa54c73`  
		Last Modified: Thu, 09 Feb 2023 11:36:33 GMT  
		Size: 75.8 MB (75825680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d3ab9c1eaecbdfad280dc92f39431564c14053c2af1d58d5b720a303be22c1`  
		Last Modified: Thu, 09 Feb 2023 11:36:23 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; ppc64le

```console
$ docker pull varnish@sha256:456e1ab0c95e2025140b7ad74c5f8f784cf929a523d49cf8572e57edd918828d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.1 MB (106108350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbf49277a8a95baf5ea51cfb4eb767ca3cb1a463eb7dd260477154c2407e4074`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 06:21:49 GMT
ADD file:b09577b8131a90731fdfb00b824a97dc65ccb51d484cb9004382035d64a5741c in / 
# Thu, 09 Feb 2023 06:21:52 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 11:49:24 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 09 Feb 2023 11:49:24 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 09 Feb 2023 11:49:25 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 09 Feb 2023 11:49:25 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 09 Feb 2023 11:49:26 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 09 Feb 2023 11:49:26 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 09 Feb 2023 11:49:26 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 09 Feb 2023 11:49:26 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 09 Feb 2023 11:49:27 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 09 Feb 2023 11:49:27 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Thu, 09 Feb 2023 11:49:27 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 11:56:31 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 09 Feb 2023 11:56:35 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 11:56:35 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 09 Feb 2023 11:56:36 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 11:56:38 GMT
USER varnish
# Thu, 09 Feb 2023 11:56:38 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 11:56:38 GMT
CMD []
```

-	Layers:
	-	`sha256:4ea90e1a094ae86c7950bbec99e7a79b08fae641ad5f3bc3af9081c925894c41`  
		Last Modified: Thu, 09 Feb 2023 06:28:27 GMT  
		Size: 35.3 MB (35289252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e5d4b8afc29eb5a60b400a5a3ed200436b51055825af9d162bd04699491d76`  
		Last Modified: Thu, 09 Feb 2023 12:12:18 GMT  
		Size: 70.8 MB (70818605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab21c5070a377ef6e57bbe6990d1043689f75fbc0c8b7e1f7050f1ec7268642`  
		Last Modified: Thu, 09 Feb 2023 12:12:00 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; s390x

```console
$ docker pull varnish@sha256:91374e1e9cf49dbdc947ad7908b9c4677f92abc06083dce76d8eab0e80814022
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.1 MB (87139320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c46fabb8d3b70dba47fcba3a588f2266fb2f5f72c7bf3eaa7306e997891f41ad`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 02:41:45 GMT
ADD file:dc3c16b50baeac5b9644e607c8df9606e9583f8598e3ba34bcdd69c669a5904c in / 
# Thu, 09 Feb 2023 02:41:46 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 04:31:11 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Thu, 09 Feb 2023 04:31:11 GMT
ARG VARNISH_VERSION=7.2.1
# Thu, 09 Feb 2023 04:31:11 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Thu, 09 Feb 2023 04:31:11 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Thu, 09 Feb 2023 04:31:11 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Thu, 09 Feb 2023 04:31:11 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 09 Feb 2023 04:31:12 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Thu, 09 Feb 2023 04:31:12 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Thu, 09 Feb 2023 04:31:12 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 09 Feb 2023 04:31:12 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Thu, 09 Feb 2023 04:31:12 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 04:35:02 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 09 Feb 2023 04:35:10 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 04:35:10 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 09 Feb 2023 04:35:11 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 04:35:12 GMT
USER varnish
# Thu, 09 Feb 2023 04:35:12 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 04:35:13 GMT
CMD []
```

-	Layers:
	-	`sha256:c2f78940fdfbfc5ce5d1d3cff3c27a319451aeb3ec12ff2473073516907fbce9`  
		Last Modified: Thu, 09 Feb 2023 02:46:06 GMT  
		Size: 29.6 MB (29647513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6956ec29c8de529c99c757cf901e5f2c77d691fc70707c44e776970c0071db9e`  
		Last Modified: Thu, 09 Feb 2023 04:42:56 GMT  
		Size: 57.5 MB (57491314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a38481f200bfa9b450cc4cebc812b08de7de18c35f4b7de12a835c601f2436`  
		Last Modified: Thu, 09 Feb 2023 04:42:49 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:old`

```console
$ docker pull varnish@sha256:e9456a472f77f375121d88078702733c80bccfa30f5ee471357f6c88d3193d8e
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
$ docker pull varnish@sha256:86b5b917a68ee39dc513d1017569eb600357c1d773e0b29c7d7e936d41fdb968
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.5 MB (106537864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f711ef0df5359ec75fbc8ecfb0a6d7a3817bab883c77f1573ec780770b149fda`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:42:09 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 09 Feb 2023 06:42:09 GMT
ARG VARNISH_VERSION=7.1.2
# Thu, 09 Feb 2023 06:42:09 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Thu, 09 Feb 2023 06:42:09 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 09 Feb 2023 06:42:10 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 09 Feb 2023 06:42:10 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 09 Feb 2023 06:42:10 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 09 Feb 2023 06:42:10 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 09 Feb 2023 06:42:10 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 09 Feb 2023 06:42:10 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Thu, 09 Feb 2023 06:42:10 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 06:45:03 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.2.tgz -o $tmpdir/orig.tgz;     echo "e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 09 Feb 2023 06:45:03 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 06:45:03 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 09 Feb 2023 06:45:04 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 06:45:04 GMT
USER varnish
# Thu, 09 Feb 2023 06:45:04 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 06:45:04 GMT
CMD []
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45419548745e83c966d460c337d99ce0f8bc4197cd132a7152c2bee977289c2`  
		Last Modified: Thu, 09 Feb 2023 06:48:34 GMT  
		Size: 75.1 MB (75125563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9709f37aae9d1c1f49e6e2b5d00cfe737700ec9560876ea55e9f18b44cab188f`  
		Last Modified: Thu, 09 Feb 2023 06:48:24 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; arm variant v7

```console
$ docker pull varnish@sha256:af440494a9fa63f6e01ab2de90f7511757acffa9f5a6a3d99091307b05143f7d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.9 MB (82883084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30142de2126bc95650930d00a49e560bf838c6bd56af0c704f1b89dd7277be67`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Sat, 04 Feb 2023 09:59:36 GMT
ADD file:c3cb8f4527fa96e99a4741ecb398113f25f53389c173b74f6c2a5e39a6575c60 in / 
# Sat, 04 Feb 2023 09:59:36 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 21:22:46 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Sat, 04 Feb 2023 21:22:46 GMT
ARG VARNISH_VERSION=7.1.2
# Sat, 04 Feb 2023 21:22:46 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Sat, 04 Feb 2023 21:22:46 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Sat, 04 Feb 2023 21:22:46 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Sat, 04 Feb 2023 21:22:46 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Sat, 04 Feb 2023 21:22:46 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Sat, 04 Feb 2023 21:22:46 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Sat, 04 Feb 2023 21:22:46 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Sat, 04 Feb 2023 21:22:46 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Sat, 04 Feb 2023 21:22:46 GMT
ENV VARNISH_SIZE=100M
# Sat, 04 Feb 2023 21:25:38 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.2.tgz -o $tmpdir/orig.tgz;     echo "e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Sat, 04 Feb 2023 21:25:39 GMT
WORKDIR /etc/varnish
# Sat, 04 Feb 2023 21:25:39 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Sat, 04 Feb 2023 21:25:39 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sat, 04 Feb 2023 21:25:39 GMT
USER varnish
# Sat, 04 Feb 2023 21:25:39 GMT
EXPOSE 80 8443
# Sat, 04 Feb 2023 21:25:39 GMT
CMD []
```

-	Layers:
	-	`sha256:bd25bcdfbaa165120ee21b6567df395fe7d7b38da3cca0bcecee55a190e04aab`  
		Last Modified: Sat, 04 Feb 2023 10:06:24 GMT  
		Size: 26.6 MB (26559474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a86cf7003c8f00c3a87657fb934e5c12a0414057288dcf7f8d1c94edb9d665`  
		Last Modified: Sat, 04 Feb 2023 21:29:54 GMT  
		Size: 56.3 MB (56323117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769df1d3e88475c39dda498ae716e7af2815967f933c5cede97335326f57ccaf`  
		Last Modified: Sat, 04 Feb 2023 21:29:45 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:0a30e53f8a879d0694179b1b1f4c333137a40a4b5f0c5333eb19073a96f2f37d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100553785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0280926bf0f5644eeb444f60b474c1f930ab6f2b993bef702237ef1acef0e39d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 08:47:05 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 09 Feb 2023 08:47:06 GMT
ARG VARNISH_VERSION=7.1.2
# Thu, 09 Feb 2023 08:47:06 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Thu, 09 Feb 2023 08:47:06 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 09 Feb 2023 08:47:06 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 09 Feb 2023 08:47:06 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 09 Feb 2023 08:47:06 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 09 Feb 2023 08:47:06 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 09 Feb 2023 08:47:06 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 09 Feb 2023 08:47:06 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Thu, 09 Feb 2023 08:47:06 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 08:49:24 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.2.tgz -o $tmpdir/orig.tgz;     echo "e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 09 Feb 2023 08:49:24 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 08:49:24 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 09 Feb 2023 08:49:24 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 08:49:24 GMT
USER varnish
# Thu, 09 Feb 2023 08:49:25 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 08:49:25 GMT
CMD []
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2d201a526e5c2cd221f64119321ea6485287d221c398880175d45ad922cac8`  
		Last Modified: Thu, 09 Feb 2023 08:52:21 GMT  
		Size: 70.5 MB (70490781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b57b0db05e8c4d5f84e5ec7882fce9b2d3f2e59ef0a762d685f38862463c76f`  
		Last Modified: Thu, 09 Feb 2023 08:52:13 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; 386

```console
$ docker pull varnish@sha256:ca5c1980e1e095a68397f8b5823d53ebebeb77685c42b22e5e2c20ad2f87121a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.9 MB (107917601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43ff32c9d6df2db2894a8b138d4ed404865bd95b5ba4c2cf7db9d4795031ab1f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 05:12:53 GMT
ADD file:7740abd3129d33122ce51153c0b6c3323b9cbe9ea0e81672e16b2d7b210d24e3 in / 
# Thu, 09 Feb 2023 05:12:53 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 11:32:02 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 09 Feb 2023 11:32:03 GMT
ARG VARNISH_VERSION=7.1.2
# Thu, 09 Feb 2023 11:32:04 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Thu, 09 Feb 2023 11:32:05 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 09 Feb 2023 11:32:06 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 09 Feb 2023 11:32:07 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 09 Feb 2023 11:32:08 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 09 Feb 2023 11:32:09 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 09 Feb 2023 11:32:10 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 09 Feb 2023 11:32:11 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Thu, 09 Feb 2023 11:32:12 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 11:35:05 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.2.tgz -o $tmpdir/orig.tgz;     echo "e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 09 Feb 2023 11:35:05 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 11:35:07 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 09 Feb 2023 11:35:07 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 11:35:08 GMT
USER varnish
# Thu, 09 Feb 2023 11:35:09 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 11:35:10 GMT
CMD []
```

-	Layers:
	-	`sha256:20744f4988404b1dee2cd438157b288d16a89da472583c0f04332ed389b258f8`  
		Last Modified: Thu, 09 Feb 2023 05:18:42 GMT  
		Size: 32.4 MB (32396875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0573a6fdb6f67f86faa1dce42564d76e6997e8130436cdf49ba43e7953a4411`  
		Last Modified: Thu, 09 Feb 2023 11:37:10 GMT  
		Size: 75.5 MB (75520232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6184742911a33db3f684db4f78b9b476388a95e13bc7d5c92e880436dc0ba6`  
		Last Modified: Thu, 09 Feb 2023 11:37:01 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; ppc64le

```console
$ docker pull varnish@sha256:a66bc11c56528ecd014a1e98d6ec8dc78342780cb7ee86f27e13fdaf727b578a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.8 MB (105819665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:564f0c4cff12c34e206ca62da60e6adc2167316b48e5be13d5879104a4cfd813`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 06:21:49 GMT
ADD file:b09577b8131a90731fdfb00b824a97dc65ccb51d484cb9004382035d64a5741c in / 
# Thu, 09 Feb 2023 06:21:52 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 11:56:55 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 09 Feb 2023 11:56:56 GMT
ARG VARNISH_VERSION=7.1.2
# Thu, 09 Feb 2023 11:56:56 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Thu, 09 Feb 2023 11:56:57 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 09 Feb 2023 11:56:57 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 09 Feb 2023 11:56:58 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 09 Feb 2023 11:56:58 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 09 Feb 2023 11:56:58 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 09 Feb 2023 11:56:59 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 09 Feb 2023 11:56:59 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Thu, 09 Feb 2023 11:56:59 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 12:04:06 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.2.tgz -o $tmpdir/orig.tgz;     echo "e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 09 Feb 2023 12:04:09 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 12:04:10 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 09 Feb 2023 12:04:10 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 12:04:11 GMT
USER varnish
# Thu, 09 Feb 2023 12:04:11 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 12:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:4ea90e1a094ae86c7950bbec99e7a79b08fae641ad5f3bc3af9081c925894c41`  
		Last Modified: Thu, 09 Feb 2023 06:28:27 GMT  
		Size: 35.3 MB (35289252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae58755fff07f0f195cbf87771a105e6741fe9dfeec0b41be3d8034b67cfbe9e`  
		Last Modified: Thu, 09 Feb 2023 12:12:56 GMT  
		Size: 70.5 MB (70529918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e616fbd77e4b0b793bea388a655624c763b53737dcaa1c492e7b39385e583c1`  
		Last Modified: Thu, 09 Feb 2023 12:12:38 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; s390x

```console
$ docker pull varnish@sha256:e75e34fba93f3f32d106700d4e93c5c9707eb9eb32058da5f1328e8e4ad5d27c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.8 MB (86833950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aebf2a458caabeda0bd00d1cba9bbc14c65034713a39b9385e47c504a9ac5036`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:43:11 GMT
ADD file:c1d41928e802c0b63beb07130c33bcc6dbdeb380a7f47510163cb176891e682a in / 
# Wed, 21 Dec 2022 01:43:14 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 10:26:01 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Wed, 21 Dec 2022 10:26:02 GMT
ARG VARNISH_VERSION=7.1.2
# Wed, 21 Dec 2022 10:26:02 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Wed, 21 Dec 2022 10:26:02 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Wed, 21 Dec 2022 10:26:02 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Wed, 21 Dec 2022 10:26:02 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Wed, 21 Dec 2022 10:26:03 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Wed, 21 Dec 2022 10:26:03 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Wed, 21 Dec 2022 10:26:03 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 21 Dec 2022 10:26:03 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 21 Dec 2022 10:26:04 GMT
ENV VARNISH_SIZE=100M
# Tue, 10 Jan 2023 01:41:58 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.2.tgz -o $tmpdir/orig.tgz;     echo "e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 10 Jan 2023 01:42:07 GMT
WORKDIR /etc/varnish
# Tue, 10 Jan 2023 01:42:07 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 10 Jan 2023 01:42:08 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 10 Jan 2023 01:42:08 GMT
USER varnish
# Tue, 10 Jan 2023 01:42:09 GMT
EXPOSE 80 8443
# Tue, 10 Jan 2023 01:42:09 GMT
CMD []
```

-	Layers:
	-	`sha256:197dcf20f55386b4c3f5fbace4720b64b5b0b606658b4ea9925121b9dbe7d638`  
		Last Modified: Wed, 21 Dec 2022 01:49:12 GMT  
		Size: 29.6 MB (29629760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d4c9c347e9b7f6ec4e2913f77427f763121ee4c5c1581c98442b5f1196eaa1`  
		Last Modified: Tue, 10 Jan 2023 01:43:26 GMT  
		Size: 57.2 MB (57203697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44b8332de2d27a2172b14f1b3da08d4945e94d884acb16dc735410d206be275`  
		Last Modified: Tue, 10 Jan 2023 01:43:18 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:old-alpine`

```console
$ docker pull varnish@sha256:3331356f8f0755e4e3ed11e499aede3598eb762db833fc1d8061c11327c9c212
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
$ docker pull varnish@sha256:bfc65610836fc2c37e08b84bb6f240889b355da18b842eb9348067d7750f04ce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.1 MB (59090797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3cdb897373eeab8d7f7fc2ff61e7991f4a238437ede05a3ff5bf9848fc43411`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:24:33 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 08 Nov 2022 19:01:38 GMT
ARG VARNISH_VERSION=7.1.2
# Tue, 08 Nov 2022 19:01:38 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Tue, 08 Nov 2022 19:01:38 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 08 Nov 2022 19:01:38 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 08 Nov 2022 19:01:38 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 08 Nov 2022 19:01:39 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 08 Nov 2022 19:01:39 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 08 Nov 2022 19:01:39 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 08 Nov 2022 19:01:39 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Tue, 08 Nov 2022 19:01:39 GMT
ENV VARNISH_SIZE=100M
# Tue, 08 Nov 2022 19:02:55 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Tue, 08 Nov 2022 19:02:55 GMT
WORKDIR /etc/varnish
# Tue, 08 Nov 2022 19:02:55 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 08 Nov 2022 19:02:55 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 08 Nov 2022 19:02:55 GMT
USER varnish
# Tue, 08 Nov 2022 19:02:55 GMT
EXPOSE 80 8443
# Tue, 08 Nov 2022 19:02:56 GMT
CMD []
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670d3e80e9abfb3a928cc7c4731595397e55cb0ce688957e59cfd484638c4232`  
		Last Modified: Tue, 08 Nov 2022 19:07:01 GMT  
		Size: 56.3 MB (56266789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c2c314e27890a793acce697402def118c2653924d827e52bbf967c8bda1928`  
		Last Modified: Tue, 08 Nov 2022 19:06:54 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:e4973a41b8c02a57dea2fbde4bf421a8a8ffdb78fb88965bd67696865b0d0f22
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44857379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7619084158717a1a17c4ed5501e554e505399f0a94aab05362677d3a16b044fd`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 10 Nov 2022 19:57:41 GMT
ADD file:0bd18306f21937a9572e68c768f05f4a9d8341b40c2379a7bfcb857c77734a14 in / 
# Thu, 10 Nov 2022 19:57:41 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 13:53:37 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Fri, 11 Nov 2022 13:53:37 GMT
ARG VARNISH_VERSION=7.1.2
# Fri, 11 Nov 2022 13:53:37 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Fri, 11 Nov 2022 13:53:37 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Fri, 11 Nov 2022 13:53:37 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Fri, 11 Nov 2022 13:53:37 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 11 Nov 2022 13:53:37 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Fri, 11 Nov 2022 13:53:37 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Fri, 11 Nov 2022 13:53:38 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 11 Nov 2022 13:53:38 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Fri, 11 Nov 2022 13:53:38 GMT
ENV VARNISH_SIZE=100M
# Fri, 11 Nov 2022 13:54:56 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 11 Nov 2022 13:54:56 GMT
WORKDIR /etc/varnish
# Fri, 11 Nov 2022 13:54:56 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 11 Nov 2022 13:54:56 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 11 Nov 2022 13:54:56 GMT
USER varnish
# Fri, 11 Nov 2022 13:54:57 GMT
EXPOSE 80 8443
# Fri, 11 Nov 2022 13:54:57 GMT
CMD []
```

-	Layers:
	-	`sha256:59775c20a906b1a49edcdc41a700a795998979d6ecf8f8d9cd7cbdf45e686d81`  
		Last Modified: Tue, 09 Aug 2022 16:59:12 GMT  
		Size: 2.4 MB (2435092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2419579e60811439aabf58796ee9d89983cd314305eeeab0808489234c9db1a7`  
		Last Modified: Fri, 11 Nov 2022 13:56:32 GMT  
		Size: 42.4 MB (42421790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55eae22e1ead549cfa2f80d74a145fa6455e60c7660da0ca8752ec2383251fd9`  
		Last Modified: Fri, 11 Nov 2022 13:56:26 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:6f2a92bc4631e45fdf46e30ca2a678fc18d69a796794c78081fdfb2177539796
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51821334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef8b0ea598ca779a5b17a6cfc945f5fb7924556f05fb2363b5f9036b0e174ad4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 11:11:27 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Fri, 11 Nov 2022 11:11:27 GMT
ARG VARNISH_VERSION=7.1.2
# Fri, 11 Nov 2022 11:11:27 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Fri, 11 Nov 2022 11:11:27 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Fri, 11 Nov 2022 11:11:27 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Fri, 11 Nov 2022 11:11:27 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 11 Nov 2022 11:11:27 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Fri, 11 Nov 2022 11:11:27 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Fri, 11 Nov 2022 11:11:27 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 11 Nov 2022 11:11:27 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Fri, 11 Nov 2022 11:11:27 GMT
ENV VARNISH_SIZE=100M
# Fri, 11 Nov 2022 11:12:31 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 11 Nov 2022 11:12:31 GMT
WORKDIR /etc/varnish
# Fri, 11 Nov 2022 11:12:31 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 11 Nov 2022 11:12:31 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 11 Nov 2022 11:12:32 GMT
USER varnish
# Fri, 11 Nov 2022 11:12:32 GMT
EXPOSE 80 8443
# Fri, 11 Nov 2022 11:12:32 GMT
CMD []
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc75e4f36dbe8d71a5eaf0e56fba0e90226526c5e3759babf17ba6a3e553ce47`  
		Last Modified: Fri, 11 Nov 2022 11:12:57 GMT  
		Size: 49.1 MB (49102395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6324f8809992cfd331bdcf3e0f499b98535fbf7427ae9168308687cf0567305a`  
		Last Modified: Fri, 11 Nov 2022 11:12:51 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; 386

```console
$ docker pull varnish@sha256:b3f5feb5d221bd9c13b856c10cb0120b95291c7e4f7fdb927fe08ec4ad1e88ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.3 MB (59279274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67b581c96ccf8b2633e4f6c79db5ce762a929d95d479de81e844126a865f8c8d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 02:12:55 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 08 Nov 2022 18:44:36 GMT
ARG VARNISH_VERSION=7.1.2
# Tue, 08 Nov 2022 18:44:37 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Tue, 08 Nov 2022 18:44:38 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 08 Nov 2022 18:44:39 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 08 Nov 2022 18:44:40 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 08 Nov 2022 18:44:41 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 08 Nov 2022 18:44:42 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 08 Nov 2022 18:44:43 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 08 Nov 2022 18:44:44 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Tue, 08 Nov 2022 18:44:45 GMT
ENV VARNISH_SIZE=100M
# Tue, 08 Nov 2022 18:46:00 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Tue, 08 Nov 2022 18:46:00 GMT
WORKDIR /etc/varnish
# Tue, 08 Nov 2022 18:46:02 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 08 Nov 2022 18:46:02 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 08 Nov 2022 18:46:03 GMT
USER varnish
# Tue, 08 Nov 2022 18:46:04 GMT
EXPOSE 80 8443
# Tue, 08 Nov 2022 18:46:05 GMT
CMD []
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b7b64086583adaf8e717a764baa8e1e5518939598e37bfbd3d5d8a10b16099`  
		Last Modified: Tue, 08 Nov 2022 18:48:14 GMT  
		Size: 56.5 MB (56450259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e960ed7e731a3a4de714a5163ea0b5b051db544035426db396aede8d60d4a2`  
		Last Modified: Tue, 08 Nov 2022 18:48:07 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:fd13ff160f58772d17c34ea5366635adea6934f90965f814bbff7809a81e1956
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48891152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14848d3913a9ba32f1c0a797e633fd7c7b24673f71f8b6d95ff4f31c6a8cb674`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:17:20 GMT
ADD file:be31abb0aba89ed5ff9200736a1c46091abc3845d0e332efd5e5c874ef2c99d1 in / 
# Tue, 09 Aug 2022 17:17:21 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:52:54 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 08 Nov 2022 22:32:34 GMT
ARG VARNISH_VERSION=7.1.2
# Tue, 08 Nov 2022 22:32:35 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Tue, 08 Nov 2022 22:32:35 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 08 Nov 2022 22:32:35 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 08 Nov 2022 22:32:35 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 08 Nov 2022 22:32:36 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 08 Nov 2022 22:32:37 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 08 Nov 2022 22:32:37 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 08 Nov 2022 22:32:38 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Tue, 08 Nov 2022 22:32:38 GMT
ENV VARNISH_SIZE=100M
# Tue, 08 Nov 2022 22:34:25 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Tue, 08 Nov 2022 22:34:27 GMT
WORKDIR /etc/varnish
# Tue, 08 Nov 2022 22:34:27 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 08 Nov 2022 22:34:28 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 08 Nov 2022 22:34:28 GMT
USER varnish
# Tue, 08 Nov 2022 22:34:29 GMT
EXPOSE 80 8443
# Tue, 08 Nov 2022 22:34:29 GMT
CMD []
```

-	Layers:
	-	`sha256:deb7065b3304c3a9834f31b8a53e8d6089060e9c6522668abd22f1f4d9f52ca7`  
		Last Modified: Tue, 09 Aug 2022 17:18:45 GMT  
		Size: 2.8 MB (2812989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fa6b482f0aa86974b6985a7ec840d7f1efd96cf825f3b458d93f6957be2dc2`  
		Last Modified: Tue, 08 Nov 2022 22:41:17 GMT  
		Size: 46.1 MB (46077664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d52f90e5fa0cbf3d9c1dcc9b50fba21e6e1c849ed28b7dba4cccc2caea937c`  
		Last Modified: Tue, 08 Nov 2022 22:41:05 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:cd614f6294b6623abcc8e6b95a192e7bbcf1ee7eb7fde1c7fb8b25c5caeaa136
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.3 MB (47345351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39158646bb7f7dd43a83f88c405b6e61369cb1d9ca741da81aa7660e3efe3720`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 10:18:49 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 08 Nov 2022 18:22:21 GMT
ARG VARNISH_VERSION=7.1.2
# Tue, 08 Nov 2022 18:22:22 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Tue, 08 Nov 2022 18:22:22 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 08 Nov 2022 18:22:23 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 08 Nov 2022 18:22:24 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 08 Nov 2022 18:22:24 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 08 Nov 2022 18:22:25 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 08 Nov 2022 18:22:25 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 08 Nov 2022 18:22:26 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Tue, 08 Nov 2022 18:22:26 GMT
ENV VARNISH_SIZE=100M
# Tue, 08 Nov 2022 18:25:11 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Tue, 08 Nov 2022 18:25:17 GMT
WORKDIR /etc/varnish
# Tue, 08 Nov 2022 18:25:18 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 08 Nov 2022 18:25:19 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 08 Nov 2022 18:25:19 GMT
USER varnish
# Tue, 08 Nov 2022 18:25:20 GMT
EXPOSE 80 8443
# Tue, 08 Nov 2022 18:25:21 GMT
CMD []
```

-	Layers:
	-	`sha256:cdf710f5b7ee39c5124c50c753228dc9b8b1c1c0a1a38f1413487548565445c3`  
		Last Modified: Tue, 09 Aug 2022 17:42:56 GMT  
		Size: 2.6 MB (2606087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9702764c9fb92996851b17f3da01efeb6e89bafbae74f375e28b8be5391f2ace`  
		Last Modified: Tue, 08 Nov 2022 18:27:39 GMT  
		Size: 44.7 MB (44738766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e185d30ef72fbdb2cf68aded1268dc798f233bdb4dddb8e273a4c909f52bb5`  
		Last Modified: Tue, 08 Nov 2022 18:27:34 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:stable`

```console
$ docker pull varnish@sha256:b0d247fec393954674a4157f3de84fa53a2ccb7717d0ee38b373422b62549668
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
$ docker pull varnish@sha256:e4cd2e7566f7b0bb6024b2bbc7afbcc0051578eda02a26f23e6eb0f2fb1d8b17
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100654177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a3021a46bbb249a168c045b9b28ed52b3080066ecd5c56949a13f602a883fe5`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:45:19 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 06:47:30 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 09 Feb 2023 06:47:31 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 06:47:31 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 09 Feb 2023 06:47:31 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 06:47:31 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 06:47:31 GMT
CMD []
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80050f63f771eb4efeb5c0520d8f026ffeb09052cc3d2e9ad6a21a0b9e421d9`  
		Last Modified: Thu, 09 Feb 2023 06:48:55 GMT  
		Size: 69.2 MB (69241665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6274344d07d3f36b703541c8cbd5a4af391685ca105a99b7428780321587d14`  
		Last Modified: Thu, 09 Feb 2023 06:48:46 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; arm variant v7

```console
$ docker pull varnish@sha256:0f77cb08adbcd607941b11e583028385baa63d283cc3ec0f6b2588b72963746a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77210486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67eb10f44de604385766a212cdf419e153376019a21700a8fca61efc445f1110`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Sat, 04 Feb 2023 09:59:36 GMT
ADD file:c3cb8f4527fa96e99a4741ecb398113f25f53389c173b74f6c2a5e39a6575c60 in / 
# Sat, 04 Feb 2023 09:59:36 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 21:26:03 GMT
ENV VARNISH_SIZE=100M
# Sat, 04 Feb 2023 21:28:15 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Sat, 04 Feb 2023 21:28:16 GMT
WORKDIR /etc/varnish
# Sat, 04 Feb 2023 21:28:16 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Sat, 04 Feb 2023 21:28:16 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sat, 04 Feb 2023 21:28:16 GMT
EXPOSE 80 8443
# Sat, 04 Feb 2023 21:28:16 GMT
CMD []
```

-	Layers:
	-	`sha256:bd25bcdfbaa165120ee21b6567df395fe7d7b38da3cca0bcecee55a190e04aab`  
		Last Modified: Sat, 04 Feb 2023 10:06:24 GMT  
		Size: 26.6 MB (26559474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333b4a031d92c063bed44bddd31488609edfb71d88110e3809d9651c51d6226f`  
		Last Modified: Sat, 04 Feb 2023 21:30:19 GMT  
		Size: 50.7 MB (50650309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3f7526ff1da106d69172301d1772476cef2a5485c2ad546e1ca910343be780`  
		Last Modified: Sat, 04 Feb 2023 21:30:11 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:c450ad79500ba96cc35dd3c52ad3599334e6b3041428c499f6be27e07f1d22c7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94715178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bcf86c429658bbe854449e54a0595d02f2cd4d0cd0a866950b73caa3b511092`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 08:49:30 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 08:51:12 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 09 Feb 2023 08:51:12 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 08:51:12 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 09 Feb 2023 08:51:12 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 08:51:12 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 08:51:12 GMT
CMD []
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf53fb8b108e21aca2703892f32fa2f2619b742b46646331e3de24ab29d2ff0`  
		Last Modified: Thu, 09 Feb 2023 08:52:40 GMT  
		Size: 64.7 MB (64651966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221a70689e8a24c44e0e2d2a614e95e20e58ad7b87f01b72f52870e353b77c63`  
		Last Modified: Thu, 09 Feb 2023 08:52:33 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; 386

```console
$ docker pull varnish@sha256:f56aa456fae0b77ca66bec4fe85700f8781a3884de98883c8ff959c9dd055f2d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102061249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de466f497ac50aeb90f89b48ee5a85c34f954ccb439cd58cafdc8cb74267e295`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Sat, 04 Feb 2023 07:49:22 GMT
ADD file:82af884aad6a87f5b309a7418aa1df69f92180a39818ae6d77d37d072cb6fecb in / 
# Sat, 04 Feb 2023 07:49:22 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 21:42:34 GMT
ENV VARNISH_SIZE=100M
# Sat, 04 Feb 2023 21:45:00 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Sat, 04 Feb 2023 21:45:00 GMT
WORKDIR /etc/varnish
# Sat, 04 Feb 2023 21:45:02 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Sat, 04 Feb 2023 21:45:02 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sat, 04 Feb 2023 21:45:03 GMT
EXPOSE 80 8443
# Sat, 04 Feb 2023 21:45:04 GMT
CMD []
```

-	Layers:
	-	`sha256:fb99e0a97d653ef9acb2bdac0d1d10a8655b789bd4e8924c4a1c4a2af8adbb4a`  
		Last Modified: Sat, 04 Feb 2023 07:55:04 GMT  
		Size: 32.4 MB (32375772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2e84e91a218f50a680c6e76813b7dc715f8531d7019f32602ffd231bc68c52`  
		Last Modified: Sat, 04 Feb 2023 21:46:29 GMT  
		Size: 69.7 MB (69684776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0caa57957b3cf341e896f98722d6ad32929b1ea6ddd1a3934ed40cdd62d247eb`  
		Last Modified: Sat, 04 Feb 2023 21:46:20 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; ppc64le

```console
$ docker pull varnish@sha256:193cbaeb322e0557f034c425514d885339d6668c4386aa513402721bd9c21133
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.8 MB (99799855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fda082de4c7749b8307345a3b8d4137b5dabdedcabcd421708578b85a9e9a489`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 06:21:49 GMT
ADD file:b09577b8131a90731fdfb00b824a97dc65ccb51d484cb9004382035d64a5741c in / 
# Thu, 09 Feb 2023 06:21:52 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:04:27 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 12:11:06 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 09 Feb 2023 12:11:08 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 12:11:09 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 09 Feb 2023 12:11:09 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 12:11:10 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 12:11:10 GMT
CMD []
```

-	Layers:
	-	`sha256:4ea90e1a094ae86c7950bbec99e7a79b08fae641ad5f3bc3af9081c925894c41`  
		Last Modified: Thu, 09 Feb 2023 06:28:27 GMT  
		Size: 35.3 MB (35289252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d53de417bdc50d62d7fdbeeea8e46800fabd0ed80370a9069c87147b7123ad5`  
		Last Modified: Thu, 09 Feb 2023 12:13:28 GMT  
		Size: 64.5 MB (64509900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622e78faebf5b8024d64bf97cbc1e0a1a2ef6e8ed2fddbb16abfc817471fc463`  
		Last Modified: Thu, 09 Feb 2023 12:13:11 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; s390x

```console
$ docker pull varnish@sha256:df592d2c04da7cb2ee2144d4d971e719e7a60555c989bb86dde0d6c56089a79f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.0 MB (81002185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73636281614290efddc6e2f074b73a8ae88c72ab5f8d5e59d9349b2e0b0203b4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 09 Feb 2023 02:41:45 GMT
ADD file:dc3c16b50baeac5b9644e607c8df9606e9583f8598e3ba34bcdd69c669a5904c in / 
# Thu, 09 Feb 2023 02:41:46 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 04:36:52 GMT
ENV VARNISH_SIZE=100M
# Thu, 09 Feb 2023 04:41:52 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 09 Feb 2023 04:42:02 GMT
WORKDIR /etc/varnish
# Thu, 09 Feb 2023 04:42:02 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 09 Feb 2023 04:42:03 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 09 Feb 2023 04:42:03 GMT
EXPOSE 80 8443
# Thu, 09 Feb 2023 04:42:04 GMT
CMD []
```

-	Layers:
	-	`sha256:c2f78940fdfbfc5ce5d1d3cff3c27a319451aeb3ec12ff2473073516907fbce9`  
		Last Modified: Thu, 09 Feb 2023 02:46:06 GMT  
		Size: 29.6 MB (29647513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745410423134e2a363bf94f19d54352747cc0d7d642545ec7a337ad28c334724`  
		Last Modified: Thu, 09 Feb 2023 04:43:20 GMT  
		Size: 51.4 MB (51353971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e967e8ebb718a1ca31b86298d62b3fdfdcf3fac94d321d34ba0754a9c55395`  
		Last Modified: Thu, 09 Feb 2023 04:43:14 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
