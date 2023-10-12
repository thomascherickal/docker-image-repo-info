<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `varnish`

-	[`varnish:6.0`](#varnish60)
-	[`varnish:6.0.11`](#varnish6011)
-	[`varnish:7.3`](#varnish73)
-	[`varnish:7.3-alpine`](#varnish73-alpine)
-	[`varnish:7.3.0`](#varnish730)
-	[`varnish:7.3.0-alpine`](#varnish730-alpine)
-	[`varnish:7.4`](#varnish74)
-	[`varnish:7.4-alpine`](#varnish74-alpine)
-	[`varnish:7.4.1`](#varnish741)
-	[`varnish:7.4.1-alpine`](#varnish741-alpine)
-	[`varnish:alpine`](#varnishalpine)
-	[`varnish:fresh`](#varnishfresh)
-	[`varnish:fresh-alpine`](#varnishfresh-alpine)
-	[`varnish:latest`](#varnishlatest)
-	[`varnish:old`](#varnishold)
-	[`varnish:old-alpine`](#varnishold-alpine)
-	[`varnish:stable`](#varnishstable)

## `varnish:6.0`

```console
$ docker pull varnish@sha256:fb2e04b1f54164cddf211eebf12b28454c53ca3a9f7cdce988139b686e32746d
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
$ docker pull varnish@sha256:a2fedd4b349bef78954711ebf0c48d29529d9665b24c87be8d68469f7b301601
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.8 MB (95777272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:088201a03c09141b578de5f1a90431a08261d79560690ceec3a8611cd3cb8139`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:32:51 GMT
ENV VARNISH_SIZE=100M
# Wed, 11 Oct 2023 21:34:27 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 11 Oct 2023 21:34:28 GMT
WORKDIR /etc/varnish
# Wed, 11 Oct 2023 21:34:28 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 11 Oct 2023 21:34:28 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 11 Oct 2023 21:34:28 GMT
EXPOSE 80 8443
# Wed, 11 Oct 2023 21:34:28 GMT
CMD []
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f466157a7a5fef1673f33f132f409dc74a64a07cb115ed2c205c6fb160f57db8`  
		Last Modified: Wed, 11 Oct 2023 21:36:01 GMT  
		Size: 64.4 MB (64358708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ce6e3334e93dd03918524df1b07da65b86555a5dd2e0b3a8d1758967710f2b`  
		Last Modified: Wed, 11 Oct 2023 21:35:52 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; arm variant v7

```console
$ docker pull varnish@sha256:31b618463c24e16717213a163e6fdfda57f5ebb66af4f243fb975047a1e5c306
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.8 MB (72779237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1cae40c71c4d7501687eb440e432afdd6a26e012aba587fb1b0dace08c63301`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:42:29 GMT
ADD file:0d1753bfedd7193184780166819d0407867a22d82804c0045274f1f13afecac0 in / 
# Wed, 11 Oct 2023 17:42:29 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:15:25 GMT
ENV VARNISH_SIZE=100M
# Wed, 11 Oct 2023 18:17:06 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 11 Oct 2023 18:17:06 GMT
WORKDIR /etc/varnish
# Wed, 11 Oct 2023 18:17:06 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 11 Oct 2023 18:17:06 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 11 Oct 2023 18:17:06 GMT
EXPOSE 80 8443
# Wed, 11 Oct 2023 18:17:06 GMT
CMD []
```

-	Layers:
	-	`sha256:bb9c59b28e9fb9c31ffdb002ca9a6656677eee093c8093fcbea8818e927df70a`  
		Last Modified: Wed, 11 Oct 2023 17:47:06 GMT  
		Size: 26.6 MB (26579008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49121c62882c0fa09c7201e9a0342332b2b0e9c98b2a44964bf44876393d157e`  
		Last Modified: Wed, 11 Oct 2023 18:18:28 GMT  
		Size: 46.2 MB (46199529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4edd845338656f474cd4df537619e975b66eb14023de26b5fefc3e26b0bbe7`  
		Last Modified: Wed, 11 Oct 2023 18:18:21 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:931582d1753bfcdf601c1c014cd7f76bff9b35086ee2ea9f986c1b36a0a09088
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.9 MB (89876950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e62a2aa115496a1b3f5ba28121d5244d477851e9d4771b51c6fec40210b7c094`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:30:05 GMT
ENV VARNISH_SIZE=100M
# Wed, 11 Oct 2023 22:31:33 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 11 Oct 2023 22:31:34 GMT
WORKDIR /etc/varnish
# Wed, 11 Oct 2023 22:31:34 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 11 Oct 2023 22:31:34 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 11 Oct 2023 22:31:34 GMT
EXPOSE 80 8443
# Wed, 11 Oct 2023 22:31:34 GMT
CMD []
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9307d4506e3c009b9b9dec476e7a7b4a26706727b77cb98af3a2766eacb7993`  
		Last Modified: Wed, 11 Oct 2023 22:32:21 GMT  
		Size: 59.8 MB (59812161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3fd3fac24ecb46472db6ad2cb107ff688bf54d794ec2ab3dc6ce4263e712ae`  
		Last Modified: Wed, 11 Oct 2023 22:32:15 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; 386

```console
$ docker pull varnish@sha256:8f220404a10d593f6c07faddc6d5b32c252eafe3e3e918fa513996b10b532091
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.1 MB (97073360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a12489d0673cd00fd3b59c177e4e6a0772510a4a1f409d06e1394f3bfb07c9a8`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:41:03 GMT
ADD file:ec6d51df021532be6c52d882f60a33d5cce8c3bff039efe8b98e923f2658ba45 in / 
# Wed, 11 Oct 2023 17:41:03 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 08:45:53 GMT
ENV VARNISH_SIZE=100M
# Thu, 12 Oct 2023 08:47:58 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 12 Oct 2023 08:47:59 GMT
WORKDIR /etc/varnish
# Thu, 12 Oct 2023 08:47:59 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 12 Oct 2023 08:47:59 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 12 Oct 2023 08:47:59 GMT
EXPOSE 80 8443
# Thu, 12 Oct 2023 08:47:59 GMT
CMD []
```

-	Layers:
	-	`sha256:f088164df28359c53d5766709e069e084073984ecf4688687b4c7c529a8926a5`  
		Last Modified: Wed, 11 Oct 2023 17:46:21 GMT  
		Size: 32.4 MB (32402649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6699d0944fb8112e17e8f107db82827a2c19e0d6474e5280ca826fb9ebb1785`  
		Last Modified: Thu, 12 Oct 2023 08:49:29 GMT  
		Size: 64.7 MB (64670008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98eb18751f2956df8a3185d1a7bb422b57927cb9a6419bc9c10fd19da1a884d9`  
		Last Modified: Thu, 12 Oct 2023 08:49:16 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; ppc64le

```console
$ docker pull varnish@sha256:dcb527bec6a95f326235868b2224d0adef2a46c5e77911fa97b66f283917bdb1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.6 MB (94589366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01a2cd1f691613607a05c5f1a52e65b5ea0bef282662a03029bcd8ec32a32ad2`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:44:53 GMT
ADD file:96450fb62af4cd68105cbbf612cb5d2f79139cc9416835b6c2fdf40727635939 in / 
# Wed, 11 Oct 2023 17:44:55 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 12:25:06 GMT
ENV VARNISH_SIZE=100M
# Thu, 12 Oct 2023 12:30:37 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 12 Oct 2023 12:30:40 GMT
WORKDIR /etc/varnish
# Thu, 12 Oct 2023 12:30:40 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 12 Oct 2023 12:30:41 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 12 Oct 2023 12:30:41 GMT
EXPOSE 80 8443
# Thu, 12 Oct 2023 12:30:42 GMT
CMD []
```

-	Layers:
	-	`sha256:cde4df93466f96fbb1bbc513d09d354ea1e58d3e619c19fcf9120dbba87405ea`  
		Last Modified: Wed, 11 Oct 2023 17:50:55 GMT  
		Size: 35.3 MB (35293715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970f2ad54c0186fe95658ba1e1a19f61aa59ff8d68e1c7fc1260bacb62521adf`  
		Last Modified: Thu, 12 Oct 2023 12:32:24 GMT  
		Size: 59.3 MB (59294948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a05cb5c5fbcca586645108664334a9d2183959a15e7a36924aa0aaed55e327`  
		Last Modified: Thu, 12 Oct 2023 12:32:09 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; s390x

```console
$ docker pull varnish@sha256:6312c151e13da2a594d0081723ae173f9d125bf486b37e5fe18cfa26283bbc71
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76186973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f0768ac525a10ed3e3ec2fbbece634f0e229fa4c406d5d998369342f29b27c0`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:50:58 GMT
ADD file:0cfc89fea6da8404b2bccfb0c408dde9e7497e8a93304c4ced9e51bd2b3a319a in / 
# Wed, 11 Oct 2023 17:51:00 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 01:13:22 GMT
ENV VARNISH_SIZE=100M
# Thu, 12 Oct 2023 01:14:52 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 12 Oct 2023 01:14:55 GMT
WORKDIR /etc/varnish
# Thu, 12 Oct 2023 01:14:55 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 12 Oct 2023 01:14:55 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 12 Oct 2023 01:14:56 GMT
EXPOSE 80 8443
# Thu, 12 Oct 2023 01:14:56 GMT
CMD []
```

-	Layers:
	-	`sha256:a12df18f4c86c0f825c6b30eb023dc9f30ba0de34f6b97dca708a7247f4f6c49`  
		Last Modified: Wed, 11 Oct 2023 17:57:36 GMT  
		Size: 29.7 MB (29656917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d80cc9733cb32eb8c5432a7e7c81b9a7a14ce628c02ee290d4327994dfd50c`  
		Last Modified: Thu, 12 Oct 2023 01:17:03 GMT  
		Size: 46.5 MB (46529355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c3cc48fdfae886d0a5d91252dc870bd710dbe7770bdcba9a8efb2e621c8d9c`  
		Last Modified: Thu, 12 Oct 2023 01:16:57 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0.11`

```console
$ docker pull varnish@sha256:fb2e04b1f54164cddf211eebf12b28454c53ca3a9f7cdce988139b686e32746d
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
$ docker pull varnish@sha256:a2fedd4b349bef78954711ebf0c48d29529d9665b24c87be8d68469f7b301601
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.8 MB (95777272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:088201a03c09141b578de5f1a90431a08261d79560690ceec3a8611cd3cb8139`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:32:51 GMT
ENV VARNISH_SIZE=100M
# Wed, 11 Oct 2023 21:34:27 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 11 Oct 2023 21:34:28 GMT
WORKDIR /etc/varnish
# Wed, 11 Oct 2023 21:34:28 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 11 Oct 2023 21:34:28 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 11 Oct 2023 21:34:28 GMT
EXPOSE 80 8443
# Wed, 11 Oct 2023 21:34:28 GMT
CMD []
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f466157a7a5fef1673f33f132f409dc74a64a07cb115ed2c205c6fb160f57db8`  
		Last Modified: Wed, 11 Oct 2023 21:36:01 GMT  
		Size: 64.4 MB (64358708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ce6e3334e93dd03918524df1b07da65b86555a5dd2e0b3a8d1758967710f2b`  
		Last Modified: Wed, 11 Oct 2023 21:35:52 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.11` - linux; arm variant v7

```console
$ docker pull varnish@sha256:31b618463c24e16717213a163e6fdfda57f5ebb66af4f243fb975047a1e5c306
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.8 MB (72779237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1cae40c71c4d7501687eb440e432afdd6a26e012aba587fb1b0dace08c63301`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:42:29 GMT
ADD file:0d1753bfedd7193184780166819d0407867a22d82804c0045274f1f13afecac0 in / 
# Wed, 11 Oct 2023 17:42:29 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:15:25 GMT
ENV VARNISH_SIZE=100M
# Wed, 11 Oct 2023 18:17:06 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 11 Oct 2023 18:17:06 GMT
WORKDIR /etc/varnish
# Wed, 11 Oct 2023 18:17:06 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 11 Oct 2023 18:17:06 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 11 Oct 2023 18:17:06 GMT
EXPOSE 80 8443
# Wed, 11 Oct 2023 18:17:06 GMT
CMD []
```

-	Layers:
	-	`sha256:bb9c59b28e9fb9c31ffdb002ca9a6656677eee093c8093fcbea8818e927df70a`  
		Last Modified: Wed, 11 Oct 2023 17:47:06 GMT  
		Size: 26.6 MB (26579008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49121c62882c0fa09c7201e9a0342332b2b0e9c98b2a44964bf44876393d157e`  
		Last Modified: Wed, 11 Oct 2023 18:18:28 GMT  
		Size: 46.2 MB (46199529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4edd845338656f474cd4df537619e975b66eb14023de26b5fefc3e26b0bbe7`  
		Last Modified: Wed, 11 Oct 2023 18:18:21 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.11` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:931582d1753bfcdf601c1c014cd7f76bff9b35086ee2ea9f986c1b36a0a09088
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.9 MB (89876950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e62a2aa115496a1b3f5ba28121d5244d477851e9d4771b51c6fec40210b7c094`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:30:05 GMT
ENV VARNISH_SIZE=100M
# Wed, 11 Oct 2023 22:31:33 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 11 Oct 2023 22:31:34 GMT
WORKDIR /etc/varnish
# Wed, 11 Oct 2023 22:31:34 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 11 Oct 2023 22:31:34 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 11 Oct 2023 22:31:34 GMT
EXPOSE 80 8443
# Wed, 11 Oct 2023 22:31:34 GMT
CMD []
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9307d4506e3c009b9b9dec476e7a7b4a26706727b77cb98af3a2766eacb7993`  
		Last Modified: Wed, 11 Oct 2023 22:32:21 GMT  
		Size: 59.8 MB (59812161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3fd3fac24ecb46472db6ad2cb107ff688bf54d794ec2ab3dc6ce4263e712ae`  
		Last Modified: Wed, 11 Oct 2023 22:32:15 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.11` - linux; 386

```console
$ docker pull varnish@sha256:8f220404a10d593f6c07faddc6d5b32c252eafe3e3e918fa513996b10b532091
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.1 MB (97073360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a12489d0673cd00fd3b59c177e4e6a0772510a4a1f409d06e1394f3bfb07c9a8`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:41:03 GMT
ADD file:ec6d51df021532be6c52d882f60a33d5cce8c3bff039efe8b98e923f2658ba45 in / 
# Wed, 11 Oct 2023 17:41:03 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 08:45:53 GMT
ENV VARNISH_SIZE=100M
# Thu, 12 Oct 2023 08:47:58 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 12 Oct 2023 08:47:59 GMT
WORKDIR /etc/varnish
# Thu, 12 Oct 2023 08:47:59 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 12 Oct 2023 08:47:59 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 12 Oct 2023 08:47:59 GMT
EXPOSE 80 8443
# Thu, 12 Oct 2023 08:47:59 GMT
CMD []
```

-	Layers:
	-	`sha256:f088164df28359c53d5766709e069e084073984ecf4688687b4c7c529a8926a5`  
		Last Modified: Wed, 11 Oct 2023 17:46:21 GMT  
		Size: 32.4 MB (32402649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6699d0944fb8112e17e8f107db82827a2c19e0d6474e5280ca826fb9ebb1785`  
		Last Modified: Thu, 12 Oct 2023 08:49:29 GMT  
		Size: 64.7 MB (64670008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98eb18751f2956df8a3185d1a7bb422b57927cb9a6419bc9c10fd19da1a884d9`  
		Last Modified: Thu, 12 Oct 2023 08:49:16 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.11` - linux; ppc64le

```console
$ docker pull varnish@sha256:dcb527bec6a95f326235868b2224d0adef2a46c5e77911fa97b66f283917bdb1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.6 MB (94589366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01a2cd1f691613607a05c5f1a52e65b5ea0bef282662a03029bcd8ec32a32ad2`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:44:53 GMT
ADD file:96450fb62af4cd68105cbbf612cb5d2f79139cc9416835b6c2fdf40727635939 in / 
# Wed, 11 Oct 2023 17:44:55 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 12:25:06 GMT
ENV VARNISH_SIZE=100M
# Thu, 12 Oct 2023 12:30:37 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 12 Oct 2023 12:30:40 GMT
WORKDIR /etc/varnish
# Thu, 12 Oct 2023 12:30:40 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 12 Oct 2023 12:30:41 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 12 Oct 2023 12:30:41 GMT
EXPOSE 80 8443
# Thu, 12 Oct 2023 12:30:42 GMT
CMD []
```

-	Layers:
	-	`sha256:cde4df93466f96fbb1bbc513d09d354ea1e58d3e619c19fcf9120dbba87405ea`  
		Last Modified: Wed, 11 Oct 2023 17:50:55 GMT  
		Size: 35.3 MB (35293715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970f2ad54c0186fe95658ba1e1a19f61aa59ff8d68e1c7fc1260bacb62521adf`  
		Last Modified: Thu, 12 Oct 2023 12:32:24 GMT  
		Size: 59.3 MB (59294948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a05cb5c5fbcca586645108664334a9d2183959a15e7a36924aa0aaed55e327`  
		Last Modified: Thu, 12 Oct 2023 12:32:09 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.11` - linux; s390x

```console
$ docker pull varnish@sha256:6312c151e13da2a594d0081723ae173f9d125bf486b37e5fe18cfa26283bbc71
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76186973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f0768ac525a10ed3e3ec2fbbece634f0e229fa4c406d5d998369342f29b27c0`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:50:58 GMT
ADD file:0cfc89fea6da8404b2bccfb0c408dde9e7497e8a93304c4ced9e51bd2b3a319a in / 
# Wed, 11 Oct 2023 17:51:00 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 01:13:22 GMT
ENV VARNISH_SIZE=100M
# Thu, 12 Oct 2023 01:14:52 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 12 Oct 2023 01:14:55 GMT
WORKDIR /etc/varnish
# Thu, 12 Oct 2023 01:14:55 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 12 Oct 2023 01:14:55 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 12 Oct 2023 01:14:56 GMT
EXPOSE 80 8443
# Thu, 12 Oct 2023 01:14:56 GMT
CMD []
```

-	Layers:
	-	`sha256:a12df18f4c86c0f825c6b30eb023dc9f30ba0de34f6b97dca708a7247f4f6c49`  
		Last Modified: Wed, 11 Oct 2023 17:57:36 GMT  
		Size: 29.7 MB (29656917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d80cc9733cb32eb8c5432a7e7c81b9a7a14ce628c02ee290d4327994dfd50c`  
		Last Modified: Thu, 12 Oct 2023 01:17:03 GMT  
		Size: 46.5 MB (46529355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c3cc48fdfae886d0a5d91252dc870bd710dbe7770bdcba9a8efb2e621c8d9c`  
		Last Modified: Thu, 12 Oct 2023 01:16:57 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.3`

```console
$ docker pull varnish@sha256:127e17b1c06f1f4cf5d029c6711bcfee9354d75906651bd50ffdf32b79d85aa0
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
$ docker pull varnish@sha256:a472ccc3c27a471ada7e8366395dc79a818e71d630050b0071309d2c471dba72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101925092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2470d3cdd052769b3be290f06eb7865b5bfab4d102d4f8c5889eb5fec29c7b5`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:30:09 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 11 Oct 2023 21:30:10 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 11 Oct 2023 21:30:10 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 11 Oct 2023 21:30:10 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 11 Oct 2023 21:30:10 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 11 Oct 2023 21:30:10 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 11 Oct 2023 21:30:10 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 11 Oct 2023 21:30:10 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 11 Oct 2023 21:30:10 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Wed, 11 Oct 2023 21:30:10 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Wed, 11 Oct 2023 21:30:10 GMT
ENV VARNISH_SIZE=100M
# Wed, 11 Oct 2023 21:32:39 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 11 Oct 2023 21:32:40 GMT
WORKDIR /etc/varnish
# Wed, 11 Oct 2023 21:32:40 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 11 Oct 2023 21:32:40 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 11 Oct 2023 21:32:40 GMT
USER varnish
# Wed, 11 Oct 2023 21:32:40 GMT
EXPOSE 80 8443
# Wed, 11 Oct 2023 21:32:40 GMT
CMD []
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c964cf9eb5e581139a408a0283a55a73a0ac0b387e3bee71059aa21eaaae36`  
		Last Modified: Wed, 11 Oct 2023 21:35:39 GMT  
		Size: 70.5 MB (70506739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a678d3c9d19dd5252a4e5f98e08a7e6a8d6452f8de01f3dc152d30a8d93623`  
		Last Modified: Wed, 11 Oct 2023 21:35:30 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3` - linux; arm variant v7

```console
$ docker pull varnish@sha256:a9d7925fd2833c99dd825f73189e690aa38ff111448711f53330829302b362bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.7 MB (78707317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02d5d5ec333f1684a11cdbabbb53763153cbcde422823880fc9915cae78872bc`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:42:29 GMT
ADD file:0d1753bfedd7193184780166819d0407867a22d82804c0045274f1f13afecac0 in / 
# Wed, 11 Oct 2023 17:42:29 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:12:16 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 11 Oct 2023 18:12:16 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 11 Oct 2023 18:12:16 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 11 Oct 2023 18:12:16 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 11 Oct 2023 18:12:16 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 11 Oct 2023 18:12:16 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 11 Oct 2023 18:12:16 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 11 Oct 2023 18:12:17 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 11 Oct 2023 18:12:17 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Wed, 11 Oct 2023 18:12:17 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Wed, 11 Oct 2023 18:12:17 GMT
ENV VARNISH_SIZE=100M
# Wed, 11 Oct 2023 18:15:16 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 11 Oct 2023 18:15:16 GMT
WORKDIR /etc/varnish
# Wed, 11 Oct 2023 18:15:17 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 11 Oct 2023 18:15:17 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 11 Oct 2023 18:15:17 GMT
USER varnish
# Wed, 11 Oct 2023 18:15:17 GMT
EXPOSE 80 8443
# Wed, 11 Oct 2023 18:15:17 GMT
CMD []
```

-	Layers:
	-	`sha256:bb9c59b28e9fb9c31ffdb002ca9a6656677eee093c8093fcbea8818e927df70a`  
		Last Modified: Wed, 11 Oct 2023 17:47:06 GMT  
		Size: 26.6 MB (26579008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38680172be1c560e622889d04d9c977f9d93f880d53d1e3d2f84f70ef22b3a64`  
		Last Modified: Wed, 11 Oct 2023 18:18:07 GMT  
		Size: 52.1 MB (52127820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22797eea0f7d1b6cf952632b0be79cac85a2fb2ffa9e162de7ad6efe3026ead6`  
		Last Modified: Wed, 11 Oct 2023 18:18:00 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:e8ade371f73b19375bfd39a503bf3fec6b9e3ba7a9bafc5c3ba88ffeb9f27797
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.7 MB (95748930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3603bd166369d9986732f8f2a43d559412758d24ee0ac9ecd035f46ef49585d0`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:27:25 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 11 Oct 2023 22:27:25 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 11 Oct 2023 22:27:25 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 11 Oct 2023 22:27:25 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 11 Oct 2023 22:27:25 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 11 Oct 2023 22:27:26 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 11 Oct 2023 22:27:26 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 11 Oct 2023 22:27:26 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 11 Oct 2023 22:27:26 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Wed, 11 Oct 2023 22:27:26 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Wed, 11 Oct 2023 22:27:26 GMT
ENV VARNISH_SIZE=100M
# Wed, 11 Oct 2023 22:29:57 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 11 Oct 2023 22:29:57 GMT
WORKDIR /etc/varnish
# Wed, 11 Oct 2023 22:29:57 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 11 Oct 2023 22:29:57 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 11 Oct 2023 22:29:58 GMT
USER varnish
# Wed, 11 Oct 2023 22:29:58 GMT
EXPOSE 80 8443
# Wed, 11 Oct 2023 22:29:58 GMT
CMD []
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a10b543b10fa7fe9ead7538159ed2a4a3f37453153e60f65860b28bf2b4636c`  
		Last Modified: Wed, 11 Oct 2023 22:32:03 GMT  
		Size: 65.7 MB (65684356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e9d1d8ab82d707c25944e2f98cc9a834f8688d17efa7d0e7223762c92326e6`  
		Last Modified: Wed, 11 Oct 2023 22:31:56 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3` - linux; 386

```console
$ docker pull varnish@sha256:cf5384fe85789a6ec705bfd6f37bb749b01d363bad340ce22cbdd9b7f474f5f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.2 MB (103168532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ef8f5b869005d0b5d34f2bb62212faef600ff5004337126ae91e3df8b379da1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:41:03 GMT
ADD file:ec6d51df021532be6c52d882f60a33d5cce8c3bff039efe8b98e923f2658ba45 in / 
# Wed, 11 Oct 2023 17:41:03 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 08:42:14 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Thu, 12 Oct 2023 08:42:14 GMT
ARG VARNISH_VERSION=7.3.0
# Thu, 12 Oct 2023 08:42:14 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Thu, 12 Oct 2023 08:42:14 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 12 Oct 2023 08:42:14 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 12 Oct 2023 08:42:14 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 12 Oct 2023 08:42:15 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Thu, 12 Oct 2023 08:42:15 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Thu, 12 Oct 2023 08:42:15 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 12 Oct 2023 08:42:15 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Thu, 12 Oct 2023 08:42:15 GMT
ENV VARNISH_SIZE=100M
# Thu, 12 Oct 2023 08:45:37 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 12 Oct 2023 08:45:37 GMT
WORKDIR /etc/varnish
# Thu, 12 Oct 2023 08:45:38 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 12 Oct 2023 08:45:38 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 12 Oct 2023 08:45:38 GMT
USER varnish
# Thu, 12 Oct 2023 08:45:38 GMT
EXPOSE 80 8443
# Thu, 12 Oct 2023 08:45:38 GMT
CMD []
```

-	Layers:
	-	`sha256:f088164df28359c53d5766709e069e084073984ecf4688687b4c7c529a8926a5`  
		Last Modified: Wed, 11 Oct 2023 17:46:21 GMT  
		Size: 32.4 MB (32402649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7276ed813d357be91f70a38731c43be595eea25c4c272cf07f899866ffef3133`  
		Last Modified: Thu, 12 Oct 2023 08:49:04 GMT  
		Size: 70.8 MB (70765390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5e53d3521a45c593fa0ce54a8ba6c98748e7adf2ceda330ab6c1a54594f4d56`  
		Last Modified: Thu, 12 Oct 2023 08:48:51 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3` - linux; ppc64le

```console
$ docker pull varnish@sha256:1dfdb622e87f19c7b5d56aa688bf9c954001b5880a9adf745686f09c0c810f49
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.8 MB (100847499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fffc62d9a1870537e7026dec2307845cfa49a5b6a5a048770f7e6828fd747efe`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:44:53 GMT
ADD file:96450fb62af4cd68105cbbf612cb5d2f79139cc9416835b6c2fdf40727635939 in / 
# Wed, 11 Oct 2023 17:44:55 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 12:19:39 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Thu, 12 Oct 2023 12:19:39 GMT
ARG VARNISH_VERSION=7.3.0
# Thu, 12 Oct 2023 12:19:40 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Thu, 12 Oct 2023 12:19:40 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 12 Oct 2023 12:19:40 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 12 Oct 2023 12:19:41 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 12 Oct 2023 12:19:41 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Thu, 12 Oct 2023 12:19:42 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Thu, 12 Oct 2023 12:19:43 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 12 Oct 2023 12:19:43 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Thu, 12 Oct 2023 12:19:43 GMT
ENV VARNISH_SIZE=100M
# Thu, 12 Oct 2023 12:24:47 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 12 Oct 2023 12:24:49 GMT
WORKDIR /etc/varnish
# Thu, 12 Oct 2023 12:24:50 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 12 Oct 2023 12:24:50 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 12 Oct 2023 12:24:50 GMT
USER varnish
# Thu, 12 Oct 2023 12:24:50 GMT
EXPOSE 80 8443
# Thu, 12 Oct 2023 12:24:51 GMT
CMD []
```

-	Layers:
	-	`sha256:cde4df93466f96fbb1bbc513d09d354ea1e58d3e619c19fcf9120dbba87405ea`  
		Last Modified: Wed, 11 Oct 2023 17:50:55 GMT  
		Size: 35.3 MB (35293715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f55666fce1391d828fed4ccaa48b5dfe237758aab33c149d33d9d3c843c08a`  
		Last Modified: Thu, 12 Oct 2023 12:31:56 GMT  
		Size: 65.6 MB (65553292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ace75fc704ec4e7022d88d22c2d18dc2130858cc6939340483e46c3adca952`  
		Last Modified: Thu, 12 Oct 2023 12:31:40 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3` - linux; s390x

```console
$ docker pull varnish@sha256:79828902a6814eedb26de74d04e0584b230792099854ce12010480292b1a1289
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.3 MB (82301300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ecbfad0f4fbd761fe1f432160333f1b520d1128cde705f2162200f8d47a63bb`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:50:58 GMT
ADD file:0cfc89fea6da8404b2bccfb0c408dde9e7497e8a93304c4ced9e51bd2b3a319a in / 
# Wed, 11 Oct 2023 17:51:00 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 01:07:22 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Thu, 12 Oct 2023 01:07:22 GMT
ARG VARNISH_VERSION=7.3.0
# Thu, 12 Oct 2023 01:07:22 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Thu, 12 Oct 2023 01:07:22 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 12 Oct 2023 01:07:23 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 12 Oct 2023 01:07:23 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 12 Oct 2023 01:07:23 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Thu, 12 Oct 2023 01:07:23 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Thu, 12 Oct 2023 01:07:24 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 12 Oct 2023 01:07:24 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Thu, 12 Oct 2023 01:07:24 GMT
ENV VARNISH_SIZE=100M
# Thu, 12 Oct 2023 01:12:57 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 12 Oct 2023 01:13:00 GMT
WORKDIR /etc/varnish
# Thu, 12 Oct 2023 01:13:00 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 12 Oct 2023 01:13:00 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 12 Oct 2023 01:13:00 GMT
USER varnish
# Thu, 12 Oct 2023 01:13:01 GMT
EXPOSE 80 8443
# Thu, 12 Oct 2023 01:13:01 GMT
CMD []
```

-	Layers:
	-	`sha256:a12df18f4c86c0f825c6b30eb023dc9f30ba0de34f6b97dca708a7247f4f6c49`  
		Last Modified: Wed, 11 Oct 2023 17:57:36 GMT  
		Size: 29.7 MB (29656917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bcbf52c84564aa12a68365a8ebf7a38a9a32fcd14d02b393dca8b9cba346789`  
		Last Modified: Thu, 12 Oct 2023 01:16:19 GMT  
		Size: 52.6 MB (52643890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6b13ce2c8b747fb0a75dc838a5b709fa75c3ae125301058f70da5e25c7ba79`  
		Last Modified: Thu, 12 Oct 2023 01:16:11 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.3-alpine`

```console
$ docker pull varnish@sha256:1eaaf02632201e9eb10980f58574e4d5b9bce3a96f4f146313e50d92901ae5de
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
$ docker pull varnish@sha256:c50109176635d4d06d1e3e8e2d6935d30a999947a87a9915adfc38911c3edbf0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.4 MB (59353279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6814db3789c866db3caba06dcbf3a5af9894ab56e19d8e605215f65f9f63d01`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:20:37 GMT
ADD file:4faae297b6caba92e1791a5ff667be0fcb4de6a4de2df155395957ef9d8ad5e5 in / 
# Mon, 07 Aug 2023 19:20:37 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:07:42 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 09 Aug 2023 04:07:43 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 09 Aug 2023 04:07:43 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 09 Aug 2023 04:07:43 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 09 Aug 2023 04:07:43 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 09 Aug 2023 04:07:43 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 09 Aug 2023 04:07:43 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 09 Aug 2023 04:07:43 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 09 Aug 2023 04:07:43 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Wed, 09 Aug 2023 04:07:43 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Wed, 09 Aug 2023 04:07:43 GMT
ENV VARNISH_SIZE=100M
# Wed, 09 Aug 2023 04:09:00 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Wed, 09 Aug 2023 04:09:01 GMT
WORKDIR /etc/varnish
# Wed, 09 Aug 2023 04:09:01 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 09 Aug 2023 04:09:01 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 09 Aug 2023 04:09:01 GMT
USER varnish
# Wed, 09 Aug 2023 04:09:01 GMT
EXPOSE 80 8443
# Wed, 09 Aug 2023 04:09:01 GMT
CMD []
```

-	Layers:
	-	`sha256:3695f6c099b80e503148dbb435d044c35147f81d34b9d6fbb27b3dcf1fd7ecaf`  
		Last Modified: Mon, 07 Aug 2023 19:21:27 GMT  
		Size: 2.8 MB (2826006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a571445311e41e13f2fc1c6ace8610ded14d6ac0c9a00d88f8fc8907d48e2f`  
		Last Modified: Wed, 09 Aug 2023 04:10:57 GMT  
		Size: 56.5 MB (56526777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f0487466108411358ef19a0fa4e224b5368812219ee7a97f6fca2b9c34e188`  
		Last Modified: Wed, 09 Aug 2023 04:10:50 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:a9066203838a2bbf6acd2a4af3dc33997546bf8e67c2502c6185b3e9d983cad7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45110187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e147f405a969edfd9f1c37b4f1a4429593d5975f3c68e98d04bc95c209c112be`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:57:37 GMT
ADD file:842dfa6e14e0537b53781830cfb26da9fa7a63229a7a1decc0fe08d8c000b5a9 in / 
# Mon, 07 Aug 2023 19:57:37 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 21:52:52 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Tue, 08 Aug 2023 21:52:52 GMT
ARG VARNISH_VERSION=7.3.0
# Tue, 08 Aug 2023 21:52:53 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Tue, 08 Aug 2023 21:52:53 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 08 Aug 2023 21:52:54 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 08 Aug 2023 21:52:54 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Tue, 08 Aug 2023 21:52:54 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Tue, 08 Aug 2023 21:52:54 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Tue, 08 Aug 2023 21:52:54 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 08 Aug 2023 21:52:55 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Tue, 08 Aug 2023 21:52:55 GMT
ENV VARNISH_SIZE=100M
# Tue, 08 Aug 2023 21:54:47 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Tue, 08 Aug 2023 21:54:47 GMT
WORKDIR /etc/varnish
# Tue, 08 Aug 2023 21:54:47 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 08 Aug 2023 21:54:47 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 08 Aug 2023 21:54:47 GMT
USER varnish
# Tue, 08 Aug 2023 21:54:47 GMT
EXPOSE 80 8443
# Tue, 08 Aug 2023 21:54:47 GMT
CMD []
```

-	Layers:
	-	`sha256:c25753df0ee4b6d3db1dacebcfb1839260ed067556f1f3ff52ddb574cab51045`  
		Last Modified: Mon, 07 Aug 2023 19:58:28 GMT  
		Size: 2.4 MB (2436761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3835c5b95f60e45f72f9756939da73ac2e053ce0e8b25927e9c38eafaa28134d`  
		Last Modified: Tue, 08 Aug 2023 21:57:08 GMT  
		Size: 42.7 MB (42672929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d6e8e8160593ed0c9c95f9057b778ef9a351adb3eaace602c4d2313dbb2d80`  
		Last Modified: Tue, 08 Aug 2023 21:57:00 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:fa2793323936a2a39bc749fe8c9f4d57ed1f5cacfc7bebd45acab4714d719ac6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52090034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73f5f31a9b25c2236a27ca4ea7326c16321adb4109342c0f4b66cb18945fc936`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:39:29 GMT
ADD file:21f240e1e33b25dacee7291cdd8c7750995aa0f460d13496a08c4a2dd92323aa in / 
# Mon, 07 Aug 2023 19:39:29 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:27:59 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 09 Aug 2023 04:27:59 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 09 Aug 2023 04:27:59 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 09 Aug 2023 04:28:00 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 09 Aug 2023 04:28:00 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 09 Aug 2023 04:28:00 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 09 Aug 2023 04:28:00 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 09 Aug 2023 04:28:00 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 09 Aug 2023 04:28:00 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Wed, 09 Aug 2023 04:28:00 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Wed, 09 Aug 2023 04:28:00 GMT
ENV VARNISH_SIZE=100M
# Wed, 09 Aug 2023 04:29:12 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Wed, 09 Aug 2023 04:29:13 GMT
WORKDIR /etc/varnish
# Wed, 09 Aug 2023 04:29:13 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 09 Aug 2023 04:29:13 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 09 Aug 2023 04:29:13 GMT
USER varnish
# Wed, 09 Aug 2023 04:29:13 GMT
EXPOSE 80 8443
# Wed, 09 Aug 2023 04:29:13 GMT
CMD []
```

-	Layers:
	-	`sha256:ad3fa0ea069c04e4ee9be58cf0ae9e1a8a56f649b96a96298203b055e8c903ff`  
		Last Modified: Mon, 07 Aug 2023 19:40:16 GMT  
		Size: 2.7 MB (2720868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af416d837d369577895656da730e7b9045ced484cb509a3c8d24ea5651f2b72b`  
		Last Modified: Wed, 09 Aug 2023 04:30:54 GMT  
		Size: 49.4 MB (49368670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72ad8cfaa77fff8808621330b797c9dcd268d87ee399f1cadc48654257351c9`  
		Last Modified: Wed, 09 Aug 2023 04:30:49 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3-alpine` - linux; 386

```console
$ docker pull varnish@sha256:40db9d7b920acf3c24a1f0fc818151592d3d617cd98e20b08149fc9526fc24c1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59534324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7db33e169f8fc0973f7d7ebf8d7a395cf221ac4eb15d75050d00bbf746d39e28`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:38:38 GMT
ADD file:2d8ac62dd229ef26536f5a9af9e61df30ea68d609fa969786dfd531aea18cf3c in / 
# Mon, 07 Aug 2023 19:38:38 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 22:26:01 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Tue, 08 Aug 2023 22:26:01 GMT
ARG VARNISH_VERSION=7.3.0
# Tue, 08 Aug 2023 22:26:01 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Tue, 08 Aug 2023 22:26:01 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 08 Aug 2023 22:26:01 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 08 Aug 2023 22:26:01 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Tue, 08 Aug 2023 22:26:01 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Tue, 08 Aug 2023 22:26:02 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Tue, 08 Aug 2023 22:26:02 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 08 Aug 2023 22:26:02 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Tue, 08 Aug 2023 22:26:02 GMT
ENV VARNISH_SIZE=100M
# Tue, 08 Aug 2023 22:28:20 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Tue, 08 Aug 2023 22:28:21 GMT
WORKDIR /etc/varnish
# Tue, 08 Aug 2023 22:28:21 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 08 Aug 2023 22:28:21 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 08 Aug 2023 22:28:21 GMT
USER varnish
# Tue, 08 Aug 2023 22:28:21 GMT
EXPOSE 80 8443
# Tue, 08 Aug 2023 22:28:22 GMT
CMD []
```

-	Layers:
	-	`sha256:add53095769493cde9110fd91f113357e53b9e0d94abf216b811fcf00107674e`  
		Last Modified: Mon, 07 Aug 2023 19:39:29 GMT  
		Size: 2.8 MB (2832316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f647a86d2fc80d9f872ddaf183a99650a85e6bb6db7ab28df1aa47f8c766c37a`  
		Last Modified: Tue, 08 Aug 2023 22:30:58 GMT  
		Size: 56.7 MB (56701511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4a6dc8cb05579dc1a1b1fcb6f15a0661ae9a7feaf8ba4eb6397236e86e4143`  
		Last Modified: Tue, 08 Aug 2023 22:30:48 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:c3a57b142209c5534422dc949c7c67a1ec15ef65f53837b3ecdce1507c22ad17
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49132355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78138cefb19943eea37fdcc772c9f4065c5177abf063d6fcb02c473414a5e3c4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 20:16:50 GMT
ADD file:f730d2cd05a420ffd38548ae1611345fc40a7db59dea5ff41328caa60ee42608 in / 
# Mon, 07 Aug 2023 20:16:51 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:50:57 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Tue, 08 Aug 2023 23:50:58 GMT
ARG VARNISH_VERSION=7.3.0
# Tue, 08 Aug 2023 23:50:58 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Tue, 08 Aug 2023 23:50:59 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 08 Aug 2023 23:50:59 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 08 Aug 2023 23:51:00 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Tue, 08 Aug 2023 23:51:00 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Tue, 08 Aug 2023 23:51:01 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Tue, 08 Aug 2023 23:51:01 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 08 Aug 2023 23:51:02 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Tue, 08 Aug 2023 23:51:02 GMT
ENV VARNISH_SIZE=100M
# Tue, 08 Aug 2023 23:53:25 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Tue, 08 Aug 2023 23:53:28 GMT
WORKDIR /etc/varnish
# Tue, 08 Aug 2023 23:53:28 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 08 Aug 2023 23:53:28 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 08 Aug 2023 23:53:28 GMT
USER varnish
# Tue, 08 Aug 2023 23:53:29 GMT
EXPOSE 80 8443
# Tue, 08 Aug 2023 23:53:29 GMT
CMD []
```

-	Layers:
	-	`sha256:f1ecf55aa97fb0011a1c90ffc58e5cb218908bc85a13afe003aea5a46e045ac8`  
		Last Modified: Mon, 07 Aug 2023 20:18:07 GMT  
		Size: 2.8 MB (2812358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e313b1b6994e0de7da0d5b504d453dd6890fafeb0e8debf9808e953fcfc3e1d1`  
		Last Modified: Tue, 08 Aug 2023 23:56:42 GMT  
		Size: 46.3 MB (46319501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f91dcda5c6dfcb572578877b768d18db70e587fc1cc7ce78429376e9546b94`  
		Last Modified: Tue, 08 Aug 2023 23:56:31 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:4d0ba154b6574f740056123e5f8384b43d90feab3dd12fb2bc6d4eca68a6bcd0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47593252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00fb757c92f0c2efeaa1eb32bcafb1400510fc0fb7ff5c160bd2714a1325cff4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:42:16 GMT
ADD file:db6cafb0897c5e32510edd0166d1e1b23001bef271dad57e4157d560bd09dd93 in / 
# Mon, 07 Aug 2023 19:42:16 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:19:26 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 09 Aug 2023 04:19:27 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 09 Aug 2023 04:19:27 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 09 Aug 2023 04:19:28 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 09 Aug 2023 04:19:29 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 09 Aug 2023 04:19:30 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 09 Aug 2023 04:19:30 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 09 Aug 2023 04:19:31 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 09 Aug 2023 04:19:32 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Wed, 09 Aug 2023 04:19:33 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Wed, 09 Aug 2023 04:19:34 GMT
ENV VARNISH_SIZE=100M
# Wed, 09 Aug 2023 04:21:51 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Wed, 09 Aug 2023 04:22:01 GMT
WORKDIR /etc/varnish
# Wed, 09 Aug 2023 04:22:01 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 09 Aug 2023 04:22:02 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 09 Aug 2023 04:22:03 GMT
USER varnish
# Wed, 09 Aug 2023 04:22:03 GMT
EXPOSE 80 8443
# Wed, 09 Aug 2023 04:22:04 GMT
CMD []
```

-	Layers:
	-	`sha256:ec103030fda7a896185e8eb8a4f00b7f611725434956faa395cf74a993a2742e`  
		Last Modified: Mon, 07 Aug 2023 19:43:01 GMT  
		Size: 2.6 MB (2609002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161846c9c73015426cc80840fbb38cd2016810411f252eb724f4fee1ea84cfbc`  
		Last Modified: Wed, 09 Aug 2023 04:25:34 GMT  
		Size: 45.0 MB (44983753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893cc747d7f6b07b13980f3ceffbd432e9f4f78e9025f02e37ce6eb64e576b48`  
		Last Modified: Wed, 09 Aug 2023 04:25:28 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.3.0`

```console
$ docker pull varnish@sha256:127e17b1c06f1f4cf5d029c6711bcfee9354d75906651bd50ffdf32b79d85aa0
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
$ docker pull varnish@sha256:a472ccc3c27a471ada7e8366395dc79a818e71d630050b0071309d2c471dba72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101925092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2470d3cdd052769b3be290f06eb7865b5bfab4d102d4f8c5889eb5fec29c7b5`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:30:09 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 11 Oct 2023 21:30:10 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 11 Oct 2023 21:30:10 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 11 Oct 2023 21:30:10 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 11 Oct 2023 21:30:10 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 11 Oct 2023 21:30:10 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 11 Oct 2023 21:30:10 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 11 Oct 2023 21:30:10 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 11 Oct 2023 21:30:10 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Wed, 11 Oct 2023 21:30:10 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Wed, 11 Oct 2023 21:30:10 GMT
ENV VARNISH_SIZE=100M
# Wed, 11 Oct 2023 21:32:39 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 11 Oct 2023 21:32:40 GMT
WORKDIR /etc/varnish
# Wed, 11 Oct 2023 21:32:40 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 11 Oct 2023 21:32:40 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 11 Oct 2023 21:32:40 GMT
USER varnish
# Wed, 11 Oct 2023 21:32:40 GMT
EXPOSE 80 8443
# Wed, 11 Oct 2023 21:32:40 GMT
CMD []
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c964cf9eb5e581139a408a0283a55a73a0ac0b387e3bee71059aa21eaaae36`  
		Last Modified: Wed, 11 Oct 2023 21:35:39 GMT  
		Size: 70.5 MB (70506739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a678d3c9d19dd5252a4e5f98e08a7e6a8d6452f8de01f3dc152d30a8d93623`  
		Last Modified: Wed, 11 Oct 2023 21:35:30 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3.0` - linux; arm variant v7

```console
$ docker pull varnish@sha256:a9d7925fd2833c99dd825f73189e690aa38ff111448711f53330829302b362bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.7 MB (78707317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02d5d5ec333f1684a11cdbabbb53763153cbcde422823880fc9915cae78872bc`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:42:29 GMT
ADD file:0d1753bfedd7193184780166819d0407867a22d82804c0045274f1f13afecac0 in / 
# Wed, 11 Oct 2023 17:42:29 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:12:16 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 11 Oct 2023 18:12:16 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 11 Oct 2023 18:12:16 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 11 Oct 2023 18:12:16 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 11 Oct 2023 18:12:16 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 11 Oct 2023 18:12:16 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 11 Oct 2023 18:12:16 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 11 Oct 2023 18:12:17 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 11 Oct 2023 18:12:17 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Wed, 11 Oct 2023 18:12:17 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Wed, 11 Oct 2023 18:12:17 GMT
ENV VARNISH_SIZE=100M
# Wed, 11 Oct 2023 18:15:16 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 11 Oct 2023 18:15:16 GMT
WORKDIR /etc/varnish
# Wed, 11 Oct 2023 18:15:17 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 11 Oct 2023 18:15:17 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 11 Oct 2023 18:15:17 GMT
USER varnish
# Wed, 11 Oct 2023 18:15:17 GMT
EXPOSE 80 8443
# Wed, 11 Oct 2023 18:15:17 GMT
CMD []
```

-	Layers:
	-	`sha256:bb9c59b28e9fb9c31ffdb002ca9a6656677eee093c8093fcbea8818e927df70a`  
		Last Modified: Wed, 11 Oct 2023 17:47:06 GMT  
		Size: 26.6 MB (26579008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38680172be1c560e622889d04d9c977f9d93f880d53d1e3d2f84f70ef22b3a64`  
		Last Modified: Wed, 11 Oct 2023 18:18:07 GMT  
		Size: 52.1 MB (52127820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22797eea0f7d1b6cf952632b0be79cac85a2fb2ffa9e162de7ad6efe3026ead6`  
		Last Modified: Wed, 11 Oct 2023 18:18:00 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3.0` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:e8ade371f73b19375bfd39a503bf3fec6b9e3ba7a9bafc5c3ba88ffeb9f27797
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.7 MB (95748930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3603bd166369d9986732f8f2a43d559412758d24ee0ac9ecd035f46ef49585d0`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:27:25 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 11 Oct 2023 22:27:25 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 11 Oct 2023 22:27:25 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 11 Oct 2023 22:27:25 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 11 Oct 2023 22:27:25 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 11 Oct 2023 22:27:26 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 11 Oct 2023 22:27:26 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 11 Oct 2023 22:27:26 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 11 Oct 2023 22:27:26 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Wed, 11 Oct 2023 22:27:26 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Wed, 11 Oct 2023 22:27:26 GMT
ENV VARNISH_SIZE=100M
# Wed, 11 Oct 2023 22:29:57 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 11 Oct 2023 22:29:57 GMT
WORKDIR /etc/varnish
# Wed, 11 Oct 2023 22:29:57 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 11 Oct 2023 22:29:57 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 11 Oct 2023 22:29:58 GMT
USER varnish
# Wed, 11 Oct 2023 22:29:58 GMT
EXPOSE 80 8443
# Wed, 11 Oct 2023 22:29:58 GMT
CMD []
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a10b543b10fa7fe9ead7538159ed2a4a3f37453153e60f65860b28bf2b4636c`  
		Last Modified: Wed, 11 Oct 2023 22:32:03 GMT  
		Size: 65.7 MB (65684356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e9d1d8ab82d707c25944e2f98cc9a834f8688d17efa7d0e7223762c92326e6`  
		Last Modified: Wed, 11 Oct 2023 22:31:56 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3.0` - linux; 386

```console
$ docker pull varnish@sha256:cf5384fe85789a6ec705bfd6f37bb749b01d363bad340ce22cbdd9b7f474f5f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.2 MB (103168532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ef8f5b869005d0b5d34f2bb62212faef600ff5004337126ae91e3df8b379da1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:41:03 GMT
ADD file:ec6d51df021532be6c52d882f60a33d5cce8c3bff039efe8b98e923f2658ba45 in / 
# Wed, 11 Oct 2023 17:41:03 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 08:42:14 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Thu, 12 Oct 2023 08:42:14 GMT
ARG VARNISH_VERSION=7.3.0
# Thu, 12 Oct 2023 08:42:14 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Thu, 12 Oct 2023 08:42:14 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 12 Oct 2023 08:42:14 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 12 Oct 2023 08:42:14 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 12 Oct 2023 08:42:15 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Thu, 12 Oct 2023 08:42:15 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Thu, 12 Oct 2023 08:42:15 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 12 Oct 2023 08:42:15 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Thu, 12 Oct 2023 08:42:15 GMT
ENV VARNISH_SIZE=100M
# Thu, 12 Oct 2023 08:45:37 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 12 Oct 2023 08:45:37 GMT
WORKDIR /etc/varnish
# Thu, 12 Oct 2023 08:45:38 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 12 Oct 2023 08:45:38 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 12 Oct 2023 08:45:38 GMT
USER varnish
# Thu, 12 Oct 2023 08:45:38 GMT
EXPOSE 80 8443
# Thu, 12 Oct 2023 08:45:38 GMT
CMD []
```

-	Layers:
	-	`sha256:f088164df28359c53d5766709e069e084073984ecf4688687b4c7c529a8926a5`  
		Last Modified: Wed, 11 Oct 2023 17:46:21 GMT  
		Size: 32.4 MB (32402649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7276ed813d357be91f70a38731c43be595eea25c4c272cf07f899866ffef3133`  
		Last Modified: Thu, 12 Oct 2023 08:49:04 GMT  
		Size: 70.8 MB (70765390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5e53d3521a45c593fa0ce54a8ba6c98748e7adf2ceda330ab6c1a54594f4d56`  
		Last Modified: Thu, 12 Oct 2023 08:48:51 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3.0` - linux; ppc64le

```console
$ docker pull varnish@sha256:1dfdb622e87f19c7b5d56aa688bf9c954001b5880a9adf745686f09c0c810f49
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.8 MB (100847499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fffc62d9a1870537e7026dec2307845cfa49a5b6a5a048770f7e6828fd747efe`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:44:53 GMT
ADD file:96450fb62af4cd68105cbbf612cb5d2f79139cc9416835b6c2fdf40727635939 in / 
# Wed, 11 Oct 2023 17:44:55 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 12:19:39 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Thu, 12 Oct 2023 12:19:39 GMT
ARG VARNISH_VERSION=7.3.0
# Thu, 12 Oct 2023 12:19:40 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Thu, 12 Oct 2023 12:19:40 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 12 Oct 2023 12:19:40 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 12 Oct 2023 12:19:41 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 12 Oct 2023 12:19:41 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Thu, 12 Oct 2023 12:19:42 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Thu, 12 Oct 2023 12:19:43 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 12 Oct 2023 12:19:43 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Thu, 12 Oct 2023 12:19:43 GMT
ENV VARNISH_SIZE=100M
# Thu, 12 Oct 2023 12:24:47 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 12 Oct 2023 12:24:49 GMT
WORKDIR /etc/varnish
# Thu, 12 Oct 2023 12:24:50 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 12 Oct 2023 12:24:50 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 12 Oct 2023 12:24:50 GMT
USER varnish
# Thu, 12 Oct 2023 12:24:50 GMT
EXPOSE 80 8443
# Thu, 12 Oct 2023 12:24:51 GMT
CMD []
```

-	Layers:
	-	`sha256:cde4df93466f96fbb1bbc513d09d354ea1e58d3e619c19fcf9120dbba87405ea`  
		Last Modified: Wed, 11 Oct 2023 17:50:55 GMT  
		Size: 35.3 MB (35293715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f55666fce1391d828fed4ccaa48b5dfe237758aab33c149d33d9d3c843c08a`  
		Last Modified: Thu, 12 Oct 2023 12:31:56 GMT  
		Size: 65.6 MB (65553292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ace75fc704ec4e7022d88d22c2d18dc2130858cc6939340483e46c3adca952`  
		Last Modified: Thu, 12 Oct 2023 12:31:40 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3.0` - linux; s390x

```console
$ docker pull varnish@sha256:79828902a6814eedb26de74d04e0584b230792099854ce12010480292b1a1289
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.3 MB (82301300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ecbfad0f4fbd761fe1f432160333f1b520d1128cde705f2162200f8d47a63bb`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:50:58 GMT
ADD file:0cfc89fea6da8404b2bccfb0c408dde9e7497e8a93304c4ced9e51bd2b3a319a in / 
# Wed, 11 Oct 2023 17:51:00 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 01:07:22 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Thu, 12 Oct 2023 01:07:22 GMT
ARG VARNISH_VERSION=7.3.0
# Thu, 12 Oct 2023 01:07:22 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Thu, 12 Oct 2023 01:07:22 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 12 Oct 2023 01:07:23 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 12 Oct 2023 01:07:23 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 12 Oct 2023 01:07:23 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Thu, 12 Oct 2023 01:07:23 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Thu, 12 Oct 2023 01:07:24 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 12 Oct 2023 01:07:24 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Thu, 12 Oct 2023 01:07:24 GMT
ENV VARNISH_SIZE=100M
# Thu, 12 Oct 2023 01:12:57 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 12 Oct 2023 01:13:00 GMT
WORKDIR /etc/varnish
# Thu, 12 Oct 2023 01:13:00 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 12 Oct 2023 01:13:00 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 12 Oct 2023 01:13:00 GMT
USER varnish
# Thu, 12 Oct 2023 01:13:01 GMT
EXPOSE 80 8443
# Thu, 12 Oct 2023 01:13:01 GMT
CMD []
```

-	Layers:
	-	`sha256:a12df18f4c86c0f825c6b30eb023dc9f30ba0de34f6b97dca708a7247f4f6c49`  
		Last Modified: Wed, 11 Oct 2023 17:57:36 GMT  
		Size: 29.7 MB (29656917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bcbf52c84564aa12a68365a8ebf7a38a9a32fcd14d02b393dca8b9cba346789`  
		Last Modified: Thu, 12 Oct 2023 01:16:19 GMT  
		Size: 52.6 MB (52643890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6b13ce2c8b747fb0a75dc838a5b709fa75c3ae125301058f70da5e25c7ba79`  
		Last Modified: Thu, 12 Oct 2023 01:16:11 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.3.0-alpine`

```console
$ docker pull varnish@sha256:1eaaf02632201e9eb10980f58574e4d5b9bce3a96f4f146313e50d92901ae5de
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
$ docker pull varnish@sha256:c50109176635d4d06d1e3e8e2d6935d30a999947a87a9915adfc38911c3edbf0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.4 MB (59353279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6814db3789c866db3caba06dcbf3a5af9894ab56e19d8e605215f65f9f63d01`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:20:37 GMT
ADD file:4faae297b6caba92e1791a5ff667be0fcb4de6a4de2df155395957ef9d8ad5e5 in / 
# Mon, 07 Aug 2023 19:20:37 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:07:42 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 09 Aug 2023 04:07:43 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 09 Aug 2023 04:07:43 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 09 Aug 2023 04:07:43 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 09 Aug 2023 04:07:43 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 09 Aug 2023 04:07:43 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 09 Aug 2023 04:07:43 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 09 Aug 2023 04:07:43 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 09 Aug 2023 04:07:43 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Wed, 09 Aug 2023 04:07:43 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Wed, 09 Aug 2023 04:07:43 GMT
ENV VARNISH_SIZE=100M
# Wed, 09 Aug 2023 04:09:00 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Wed, 09 Aug 2023 04:09:01 GMT
WORKDIR /etc/varnish
# Wed, 09 Aug 2023 04:09:01 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 09 Aug 2023 04:09:01 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 09 Aug 2023 04:09:01 GMT
USER varnish
# Wed, 09 Aug 2023 04:09:01 GMT
EXPOSE 80 8443
# Wed, 09 Aug 2023 04:09:01 GMT
CMD []
```

-	Layers:
	-	`sha256:3695f6c099b80e503148dbb435d044c35147f81d34b9d6fbb27b3dcf1fd7ecaf`  
		Last Modified: Mon, 07 Aug 2023 19:21:27 GMT  
		Size: 2.8 MB (2826006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a571445311e41e13f2fc1c6ace8610ded14d6ac0c9a00d88f8fc8907d48e2f`  
		Last Modified: Wed, 09 Aug 2023 04:10:57 GMT  
		Size: 56.5 MB (56526777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f0487466108411358ef19a0fa4e224b5368812219ee7a97f6fca2b9c34e188`  
		Last Modified: Wed, 09 Aug 2023 04:10:50 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3.0-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:a9066203838a2bbf6acd2a4af3dc33997546bf8e67c2502c6185b3e9d983cad7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45110187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e147f405a969edfd9f1c37b4f1a4429593d5975f3c68e98d04bc95c209c112be`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:57:37 GMT
ADD file:842dfa6e14e0537b53781830cfb26da9fa7a63229a7a1decc0fe08d8c000b5a9 in / 
# Mon, 07 Aug 2023 19:57:37 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 21:52:52 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Tue, 08 Aug 2023 21:52:52 GMT
ARG VARNISH_VERSION=7.3.0
# Tue, 08 Aug 2023 21:52:53 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Tue, 08 Aug 2023 21:52:53 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 08 Aug 2023 21:52:54 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 08 Aug 2023 21:52:54 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Tue, 08 Aug 2023 21:52:54 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Tue, 08 Aug 2023 21:52:54 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Tue, 08 Aug 2023 21:52:54 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 08 Aug 2023 21:52:55 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Tue, 08 Aug 2023 21:52:55 GMT
ENV VARNISH_SIZE=100M
# Tue, 08 Aug 2023 21:54:47 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Tue, 08 Aug 2023 21:54:47 GMT
WORKDIR /etc/varnish
# Tue, 08 Aug 2023 21:54:47 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 08 Aug 2023 21:54:47 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 08 Aug 2023 21:54:47 GMT
USER varnish
# Tue, 08 Aug 2023 21:54:47 GMT
EXPOSE 80 8443
# Tue, 08 Aug 2023 21:54:47 GMT
CMD []
```

-	Layers:
	-	`sha256:c25753df0ee4b6d3db1dacebcfb1839260ed067556f1f3ff52ddb574cab51045`  
		Last Modified: Mon, 07 Aug 2023 19:58:28 GMT  
		Size: 2.4 MB (2436761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3835c5b95f60e45f72f9756939da73ac2e053ce0e8b25927e9c38eafaa28134d`  
		Last Modified: Tue, 08 Aug 2023 21:57:08 GMT  
		Size: 42.7 MB (42672929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d6e8e8160593ed0c9c95f9057b778ef9a351adb3eaace602c4d2313dbb2d80`  
		Last Modified: Tue, 08 Aug 2023 21:57:00 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3.0-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:fa2793323936a2a39bc749fe8c9f4d57ed1f5cacfc7bebd45acab4714d719ac6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52090034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73f5f31a9b25c2236a27ca4ea7326c16321adb4109342c0f4b66cb18945fc936`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:39:29 GMT
ADD file:21f240e1e33b25dacee7291cdd8c7750995aa0f460d13496a08c4a2dd92323aa in / 
# Mon, 07 Aug 2023 19:39:29 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:27:59 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 09 Aug 2023 04:27:59 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 09 Aug 2023 04:27:59 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 09 Aug 2023 04:28:00 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 09 Aug 2023 04:28:00 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 09 Aug 2023 04:28:00 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 09 Aug 2023 04:28:00 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 09 Aug 2023 04:28:00 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 09 Aug 2023 04:28:00 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Wed, 09 Aug 2023 04:28:00 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Wed, 09 Aug 2023 04:28:00 GMT
ENV VARNISH_SIZE=100M
# Wed, 09 Aug 2023 04:29:12 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Wed, 09 Aug 2023 04:29:13 GMT
WORKDIR /etc/varnish
# Wed, 09 Aug 2023 04:29:13 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 09 Aug 2023 04:29:13 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 09 Aug 2023 04:29:13 GMT
USER varnish
# Wed, 09 Aug 2023 04:29:13 GMT
EXPOSE 80 8443
# Wed, 09 Aug 2023 04:29:13 GMT
CMD []
```

-	Layers:
	-	`sha256:ad3fa0ea069c04e4ee9be58cf0ae9e1a8a56f649b96a96298203b055e8c903ff`  
		Last Modified: Mon, 07 Aug 2023 19:40:16 GMT  
		Size: 2.7 MB (2720868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af416d837d369577895656da730e7b9045ced484cb509a3c8d24ea5651f2b72b`  
		Last Modified: Wed, 09 Aug 2023 04:30:54 GMT  
		Size: 49.4 MB (49368670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72ad8cfaa77fff8808621330b797c9dcd268d87ee399f1cadc48654257351c9`  
		Last Modified: Wed, 09 Aug 2023 04:30:49 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3.0-alpine` - linux; 386

```console
$ docker pull varnish@sha256:40db9d7b920acf3c24a1f0fc818151592d3d617cd98e20b08149fc9526fc24c1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59534324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7db33e169f8fc0973f7d7ebf8d7a395cf221ac4eb15d75050d00bbf746d39e28`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:38:38 GMT
ADD file:2d8ac62dd229ef26536f5a9af9e61df30ea68d609fa969786dfd531aea18cf3c in / 
# Mon, 07 Aug 2023 19:38:38 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 22:26:01 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Tue, 08 Aug 2023 22:26:01 GMT
ARG VARNISH_VERSION=7.3.0
# Tue, 08 Aug 2023 22:26:01 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Tue, 08 Aug 2023 22:26:01 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 08 Aug 2023 22:26:01 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 08 Aug 2023 22:26:01 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Tue, 08 Aug 2023 22:26:01 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Tue, 08 Aug 2023 22:26:02 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Tue, 08 Aug 2023 22:26:02 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 08 Aug 2023 22:26:02 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Tue, 08 Aug 2023 22:26:02 GMT
ENV VARNISH_SIZE=100M
# Tue, 08 Aug 2023 22:28:20 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Tue, 08 Aug 2023 22:28:21 GMT
WORKDIR /etc/varnish
# Tue, 08 Aug 2023 22:28:21 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 08 Aug 2023 22:28:21 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 08 Aug 2023 22:28:21 GMT
USER varnish
# Tue, 08 Aug 2023 22:28:21 GMT
EXPOSE 80 8443
# Tue, 08 Aug 2023 22:28:22 GMT
CMD []
```

-	Layers:
	-	`sha256:add53095769493cde9110fd91f113357e53b9e0d94abf216b811fcf00107674e`  
		Last Modified: Mon, 07 Aug 2023 19:39:29 GMT  
		Size: 2.8 MB (2832316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f647a86d2fc80d9f872ddaf183a99650a85e6bb6db7ab28df1aa47f8c766c37a`  
		Last Modified: Tue, 08 Aug 2023 22:30:58 GMT  
		Size: 56.7 MB (56701511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4a6dc8cb05579dc1a1b1fcb6f15a0661ae9a7feaf8ba4eb6397236e86e4143`  
		Last Modified: Tue, 08 Aug 2023 22:30:48 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3.0-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:c3a57b142209c5534422dc949c7c67a1ec15ef65f53837b3ecdce1507c22ad17
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49132355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78138cefb19943eea37fdcc772c9f4065c5177abf063d6fcb02c473414a5e3c4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 20:16:50 GMT
ADD file:f730d2cd05a420ffd38548ae1611345fc40a7db59dea5ff41328caa60ee42608 in / 
# Mon, 07 Aug 2023 20:16:51 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:50:57 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Tue, 08 Aug 2023 23:50:58 GMT
ARG VARNISH_VERSION=7.3.0
# Tue, 08 Aug 2023 23:50:58 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Tue, 08 Aug 2023 23:50:59 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 08 Aug 2023 23:50:59 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 08 Aug 2023 23:51:00 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Tue, 08 Aug 2023 23:51:00 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Tue, 08 Aug 2023 23:51:01 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Tue, 08 Aug 2023 23:51:01 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 08 Aug 2023 23:51:02 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Tue, 08 Aug 2023 23:51:02 GMT
ENV VARNISH_SIZE=100M
# Tue, 08 Aug 2023 23:53:25 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Tue, 08 Aug 2023 23:53:28 GMT
WORKDIR /etc/varnish
# Tue, 08 Aug 2023 23:53:28 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 08 Aug 2023 23:53:28 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 08 Aug 2023 23:53:28 GMT
USER varnish
# Tue, 08 Aug 2023 23:53:29 GMT
EXPOSE 80 8443
# Tue, 08 Aug 2023 23:53:29 GMT
CMD []
```

-	Layers:
	-	`sha256:f1ecf55aa97fb0011a1c90ffc58e5cb218908bc85a13afe003aea5a46e045ac8`  
		Last Modified: Mon, 07 Aug 2023 20:18:07 GMT  
		Size: 2.8 MB (2812358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e313b1b6994e0de7da0d5b504d453dd6890fafeb0e8debf9808e953fcfc3e1d1`  
		Last Modified: Tue, 08 Aug 2023 23:56:42 GMT  
		Size: 46.3 MB (46319501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f91dcda5c6dfcb572578877b768d18db70e587fc1cc7ce78429376e9546b94`  
		Last Modified: Tue, 08 Aug 2023 23:56:31 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3.0-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:4d0ba154b6574f740056123e5f8384b43d90feab3dd12fb2bc6d4eca68a6bcd0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47593252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00fb757c92f0c2efeaa1eb32bcafb1400510fc0fb7ff5c160bd2714a1325cff4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:42:16 GMT
ADD file:db6cafb0897c5e32510edd0166d1e1b23001bef271dad57e4157d560bd09dd93 in / 
# Mon, 07 Aug 2023 19:42:16 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:19:26 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 09 Aug 2023 04:19:27 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 09 Aug 2023 04:19:27 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 09 Aug 2023 04:19:28 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 09 Aug 2023 04:19:29 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 09 Aug 2023 04:19:30 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 09 Aug 2023 04:19:30 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 09 Aug 2023 04:19:31 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 09 Aug 2023 04:19:32 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Wed, 09 Aug 2023 04:19:33 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Wed, 09 Aug 2023 04:19:34 GMT
ENV VARNISH_SIZE=100M
# Wed, 09 Aug 2023 04:21:51 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Wed, 09 Aug 2023 04:22:01 GMT
WORKDIR /etc/varnish
# Wed, 09 Aug 2023 04:22:01 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 09 Aug 2023 04:22:02 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 09 Aug 2023 04:22:03 GMT
USER varnish
# Wed, 09 Aug 2023 04:22:03 GMT
EXPOSE 80 8443
# Wed, 09 Aug 2023 04:22:04 GMT
CMD []
```

-	Layers:
	-	`sha256:ec103030fda7a896185e8eb8a4f00b7f611725434956faa395cf74a993a2742e`  
		Last Modified: Mon, 07 Aug 2023 19:43:01 GMT  
		Size: 2.6 MB (2609002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161846c9c73015426cc80840fbb38cd2016810411f252eb724f4fee1ea84cfbc`  
		Last Modified: Wed, 09 Aug 2023 04:25:34 GMT  
		Size: 45.0 MB (44983753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893cc747d7f6b07b13980f3ceffbd432e9f4f78e9025f02e37ce6eb64e576b48`  
		Last Modified: Wed, 09 Aug 2023 04:25:28 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.4`

```console
$ docker pull varnish@sha256:8aebb0e2fdb98f8c8f08529f42264f599ce08a7ab0179236767aebaaa62d6d7e
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
$ docker pull varnish@sha256:e03566ef6752192c478b1aa7bba603dc26f1ee563934c03f28e9c6a7a5396d59
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134737591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:266771d9cf5c42149096e6813c1b152608a114703951e87c69ce3220c862ab70`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 18:34:50 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 11 Oct 2023 18:34:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:27:13 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Wed, 11 Oct 2023 21:27:13 GMT
ARG VARNISH_VERSION=7.4.1
# Wed, 11 Oct 2023 21:27:13 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Wed, 11 Oct 2023 21:27:14 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 11 Oct 2023 21:27:14 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 11 Oct 2023 21:27:14 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Wed, 11 Oct 2023 21:27:14 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Wed, 11 Oct 2023 21:27:14 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Wed, 11 Oct 2023 21:27:14 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Wed, 11 Oct 2023 21:27:14 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Wed, 11 Oct 2023 21:27:14 GMT
ENV VARNISH_SIZE=100M
# Wed, 11 Oct 2023 21:30:00 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.1.tgz -o $tmpdir/orig.tgz;     echo "d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 11 Oct 2023 21:30:01 GMT
WORKDIR /etc/varnish
# Wed, 11 Oct 2023 21:30:01 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 11 Oct 2023 21:30:01 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 11 Oct 2023 21:30:01 GMT
USER varnish
# Wed, 11 Oct 2023 21:30:01 GMT
EXPOSE 80 8443
# Wed, 11 Oct 2023 21:30:01 GMT
CMD []
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73d3b02baeacb05096f1d533167545798575b4b39a4f516a201ad8a3c0fd9e0`  
		Last Modified: Wed, 11 Oct 2023 21:35:14 GMT  
		Size: 105.6 MB (105587228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c88afe6700045cede25a79c7cae3b4fd9c2630ea13c3445c62ee292dc732123`  
		Last Modified: Wed, 11 Oct 2023 21:34:59 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4` - linux; arm variant v7

```console
$ docker pull varnish@sha256:1feecff1374e6c3d603761b67362c81d8a15190b4fce34911d6257281a848cad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105036990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91cb20c34e8cd2ad07e5e4d7fb9e378a81db336a803bd894fda058508b99013f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:42:11 GMT
ADD file:da08fed31a161a2210fd920a1b5e43aa3f4199985cdeaa0d5d24c0a0f19044aa in / 
# Wed, 11 Oct 2023 17:42:11 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:09:22 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Wed, 11 Oct 2023 18:09:22 GMT
ARG VARNISH_VERSION=7.4.1
# Wed, 11 Oct 2023 18:09:22 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Wed, 11 Oct 2023 18:09:22 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 11 Oct 2023 18:09:22 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 11 Oct 2023 18:09:22 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Wed, 11 Oct 2023 18:09:22 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Wed, 11 Oct 2023 18:09:22 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Wed, 11 Oct 2023 18:09:22 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Wed, 11 Oct 2023 18:09:22 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Wed, 11 Oct 2023 18:09:23 GMT
ENV VARNISH_SIZE=100M
# Wed, 11 Oct 2023 18:12:11 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.1.tgz -o $tmpdir/orig.tgz;     echo "d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 11 Oct 2023 18:12:12 GMT
WORKDIR /etc/varnish
# Wed, 11 Oct 2023 18:12:12 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 11 Oct 2023 18:12:12 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 11 Oct 2023 18:12:12 GMT
USER varnish
# Wed, 11 Oct 2023 18:12:12 GMT
EXPOSE 80 8443
# Wed, 11 Oct 2023 18:12:12 GMT
CMD []
```

-	Layers:
	-	`sha256:2f11c34abc7b59f09b58bb6e2cf54f260f4b4142ecf8023a114e281ea4b532d1`  
		Last Modified: Wed, 11 Oct 2023 17:46:22 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3d75364756f4e459e71b5941b35371acb082f8bb2f09c42230d48ff70cfa56`  
		Last Modified: Wed, 11 Oct 2023 18:17:46 GMT  
		Size: 80.3 MB (80287576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd120edc727486131696ee7b8fb97154d80d4812e8c1865198e8b909d2e8e457`  
		Last Modified: Wed, 11 Oct 2023 18:17:34 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:472bd27e1d4a42daf22c320d58944cf4ea8243a2a3dd9300e1cb7b76264bedda
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.2 MB (129197485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6368c63db1f983c26740d4676cf9ae4da73811320dd0f21fabf6191e6e872ca`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 20 Sep 2023 02:44:13 GMT
ADD file:ec1a6e0aedd76c8fdc8544775f8b553f58950e9435f5cfe919f39374e222cfbb in / 
# Wed, 20 Sep 2023 02:44:14 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 17:48:56 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 21 Sep 2023 04:34:35 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 21 Sep 2023 04:34:36 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 21 Sep 2023 04:34:36 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 21 Sep 2023 04:34:36 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 21 Sep 2023 04:34:36 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 21 Sep 2023 04:34:36 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 21 Sep 2023 04:34:36 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 21 Sep 2023 04:34:36 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 21 Sep 2023 04:34:36 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Thu, 21 Sep 2023 04:34:36 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Sep 2023 04:37:04 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.1.tgz -o $tmpdir/orig.tgz;     echo "d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 21 Sep 2023 04:37:06 GMT
WORKDIR /etc/varnish
# Thu, 21 Sep 2023 04:37:06 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 21 Sep 2023 04:37:06 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Sep 2023 04:37:06 GMT
USER varnish
# Thu, 21 Sep 2023 04:37:06 GMT
EXPOSE 80 8443
# Thu, 21 Sep 2023 04:37:06 GMT
CMD []
```

-	Layers:
	-	`sha256:e886f0f47ef56fcadb6ecaf2116056bbdb273e0afe07ed034498b198d386c04e`  
		Last Modified: Wed, 20 Sep 2023 02:47:36 GMT  
		Size: 29.2 MB (29157221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d168552ad41a2f9b1ae51e74b416a1fbf5f899631badf1ecf74bb5962f131c8`  
		Last Modified: Thu, 21 Sep 2023 04:41:26 GMT  
		Size: 100.0 MB (100039772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aee0db284127fd79a1e633f9ee036d58c5817770e41d69607d88963d53c073f`  
		Last Modified: Thu, 21 Sep 2023 04:41:15 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4` - linux; 386

```console
$ docker pull varnish@sha256:b0b281bd04e70c06c4d95562ddc165603c7fcb63797a5307ea577d0854a46ba0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131877976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8763c9a49d7d742b60afd31d81ea0e3816bba8e58111f0d3bfc26b36fc3c66f5`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:40:42 GMT
ADD file:31318c1b1f05d559cce42f5b12eef97d916932217e0b987fb07c0fc11bf0a14a in / 
# Wed, 11 Oct 2023 17:40:42 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 08:38:19 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 12 Oct 2023 08:38:19 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 12 Oct 2023 08:38:20 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 12 Oct 2023 08:38:20 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 12 Oct 2023 08:38:20 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 12 Oct 2023 08:38:20 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 12 Oct 2023 08:38:20 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 12 Oct 2023 08:38:20 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 12 Oct 2023 08:38:20 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 12 Oct 2023 08:38:20 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Thu, 12 Oct 2023 08:38:20 GMT
ENV VARNISH_SIZE=100M
# Thu, 12 Oct 2023 08:42:04 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.1.tgz -o $tmpdir/orig.tgz;     echo "d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 12 Oct 2023 08:42:05 GMT
WORKDIR /etc/varnish
# Thu, 12 Oct 2023 08:42:05 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 12 Oct 2023 08:42:05 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 12 Oct 2023 08:42:06 GMT
USER varnish
# Thu, 12 Oct 2023 08:42:06 GMT
EXPOSE 80 8443
# Thu, 12 Oct 2023 08:42:06 GMT
CMD []
```

-	Layers:
	-	`sha256:b27d0f1369837277a82877763487cdd2535037988fc27e16f11cf74e103ae4cd`  
		Last Modified: Wed, 11 Oct 2023 17:45:31 GMT  
		Size: 30.2 MB (30164118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4d7224a6538ed66733bc96ac79177a58d0039e0e68594173cc295e2ea9b504`  
		Last Modified: Thu, 12 Oct 2023 08:48:35 GMT  
		Size: 101.7 MB (101713366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:621ed1744001a5b482de115c1a397507d44f792c45cdd41dce56ecb1fca9cbe3`  
		Last Modified: Thu, 12 Oct 2023 08:48:15 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4` - linux; ppc64le

```console
$ docker pull varnish@sha256:180fe86166e9d0d3b446cedb5e1b6b04f386a146b06c3e5faa0c574866f91999
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.7 MB (137667538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b6eb4c889e8ef2ee0187d1b231a86f99e559d96be323785f2739b97ea92f83d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:44:19 GMT
ADD file:53c83bdd58e7c4003ae769596cc2f8e6b72c0bbb854dbe7f006a39f273848b1b in / 
# Wed, 11 Oct 2023 17:44:21 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 12:12:26 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 12 Oct 2023 12:12:27 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 12 Oct 2023 12:12:27 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 12 Oct 2023 12:12:27 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 12 Oct 2023 12:12:28 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 12 Oct 2023 12:12:28 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 12 Oct 2023 12:12:29 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 12 Oct 2023 12:12:29 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 12 Oct 2023 12:12:29 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 12 Oct 2023 12:12:30 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Thu, 12 Oct 2023 12:12:30 GMT
ENV VARNISH_SIZE=100M
# Thu, 12 Oct 2023 12:19:14 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.1.tgz -o $tmpdir/orig.tgz;     echo "d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 12 Oct 2023 12:19:21 GMT
WORKDIR /etc/varnish
# Thu, 12 Oct 2023 12:19:21 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 12 Oct 2023 12:19:22 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 12 Oct 2023 12:19:22 GMT
USER varnish
# Thu, 12 Oct 2023 12:19:23 GMT
EXPOSE 80 8443
# Thu, 12 Oct 2023 12:19:24 GMT
CMD []
```

-	Layers:
	-	`sha256:54813908ce8a5d8a81f2db88ad0366eb5266484c7c402e5e93ef26e764f7a0e2`  
		Last Modified: Wed, 11 Oct 2023 17:49:58 GMT  
		Size: 33.1 MB (33141653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30256924f5530cebc1ea042b5fde8499f912e388dc12580b7f4bfb886ed621b9`  
		Last Modified: Thu, 12 Oct 2023 12:31:24 GMT  
		Size: 104.5 MB (104525394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2d85d3edf39adfb61ceeaf1b92b4960089dd68c909e2f2668a96803ddb162b`  
		Last Modified: Thu, 12 Oct 2023 12:30:58 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4` - linux; s390x

```console
$ docker pull varnish@sha256:c16359d33b507ad0702a5be497bc4d3bf1dc9550a6b72a01fbfef0d10a15d9e3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112330094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd8caa54cdeafd2ed33943de55ef8effd990147fcb9b0311032a90892878efb1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:50:28 GMT
ADD file:b85ed0ed01200dd3626d66cf5205d989fc48e61b3dd3498f777ee72d91e64870 in / 
# Wed, 11 Oct 2023 17:50:30 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 00:48:18 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 12 Oct 2023 00:48:18 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 12 Oct 2023 00:48:18 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 12 Oct 2023 00:48:18 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 12 Oct 2023 00:48:19 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 12 Oct 2023 00:48:19 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 12 Oct 2023 00:48:19 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 12 Oct 2023 00:48:19 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 12 Oct 2023 00:48:19 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 12 Oct 2023 00:48:19 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Thu, 12 Oct 2023 00:48:19 GMT
ENV VARNISH_SIZE=100M
# Thu, 12 Oct 2023 01:06:58 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.1.tgz -o $tmpdir/orig.tgz;     echo "d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 12 Oct 2023 01:07:08 GMT
WORKDIR /etc/varnish
# Thu, 12 Oct 2023 01:07:08 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 12 Oct 2023 01:07:08 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 12 Oct 2023 01:07:08 GMT
USER varnish
# Thu, 12 Oct 2023 01:07:09 GMT
EXPOSE 80 8443
# Thu, 12 Oct 2023 01:07:09 GMT
CMD []
```

-	Layers:
	-	`sha256:f270c1bb05fa46b165ce3680225dc9fa5bbfe4d69420a467350e80f692c78eb2`  
		Last Modified: Wed, 11 Oct 2023 17:56:03 GMT  
		Size: 27.5 MB (27512850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1ecabb8eb208085a0cd1ccad185b3741ef91253ac090a644273393b03d5ba9`  
		Last Modified: Thu, 12 Oct 2023 01:15:40 GMT  
		Size: 84.8 MB (84816753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b8069a9787fb8bc5a96e8c2c9afaa0c689c46501adc3724923dd883a96e1fd7`  
		Last Modified: Thu, 12 Oct 2023 01:15:29 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.4-alpine`

```console
$ docker pull varnish@sha256:ecf79e7945d24f92b505735170fac696ead578391da5e81183bb814d058841d4
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
$ docker pull varnish@sha256:8fd5e0d68a7bcb6c3a41155bb3b27a8cdc1ac3ebda8bc380de9b1448c958933b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (60984690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a672dc2e7c14234d749faf94e5af11adbc33c7f66fc1a0aebb3f95e34e893bb3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:20:37 GMT
ADD file:4faae297b6caba92e1791a5ff667be0fcb4de6a4de2df155395957ef9d8ad5e5 in / 
# Mon, 07 Aug 2023 19:20:37 GMT
CMD ["/bin/sh"]
# Mon, 18 Sep 2023 19:25:17 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 21 Sep 2023 10:03:06 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 21 Sep 2023 10:03:06 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 21 Sep 2023 10:03:06 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 21 Sep 2023 10:03:07 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 21 Sep 2023 10:03:07 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 21 Sep 2023 10:03:07 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 21 Sep 2023 10:03:07 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 21 Sep 2023 10:03:07 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 21 Sep 2023 10:03:07 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Thu, 21 Sep 2023 10:03:07 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Sep 2023 10:04:27 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Sep 2023 10:04:27 GMT
WORKDIR /etc/varnish
# Thu, 21 Sep 2023 10:04:27 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 21 Sep 2023 10:04:28 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Sep 2023 10:04:28 GMT
USER varnish
# Thu, 21 Sep 2023 10:04:28 GMT
EXPOSE 80 8443
# Thu, 21 Sep 2023 10:04:28 GMT
CMD []
```

-	Layers:
	-	`sha256:3695f6c099b80e503148dbb435d044c35147f81d34b9d6fbb27b3dcf1fd7ecaf`  
		Last Modified: Mon, 07 Aug 2023 19:21:27 GMT  
		Size: 2.8 MB (2826006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39051c6545f1b0c198fe83b7ffacdadb4c62c1a65bb4548192143c3c7a006ab`  
		Last Modified: Thu, 21 Sep 2023 10:08:31 GMT  
		Size: 58.2 MB (58158186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d139fff6dbe170e2eadf9014aa5ff95a6127606f4325169031bdc1f8c1b9c834`  
		Last Modified: Thu, 21 Sep 2023 10:08:23 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:53f9b3af759587518f192eec1f3c70599bcea9f9eda6a87fbf32ba90f3fec2a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.3 MB (45251077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb9c94e956b808d696f8ad9a59e811e54a348f0230eba580630885aaee1ca603`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:57:37 GMT
ADD file:842dfa6e14e0537b53781830cfb26da9fa7a63229a7a1decc0fe08d8c000b5a9 in / 
# Mon, 07 Aug 2023 19:57:37 GMT
CMD ["/bin/sh"]
# Mon, 18 Sep 2023 20:16:10 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Wed, 20 Sep 2023 22:07:41 GMT
ARG VARNISH_VERSION=7.4.1
# Wed, 20 Sep 2023 22:07:41 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Wed, 20 Sep 2023 22:07:41 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 20 Sep 2023 22:07:41 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 20 Sep 2023 22:07:42 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Wed, 20 Sep 2023 22:07:42 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Wed, 20 Sep 2023 22:07:42 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Wed, 20 Sep 2023 22:07:42 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Wed, 20 Sep 2023 22:07:42 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Wed, 20 Sep 2023 22:07:43 GMT
ENV VARNISH_SIZE=100M
# Wed, 20 Sep 2023 22:10:33 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Wed, 20 Sep 2023 22:10:34 GMT
WORKDIR /etc/varnish
# Wed, 20 Sep 2023 22:10:34 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:10:34 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 20 Sep 2023 22:10:34 GMT
USER varnish
# Wed, 20 Sep 2023 22:10:35 GMT
EXPOSE 80 8443
# Wed, 20 Sep 2023 22:10:35 GMT
CMD []
```

-	Layers:
	-	`sha256:c25753df0ee4b6d3db1dacebcfb1839260ed067556f1f3ff52ddb574cab51045`  
		Last Modified: Mon, 07 Aug 2023 19:58:28 GMT  
		Size: 2.4 MB (2436761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3edaa1bb34a769d2a617d179c3a121ce323795b2d86f371adf2b18198108ff`  
		Last Modified: Wed, 20 Sep 2023 22:17:51 GMT  
		Size: 42.8 MB (42813817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571ba818c66eb7ccee714ee8e27bf848d97144ffa2ee3885ce0d1ba9bc5edf66`  
		Last Modified: Wed, 20 Sep 2023 22:17:46 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:97de9f09c69852f96f7c296187539c50dea1aea1f5104e0c5c0c300ae8683af8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.2 MB (52224736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03377611cb0f40f9ce132047f83c95c50a27b27b11429d16a7be1312b16fa719`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:39:29 GMT
ADD file:21f240e1e33b25dacee7291cdd8c7750995aa0f460d13496a08c4a2dd92323aa in / 
# Mon, 07 Aug 2023 19:39:29 GMT
CMD ["/bin/sh"]
# Mon, 18 Sep 2023 19:52:54 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 21 Sep 2023 04:37:13 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 21 Sep 2023 04:37:13 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 21 Sep 2023 04:37:14 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 21 Sep 2023 04:37:14 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 21 Sep 2023 04:37:14 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 21 Sep 2023 04:37:14 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 21 Sep 2023 04:37:14 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 21 Sep 2023 04:37:14 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 21 Sep 2023 04:37:14 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Thu, 21 Sep 2023 04:37:14 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Sep 2023 04:38:26 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Sep 2023 04:38:27 GMT
WORKDIR /etc/varnish
# Thu, 21 Sep 2023 04:38:27 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 21 Sep 2023 04:38:27 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Sep 2023 04:38:27 GMT
USER varnish
# Thu, 21 Sep 2023 04:38:27 GMT
EXPOSE 80 8443
# Thu, 21 Sep 2023 04:38:27 GMT
CMD []
```

-	Layers:
	-	`sha256:ad3fa0ea069c04e4ee9be58cf0ae9e1a8a56f649b96a96298203b055e8c903ff`  
		Last Modified: Mon, 07 Aug 2023 19:40:16 GMT  
		Size: 2.7 MB (2720868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43115af36871113661de523d5f39c294c446e845b191847bee9039f91080b5e5`  
		Last Modified: Thu, 21 Sep 2023 04:41:44 GMT  
		Size: 49.5 MB (49503372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f08a4e7fb6fee04d2a988db665d17b65b17707f7325f9ec73cb624907e43a2`  
		Last Modified: Thu, 21 Sep 2023 04:41:38 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4-alpine` - linux; 386

```console
$ docker pull varnish@sha256:5aa6916b378447ac7ce3bce16083f21640ed77f346d9c6b6110232d87f9c8a01
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.1 MB (61137578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e205d190ad66189082289bc366ecf0ec42f35f54efea247d7e628253d2ba02c6`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:38:38 GMT
ADD file:2d8ac62dd229ef26536f5a9af9e61df30ea68d609fa969786dfd531aea18cf3c in / 
# Mon, 07 Aug 2023 19:38:38 GMT
CMD ["/bin/sh"]
# Mon, 18 Sep 2023 19:42:30 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 21 Sep 2023 02:30:06 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 21 Sep 2023 02:30:06 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 21 Sep 2023 02:30:06 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 21 Sep 2023 02:30:06 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 21 Sep 2023 02:30:06 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 21 Sep 2023 02:30:06 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 21 Sep 2023 02:30:07 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 21 Sep 2023 02:30:07 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 21 Sep 2023 02:30:07 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Thu, 21 Sep 2023 02:30:07 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Sep 2023 02:32:23 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Sep 2023 02:32:23 GMT
WORKDIR /etc/varnish
# Thu, 21 Sep 2023 02:32:24 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 21 Sep 2023 02:32:24 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Sep 2023 02:32:24 GMT
USER varnish
# Thu, 21 Sep 2023 02:32:24 GMT
EXPOSE 80 8443
# Thu, 21 Sep 2023 02:32:24 GMT
CMD []
```

-	Layers:
	-	`sha256:add53095769493cde9110fd91f113357e53b9e0d94abf216b811fcf00107674e`  
		Last Modified: Mon, 07 Aug 2023 19:39:29 GMT  
		Size: 2.8 MB (2832316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c150ec529b4641ae75ebddb680c40d4461ff6cb20cc9de9000d09e55c4cc77ae`  
		Last Modified: Thu, 21 Sep 2023 02:39:33 GMT  
		Size: 58.3 MB (58304764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d857ef55991e2baf89bc4c3c90d9b09873a4a3f98625ef9aff38572db418bdc`  
		Last Modified: Thu, 21 Sep 2023 02:39:22 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:6e774ae86d3ccd908f2effc52757ac4d1253f3a19bc81f2aa0fe7bcff9aa1f1b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49267291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d42006d222979c85edb1b343cc64120bcfde800a88fe802c42c9983c8491b645`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 20:16:50 GMT
ADD file:f730d2cd05a420ffd38548ae1611345fc40a7db59dea5ff41328caa60ee42608 in / 
# Mon, 07 Aug 2023 20:16:51 GMT
CMD ["/bin/sh"]
# Mon, 18 Sep 2023 19:23:54 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 21 Sep 2023 01:05:18 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 21 Sep 2023 01:05:18 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 21 Sep 2023 01:05:18 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 21 Sep 2023 01:05:19 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 21 Sep 2023 01:05:19 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 21 Sep 2023 01:05:19 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 21 Sep 2023 01:05:19 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 21 Sep 2023 01:05:20 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 21 Sep 2023 01:05:20 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Thu, 21 Sep 2023 01:05:20 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Sep 2023 01:07:35 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Sep 2023 01:07:37 GMT
WORKDIR /etc/varnish
# Thu, 21 Sep 2023 01:07:37 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 21 Sep 2023 01:07:38 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Sep 2023 01:07:38 GMT
USER varnish
# Thu, 21 Sep 2023 01:07:38 GMT
EXPOSE 80 8443
# Thu, 21 Sep 2023 01:07:38 GMT
CMD []
```

-	Layers:
	-	`sha256:f1ecf55aa97fb0011a1c90ffc58e5cb218908bc85a13afe003aea5a46e045ac8`  
		Last Modified: Mon, 07 Aug 2023 20:18:07 GMT  
		Size: 2.8 MB (2812358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:487e7414b13c044e2fe3ed2d0c178b35a7c77da1716fd0f18713c4b30bf0e8e2`  
		Last Modified: Thu, 21 Sep 2023 01:18:59 GMT  
		Size: 46.5 MB (46454433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e361115526684bb9e4ffadc8f804eff285d2ec63f814fb32981a3580974deded`  
		Last Modified: Thu, 21 Sep 2023 01:18:48 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:b098d4b1fdb99444ed73a7bbf08befce53f939ac48d20b65305b2819cbdbbe52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48935923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:357502947ec9a8ad3bdb2f0ed4673f3787524c7ebda92b216c258af34a941513`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:42:16 GMT
ADD file:db6cafb0897c5e32510edd0166d1e1b23001bef271dad57e4157d560bd09dd93 in / 
# Mon, 07 Aug 2023 19:42:16 GMT
CMD ["/bin/sh"]
# Mon, 18 Sep 2023 20:45:32 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 21 Sep 2023 01:49:29 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 21 Sep 2023 01:49:29 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 21 Sep 2023 01:49:29 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 21 Sep 2023 01:49:30 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 21 Sep 2023 01:49:30 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 21 Sep 2023 01:49:30 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 21 Sep 2023 01:49:30 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 21 Sep 2023 01:49:30 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 21 Sep 2023 01:49:30 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Thu, 21 Sep 2023 01:49:30 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Sep 2023 01:50:57 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Sep 2023 01:51:00 GMT
WORKDIR /etc/varnish
# Thu, 21 Sep 2023 01:51:00 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 21 Sep 2023 01:51:00 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Sep 2023 01:51:00 GMT
USER varnish
# Thu, 21 Sep 2023 01:51:00 GMT
EXPOSE 80 8443
# Thu, 21 Sep 2023 01:51:00 GMT
CMD []
```

-	Layers:
	-	`sha256:ec103030fda7a896185e8eb8a4f00b7f611725434956faa395cf74a993a2742e`  
		Last Modified: Mon, 07 Aug 2023 19:43:01 GMT  
		Size: 2.6 MB (2609002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c222777618072a84cbc1cc334e324f1cf6549d9aec24add4de60d61b25f04bf`  
		Last Modified: Thu, 21 Sep 2023 01:54:50 GMT  
		Size: 46.3 MB (46326423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f13e8e461de6c2bbbcf5890fd1669c82689bfea1ce6d63af764a6d281a801cf`  
		Last Modified: Thu, 21 Sep 2023 01:54:43 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.4.1`

```console
$ docker pull varnish@sha256:8aebb0e2fdb98f8c8f08529f42264f599ce08a7ab0179236767aebaaa62d6d7e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:7.4.1` - linux; amd64

```console
$ docker pull varnish@sha256:e03566ef6752192c478b1aa7bba603dc26f1ee563934c03f28e9c6a7a5396d59
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134737591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:266771d9cf5c42149096e6813c1b152608a114703951e87c69ce3220c862ab70`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 18:34:50 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 11 Oct 2023 18:34:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:27:13 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Wed, 11 Oct 2023 21:27:13 GMT
ARG VARNISH_VERSION=7.4.1
# Wed, 11 Oct 2023 21:27:13 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Wed, 11 Oct 2023 21:27:14 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 11 Oct 2023 21:27:14 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 11 Oct 2023 21:27:14 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Wed, 11 Oct 2023 21:27:14 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Wed, 11 Oct 2023 21:27:14 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Wed, 11 Oct 2023 21:27:14 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Wed, 11 Oct 2023 21:27:14 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Wed, 11 Oct 2023 21:27:14 GMT
ENV VARNISH_SIZE=100M
# Wed, 11 Oct 2023 21:30:00 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.1.tgz -o $tmpdir/orig.tgz;     echo "d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 11 Oct 2023 21:30:01 GMT
WORKDIR /etc/varnish
# Wed, 11 Oct 2023 21:30:01 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 11 Oct 2023 21:30:01 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 11 Oct 2023 21:30:01 GMT
USER varnish
# Wed, 11 Oct 2023 21:30:01 GMT
EXPOSE 80 8443
# Wed, 11 Oct 2023 21:30:01 GMT
CMD []
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73d3b02baeacb05096f1d533167545798575b4b39a4f516a201ad8a3c0fd9e0`  
		Last Modified: Wed, 11 Oct 2023 21:35:14 GMT  
		Size: 105.6 MB (105587228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c88afe6700045cede25a79c7cae3b4fd9c2630ea13c3445c62ee292dc732123`  
		Last Modified: Wed, 11 Oct 2023 21:34:59 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4.1` - linux; arm variant v7

```console
$ docker pull varnish@sha256:1feecff1374e6c3d603761b67362c81d8a15190b4fce34911d6257281a848cad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105036990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91cb20c34e8cd2ad07e5e4d7fb9e378a81db336a803bd894fda058508b99013f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:42:11 GMT
ADD file:da08fed31a161a2210fd920a1b5e43aa3f4199985cdeaa0d5d24c0a0f19044aa in / 
# Wed, 11 Oct 2023 17:42:11 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:09:22 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Wed, 11 Oct 2023 18:09:22 GMT
ARG VARNISH_VERSION=7.4.1
# Wed, 11 Oct 2023 18:09:22 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Wed, 11 Oct 2023 18:09:22 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 11 Oct 2023 18:09:22 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 11 Oct 2023 18:09:22 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Wed, 11 Oct 2023 18:09:22 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Wed, 11 Oct 2023 18:09:22 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Wed, 11 Oct 2023 18:09:22 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Wed, 11 Oct 2023 18:09:22 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Wed, 11 Oct 2023 18:09:23 GMT
ENV VARNISH_SIZE=100M
# Wed, 11 Oct 2023 18:12:11 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.1.tgz -o $tmpdir/orig.tgz;     echo "d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 11 Oct 2023 18:12:12 GMT
WORKDIR /etc/varnish
# Wed, 11 Oct 2023 18:12:12 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 11 Oct 2023 18:12:12 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 11 Oct 2023 18:12:12 GMT
USER varnish
# Wed, 11 Oct 2023 18:12:12 GMT
EXPOSE 80 8443
# Wed, 11 Oct 2023 18:12:12 GMT
CMD []
```

-	Layers:
	-	`sha256:2f11c34abc7b59f09b58bb6e2cf54f260f4b4142ecf8023a114e281ea4b532d1`  
		Last Modified: Wed, 11 Oct 2023 17:46:22 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3d75364756f4e459e71b5941b35371acb082f8bb2f09c42230d48ff70cfa56`  
		Last Modified: Wed, 11 Oct 2023 18:17:46 GMT  
		Size: 80.3 MB (80287576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd120edc727486131696ee7b8fb97154d80d4812e8c1865198e8b909d2e8e457`  
		Last Modified: Wed, 11 Oct 2023 18:17:34 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4.1` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:472bd27e1d4a42daf22c320d58944cf4ea8243a2a3dd9300e1cb7b76264bedda
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.2 MB (129197485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6368c63db1f983c26740d4676cf9ae4da73811320dd0f21fabf6191e6e872ca`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 20 Sep 2023 02:44:13 GMT
ADD file:ec1a6e0aedd76c8fdc8544775f8b553f58950e9435f5cfe919f39374e222cfbb in / 
# Wed, 20 Sep 2023 02:44:14 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 17:48:56 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 21 Sep 2023 04:34:35 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 21 Sep 2023 04:34:36 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 21 Sep 2023 04:34:36 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 21 Sep 2023 04:34:36 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 21 Sep 2023 04:34:36 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 21 Sep 2023 04:34:36 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 21 Sep 2023 04:34:36 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 21 Sep 2023 04:34:36 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 21 Sep 2023 04:34:36 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Thu, 21 Sep 2023 04:34:36 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Sep 2023 04:37:04 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.1.tgz -o $tmpdir/orig.tgz;     echo "d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 21 Sep 2023 04:37:06 GMT
WORKDIR /etc/varnish
# Thu, 21 Sep 2023 04:37:06 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 21 Sep 2023 04:37:06 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Sep 2023 04:37:06 GMT
USER varnish
# Thu, 21 Sep 2023 04:37:06 GMT
EXPOSE 80 8443
# Thu, 21 Sep 2023 04:37:06 GMT
CMD []
```

-	Layers:
	-	`sha256:e886f0f47ef56fcadb6ecaf2116056bbdb273e0afe07ed034498b198d386c04e`  
		Last Modified: Wed, 20 Sep 2023 02:47:36 GMT  
		Size: 29.2 MB (29157221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d168552ad41a2f9b1ae51e74b416a1fbf5f899631badf1ecf74bb5962f131c8`  
		Last Modified: Thu, 21 Sep 2023 04:41:26 GMT  
		Size: 100.0 MB (100039772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aee0db284127fd79a1e633f9ee036d58c5817770e41d69607d88963d53c073f`  
		Last Modified: Thu, 21 Sep 2023 04:41:15 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4.1` - linux; 386

```console
$ docker pull varnish@sha256:b0b281bd04e70c06c4d95562ddc165603c7fcb63797a5307ea577d0854a46ba0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131877976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8763c9a49d7d742b60afd31d81ea0e3816bba8e58111f0d3bfc26b36fc3c66f5`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:40:42 GMT
ADD file:31318c1b1f05d559cce42f5b12eef97d916932217e0b987fb07c0fc11bf0a14a in / 
# Wed, 11 Oct 2023 17:40:42 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 08:38:19 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 12 Oct 2023 08:38:19 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 12 Oct 2023 08:38:20 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 12 Oct 2023 08:38:20 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 12 Oct 2023 08:38:20 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 12 Oct 2023 08:38:20 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 12 Oct 2023 08:38:20 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 12 Oct 2023 08:38:20 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 12 Oct 2023 08:38:20 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 12 Oct 2023 08:38:20 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Thu, 12 Oct 2023 08:38:20 GMT
ENV VARNISH_SIZE=100M
# Thu, 12 Oct 2023 08:42:04 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.1.tgz -o $tmpdir/orig.tgz;     echo "d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 12 Oct 2023 08:42:05 GMT
WORKDIR /etc/varnish
# Thu, 12 Oct 2023 08:42:05 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 12 Oct 2023 08:42:05 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 12 Oct 2023 08:42:06 GMT
USER varnish
# Thu, 12 Oct 2023 08:42:06 GMT
EXPOSE 80 8443
# Thu, 12 Oct 2023 08:42:06 GMT
CMD []
```

-	Layers:
	-	`sha256:b27d0f1369837277a82877763487cdd2535037988fc27e16f11cf74e103ae4cd`  
		Last Modified: Wed, 11 Oct 2023 17:45:31 GMT  
		Size: 30.2 MB (30164118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4d7224a6538ed66733bc96ac79177a58d0039e0e68594173cc295e2ea9b504`  
		Last Modified: Thu, 12 Oct 2023 08:48:35 GMT  
		Size: 101.7 MB (101713366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:621ed1744001a5b482de115c1a397507d44f792c45cdd41dce56ecb1fca9cbe3`  
		Last Modified: Thu, 12 Oct 2023 08:48:15 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4.1` - linux; ppc64le

```console
$ docker pull varnish@sha256:180fe86166e9d0d3b446cedb5e1b6b04f386a146b06c3e5faa0c574866f91999
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.7 MB (137667538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b6eb4c889e8ef2ee0187d1b231a86f99e559d96be323785f2739b97ea92f83d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:44:19 GMT
ADD file:53c83bdd58e7c4003ae769596cc2f8e6b72c0bbb854dbe7f006a39f273848b1b in / 
# Wed, 11 Oct 2023 17:44:21 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 12:12:26 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 12 Oct 2023 12:12:27 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 12 Oct 2023 12:12:27 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 12 Oct 2023 12:12:27 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 12 Oct 2023 12:12:28 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 12 Oct 2023 12:12:28 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 12 Oct 2023 12:12:29 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 12 Oct 2023 12:12:29 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 12 Oct 2023 12:12:29 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 12 Oct 2023 12:12:30 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Thu, 12 Oct 2023 12:12:30 GMT
ENV VARNISH_SIZE=100M
# Thu, 12 Oct 2023 12:19:14 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.1.tgz -o $tmpdir/orig.tgz;     echo "d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 12 Oct 2023 12:19:21 GMT
WORKDIR /etc/varnish
# Thu, 12 Oct 2023 12:19:21 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 12 Oct 2023 12:19:22 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 12 Oct 2023 12:19:22 GMT
USER varnish
# Thu, 12 Oct 2023 12:19:23 GMT
EXPOSE 80 8443
# Thu, 12 Oct 2023 12:19:24 GMT
CMD []
```

-	Layers:
	-	`sha256:54813908ce8a5d8a81f2db88ad0366eb5266484c7c402e5e93ef26e764f7a0e2`  
		Last Modified: Wed, 11 Oct 2023 17:49:58 GMT  
		Size: 33.1 MB (33141653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30256924f5530cebc1ea042b5fde8499f912e388dc12580b7f4bfb886ed621b9`  
		Last Modified: Thu, 12 Oct 2023 12:31:24 GMT  
		Size: 104.5 MB (104525394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2d85d3edf39adfb61ceeaf1b92b4960089dd68c909e2f2668a96803ddb162b`  
		Last Modified: Thu, 12 Oct 2023 12:30:58 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4.1` - linux; s390x

```console
$ docker pull varnish@sha256:c16359d33b507ad0702a5be497bc4d3bf1dc9550a6b72a01fbfef0d10a15d9e3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112330094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd8caa54cdeafd2ed33943de55ef8effd990147fcb9b0311032a90892878efb1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:50:28 GMT
ADD file:b85ed0ed01200dd3626d66cf5205d989fc48e61b3dd3498f777ee72d91e64870 in / 
# Wed, 11 Oct 2023 17:50:30 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 00:48:18 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 12 Oct 2023 00:48:18 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 12 Oct 2023 00:48:18 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 12 Oct 2023 00:48:18 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 12 Oct 2023 00:48:19 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 12 Oct 2023 00:48:19 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 12 Oct 2023 00:48:19 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 12 Oct 2023 00:48:19 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 12 Oct 2023 00:48:19 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 12 Oct 2023 00:48:19 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Thu, 12 Oct 2023 00:48:19 GMT
ENV VARNISH_SIZE=100M
# Thu, 12 Oct 2023 01:06:58 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.1.tgz -o $tmpdir/orig.tgz;     echo "d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 12 Oct 2023 01:07:08 GMT
WORKDIR /etc/varnish
# Thu, 12 Oct 2023 01:07:08 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 12 Oct 2023 01:07:08 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 12 Oct 2023 01:07:08 GMT
USER varnish
# Thu, 12 Oct 2023 01:07:09 GMT
EXPOSE 80 8443
# Thu, 12 Oct 2023 01:07:09 GMT
CMD []
```

-	Layers:
	-	`sha256:f270c1bb05fa46b165ce3680225dc9fa5bbfe4d69420a467350e80f692c78eb2`  
		Last Modified: Wed, 11 Oct 2023 17:56:03 GMT  
		Size: 27.5 MB (27512850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1ecabb8eb208085a0cd1ccad185b3741ef91253ac090a644273393b03d5ba9`  
		Last Modified: Thu, 12 Oct 2023 01:15:40 GMT  
		Size: 84.8 MB (84816753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b8069a9787fb8bc5a96e8c2c9afaa0c689c46501adc3724923dd883a96e1fd7`  
		Last Modified: Thu, 12 Oct 2023 01:15:29 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.4.1-alpine`

```console
$ docker pull varnish@sha256:ecf79e7945d24f92b505735170fac696ead578391da5e81183bb814d058841d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:7.4.1-alpine` - linux; amd64

```console
$ docker pull varnish@sha256:8fd5e0d68a7bcb6c3a41155bb3b27a8cdc1ac3ebda8bc380de9b1448c958933b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (60984690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a672dc2e7c14234d749faf94e5af11adbc33c7f66fc1a0aebb3f95e34e893bb3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:20:37 GMT
ADD file:4faae297b6caba92e1791a5ff667be0fcb4de6a4de2df155395957ef9d8ad5e5 in / 
# Mon, 07 Aug 2023 19:20:37 GMT
CMD ["/bin/sh"]
# Mon, 18 Sep 2023 19:25:17 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 21 Sep 2023 10:03:06 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 21 Sep 2023 10:03:06 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 21 Sep 2023 10:03:06 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 21 Sep 2023 10:03:07 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 21 Sep 2023 10:03:07 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 21 Sep 2023 10:03:07 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 21 Sep 2023 10:03:07 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 21 Sep 2023 10:03:07 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 21 Sep 2023 10:03:07 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Thu, 21 Sep 2023 10:03:07 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Sep 2023 10:04:27 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Sep 2023 10:04:27 GMT
WORKDIR /etc/varnish
# Thu, 21 Sep 2023 10:04:27 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 21 Sep 2023 10:04:28 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Sep 2023 10:04:28 GMT
USER varnish
# Thu, 21 Sep 2023 10:04:28 GMT
EXPOSE 80 8443
# Thu, 21 Sep 2023 10:04:28 GMT
CMD []
```

-	Layers:
	-	`sha256:3695f6c099b80e503148dbb435d044c35147f81d34b9d6fbb27b3dcf1fd7ecaf`  
		Last Modified: Mon, 07 Aug 2023 19:21:27 GMT  
		Size: 2.8 MB (2826006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39051c6545f1b0c198fe83b7ffacdadb4c62c1a65bb4548192143c3c7a006ab`  
		Last Modified: Thu, 21 Sep 2023 10:08:31 GMT  
		Size: 58.2 MB (58158186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d139fff6dbe170e2eadf9014aa5ff95a6127606f4325169031bdc1f8c1b9c834`  
		Last Modified: Thu, 21 Sep 2023 10:08:23 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4.1-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:53f9b3af759587518f192eec1f3c70599bcea9f9eda6a87fbf32ba90f3fec2a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.3 MB (45251077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb9c94e956b808d696f8ad9a59e811e54a348f0230eba580630885aaee1ca603`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:57:37 GMT
ADD file:842dfa6e14e0537b53781830cfb26da9fa7a63229a7a1decc0fe08d8c000b5a9 in / 
# Mon, 07 Aug 2023 19:57:37 GMT
CMD ["/bin/sh"]
# Mon, 18 Sep 2023 20:16:10 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Wed, 20 Sep 2023 22:07:41 GMT
ARG VARNISH_VERSION=7.4.1
# Wed, 20 Sep 2023 22:07:41 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Wed, 20 Sep 2023 22:07:41 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 20 Sep 2023 22:07:41 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 20 Sep 2023 22:07:42 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Wed, 20 Sep 2023 22:07:42 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Wed, 20 Sep 2023 22:07:42 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Wed, 20 Sep 2023 22:07:42 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Wed, 20 Sep 2023 22:07:42 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Wed, 20 Sep 2023 22:07:43 GMT
ENV VARNISH_SIZE=100M
# Wed, 20 Sep 2023 22:10:33 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Wed, 20 Sep 2023 22:10:34 GMT
WORKDIR /etc/varnish
# Wed, 20 Sep 2023 22:10:34 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:10:34 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 20 Sep 2023 22:10:34 GMT
USER varnish
# Wed, 20 Sep 2023 22:10:35 GMT
EXPOSE 80 8443
# Wed, 20 Sep 2023 22:10:35 GMT
CMD []
```

-	Layers:
	-	`sha256:c25753df0ee4b6d3db1dacebcfb1839260ed067556f1f3ff52ddb574cab51045`  
		Last Modified: Mon, 07 Aug 2023 19:58:28 GMT  
		Size: 2.4 MB (2436761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3edaa1bb34a769d2a617d179c3a121ce323795b2d86f371adf2b18198108ff`  
		Last Modified: Wed, 20 Sep 2023 22:17:51 GMT  
		Size: 42.8 MB (42813817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571ba818c66eb7ccee714ee8e27bf848d97144ffa2ee3885ce0d1ba9bc5edf66`  
		Last Modified: Wed, 20 Sep 2023 22:17:46 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4.1-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:97de9f09c69852f96f7c296187539c50dea1aea1f5104e0c5c0c300ae8683af8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.2 MB (52224736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03377611cb0f40f9ce132047f83c95c50a27b27b11429d16a7be1312b16fa719`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:39:29 GMT
ADD file:21f240e1e33b25dacee7291cdd8c7750995aa0f460d13496a08c4a2dd92323aa in / 
# Mon, 07 Aug 2023 19:39:29 GMT
CMD ["/bin/sh"]
# Mon, 18 Sep 2023 19:52:54 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 21 Sep 2023 04:37:13 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 21 Sep 2023 04:37:13 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 21 Sep 2023 04:37:14 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 21 Sep 2023 04:37:14 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 21 Sep 2023 04:37:14 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 21 Sep 2023 04:37:14 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 21 Sep 2023 04:37:14 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 21 Sep 2023 04:37:14 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 21 Sep 2023 04:37:14 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Thu, 21 Sep 2023 04:37:14 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Sep 2023 04:38:26 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Sep 2023 04:38:27 GMT
WORKDIR /etc/varnish
# Thu, 21 Sep 2023 04:38:27 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 21 Sep 2023 04:38:27 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Sep 2023 04:38:27 GMT
USER varnish
# Thu, 21 Sep 2023 04:38:27 GMT
EXPOSE 80 8443
# Thu, 21 Sep 2023 04:38:27 GMT
CMD []
```

-	Layers:
	-	`sha256:ad3fa0ea069c04e4ee9be58cf0ae9e1a8a56f649b96a96298203b055e8c903ff`  
		Last Modified: Mon, 07 Aug 2023 19:40:16 GMT  
		Size: 2.7 MB (2720868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43115af36871113661de523d5f39c294c446e845b191847bee9039f91080b5e5`  
		Last Modified: Thu, 21 Sep 2023 04:41:44 GMT  
		Size: 49.5 MB (49503372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f08a4e7fb6fee04d2a988db665d17b65b17707f7325f9ec73cb624907e43a2`  
		Last Modified: Thu, 21 Sep 2023 04:41:38 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4.1-alpine` - linux; 386

```console
$ docker pull varnish@sha256:5aa6916b378447ac7ce3bce16083f21640ed77f346d9c6b6110232d87f9c8a01
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.1 MB (61137578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e205d190ad66189082289bc366ecf0ec42f35f54efea247d7e628253d2ba02c6`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:38:38 GMT
ADD file:2d8ac62dd229ef26536f5a9af9e61df30ea68d609fa969786dfd531aea18cf3c in / 
# Mon, 07 Aug 2023 19:38:38 GMT
CMD ["/bin/sh"]
# Mon, 18 Sep 2023 19:42:30 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 21 Sep 2023 02:30:06 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 21 Sep 2023 02:30:06 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 21 Sep 2023 02:30:06 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 21 Sep 2023 02:30:06 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 21 Sep 2023 02:30:06 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 21 Sep 2023 02:30:06 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 21 Sep 2023 02:30:07 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 21 Sep 2023 02:30:07 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 21 Sep 2023 02:30:07 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Thu, 21 Sep 2023 02:30:07 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Sep 2023 02:32:23 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Sep 2023 02:32:23 GMT
WORKDIR /etc/varnish
# Thu, 21 Sep 2023 02:32:24 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 21 Sep 2023 02:32:24 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Sep 2023 02:32:24 GMT
USER varnish
# Thu, 21 Sep 2023 02:32:24 GMT
EXPOSE 80 8443
# Thu, 21 Sep 2023 02:32:24 GMT
CMD []
```

-	Layers:
	-	`sha256:add53095769493cde9110fd91f113357e53b9e0d94abf216b811fcf00107674e`  
		Last Modified: Mon, 07 Aug 2023 19:39:29 GMT  
		Size: 2.8 MB (2832316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c150ec529b4641ae75ebddb680c40d4461ff6cb20cc9de9000d09e55c4cc77ae`  
		Last Modified: Thu, 21 Sep 2023 02:39:33 GMT  
		Size: 58.3 MB (58304764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d857ef55991e2baf89bc4c3c90d9b09873a4a3f98625ef9aff38572db418bdc`  
		Last Modified: Thu, 21 Sep 2023 02:39:22 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4.1-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:6e774ae86d3ccd908f2effc52757ac4d1253f3a19bc81f2aa0fe7bcff9aa1f1b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49267291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d42006d222979c85edb1b343cc64120bcfde800a88fe802c42c9983c8491b645`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 20:16:50 GMT
ADD file:f730d2cd05a420ffd38548ae1611345fc40a7db59dea5ff41328caa60ee42608 in / 
# Mon, 07 Aug 2023 20:16:51 GMT
CMD ["/bin/sh"]
# Mon, 18 Sep 2023 19:23:54 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 21 Sep 2023 01:05:18 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 21 Sep 2023 01:05:18 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 21 Sep 2023 01:05:18 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 21 Sep 2023 01:05:19 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 21 Sep 2023 01:05:19 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 21 Sep 2023 01:05:19 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 21 Sep 2023 01:05:19 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 21 Sep 2023 01:05:20 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 21 Sep 2023 01:05:20 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Thu, 21 Sep 2023 01:05:20 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Sep 2023 01:07:35 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Sep 2023 01:07:37 GMT
WORKDIR /etc/varnish
# Thu, 21 Sep 2023 01:07:37 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 21 Sep 2023 01:07:38 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Sep 2023 01:07:38 GMT
USER varnish
# Thu, 21 Sep 2023 01:07:38 GMT
EXPOSE 80 8443
# Thu, 21 Sep 2023 01:07:38 GMT
CMD []
```

-	Layers:
	-	`sha256:f1ecf55aa97fb0011a1c90ffc58e5cb218908bc85a13afe003aea5a46e045ac8`  
		Last Modified: Mon, 07 Aug 2023 20:18:07 GMT  
		Size: 2.8 MB (2812358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:487e7414b13c044e2fe3ed2d0c178b35a7c77da1716fd0f18713c4b30bf0e8e2`  
		Last Modified: Thu, 21 Sep 2023 01:18:59 GMT  
		Size: 46.5 MB (46454433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e361115526684bb9e4ffadc8f804eff285d2ec63f814fb32981a3580974deded`  
		Last Modified: Thu, 21 Sep 2023 01:18:48 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4.1-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:b098d4b1fdb99444ed73a7bbf08befce53f939ac48d20b65305b2819cbdbbe52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48935923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:357502947ec9a8ad3bdb2f0ed4673f3787524c7ebda92b216c258af34a941513`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:42:16 GMT
ADD file:db6cafb0897c5e32510edd0166d1e1b23001bef271dad57e4157d560bd09dd93 in / 
# Mon, 07 Aug 2023 19:42:16 GMT
CMD ["/bin/sh"]
# Mon, 18 Sep 2023 20:45:32 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 21 Sep 2023 01:49:29 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 21 Sep 2023 01:49:29 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 21 Sep 2023 01:49:29 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 21 Sep 2023 01:49:30 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 21 Sep 2023 01:49:30 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 21 Sep 2023 01:49:30 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 21 Sep 2023 01:49:30 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 21 Sep 2023 01:49:30 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 21 Sep 2023 01:49:30 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Thu, 21 Sep 2023 01:49:30 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Sep 2023 01:50:57 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Sep 2023 01:51:00 GMT
WORKDIR /etc/varnish
# Thu, 21 Sep 2023 01:51:00 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 21 Sep 2023 01:51:00 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Sep 2023 01:51:00 GMT
USER varnish
# Thu, 21 Sep 2023 01:51:00 GMT
EXPOSE 80 8443
# Thu, 21 Sep 2023 01:51:00 GMT
CMD []
```

-	Layers:
	-	`sha256:ec103030fda7a896185e8eb8a4f00b7f611725434956faa395cf74a993a2742e`  
		Last Modified: Mon, 07 Aug 2023 19:43:01 GMT  
		Size: 2.6 MB (2609002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c222777618072a84cbc1cc334e324f1cf6549d9aec24add4de60d61b25f04bf`  
		Last Modified: Thu, 21 Sep 2023 01:54:50 GMT  
		Size: 46.3 MB (46326423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f13e8e461de6c2bbbcf5890fd1669c82689bfea1ce6d63af764a6d281a801cf`  
		Last Modified: Thu, 21 Sep 2023 01:54:43 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:alpine`

```console
$ docker pull varnish@sha256:ecf79e7945d24f92b505735170fac696ead578391da5e81183bb814d058841d4
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
$ docker pull varnish@sha256:8fd5e0d68a7bcb6c3a41155bb3b27a8cdc1ac3ebda8bc380de9b1448c958933b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (60984690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a672dc2e7c14234d749faf94e5af11adbc33c7f66fc1a0aebb3f95e34e893bb3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:20:37 GMT
ADD file:4faae297b6caba92e1791a5ff667be0fcb4de6a4de2df155395957ef9d8ad5e5 in / 
# Mon, 07 Aug 2023 19:20:37 GMT
CMD ["/bin/sh"]
# Mon, 18 Sep 2023 19:25:17 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 21 Sep 2023 10:03:06 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 21 Sep 2023 10:03:06 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 21 Sep 2023 10:03:06 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 21 Sep 2023 10:03:07 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 21 Sep 2023 10:03:07 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 21 Sep 2023 10:03:07 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 21 Sep 2023 10:03:07 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 21 Sep 2023 10:03:07 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 21 Sep 2023 10:03:07 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Thu, 21 Sep 2023 10:03:07 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Sep 2023 10:04:27 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Sep 2023 10:04:27 GMT
WORKDIR /etc/varnish
# Thu, 21 Sep 2023 10:04:27 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 21 Sep 2023 10:04:28 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Sep 2023 10:04:28 GMT
USER varnish
# Thu, 21 Sep 2023 10:04:28 GMT
EXPOSE 80 8443
# Thu, 21 Sep 2023 10:04:28 GMT
CMD []
```

-	Layers:
	-	`sha256:3695f6c099b80e503148dbb435d044c35147f81d34b9d6fbb27b3dcf1fd7ecaf`  
		Last Modified: Mon, 07 Aug 2023 19:21:27 GMT  
		Size: 2.8 MB (2826006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39051c6545f1b0c198fe83b7ffacdadb4c62c1a65bb4548192143c3c7a006ab`  
		Last Modified: Thu, 21 Sep 2023 10:08:31 GMT  
		Size: 58.2 MB (58158186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d139fff6dbe170e2eadf9014aa5ff95a6127606f4325169031bdc1f8c1b9c834`  
		Last Modified: Thu, 21 Sep 2023 10:08:23 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:53f9b3af759587518f192eec1f3c70599bcea9f9eda6a87fbf32ba90f3fec2a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.3 MB (45251077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb9c94e956b808d696f8ad9a59e811e54a348f0230eba580630885aaee1ca603`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:57:37 GMT
ADD file:842dfa6e14e0537b53781830cfb26da9fa7a63229a7a1decc0fe08d8c000b5a9 in / 
# Mon, 07 Aug 2023 19:57:37 GMT
CMD ["/bin/sh"]
# Mon, 18 Sep 2023 20:16:10 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Wed, 20 Sep 2023 22:07:41 GMT
ARG VARNISH_VERSION=7.4.1
# Wed, 20 Sep 2023 22:07:41 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Wed, 20 Sep 2023 22:07:41 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 20 Sep 2023 22:07:41 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 20 Sep 2023 22:07:42 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Wed, 20 Sep 2023 22:07:42 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Wed, 20 Sep 2023 22:07:42 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Wed, 20 Sep 2023 22:07:42 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Wed, 20 Sep 2023 22:07:42 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Wed, 20 Sep 2023 22:07:43 GMT
ENV VARNISH_SIZE=100M
# Wed, 20 Sep 2023 22:10:33 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Wed, 20 Sep 2023 22:10:34 GMT
WORKDIR /etc/varnish
# Wed, 20 Sep 2023 22:10:34 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:10:34 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 20 Sep 2023 22:10:34 GMT
USER varnish
# Wed, 20 Sep 2023 22:10:35 GMT
EXPOSE 80 8443
# Wed, 20 Sep 2023 22:10:35 GMT
CMD []
```

-	Layers:
	-	`sha256:c25753df0ee4b6d3db1dacebcfb1839260ed067556f1f3ff52ddb574cab51045`  
		Last Modified: Mon, 07 Aug 2023 19:58:28 GMT  
		Size: 2.4 MB (2436761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3edaa1bb34a769d2a617d179c3a121ce323795b2d86f371adf2b18198108ff`  
		Last Modified: Wed, 20 Sep 2023 22:17:51 GMT  
		Size: 42.8 MB (42813817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571ba818c66eb7ccee714ee8e27bf848d97144ffa2ee3885ce0d1ba9bc5edf66`  
		Last Modified: Wed, 20 Sep 2023 22:17:46 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:97de9f09c69852f96f7c296187539c50dea1aea1f5104e0c5c0c300ae8683af8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.2 MB (52224736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03377611cb0f40f9ce132047f83c95c50a27b27b11429d16a7be1312b16fa719`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:39:29 GMT
ADD file:21f240e1e33b25dacee7291cdd8c7750995aa0f460d13496a08c4a2dd92323aa in / 
# Mon, 07 Aug 2023 19:39:29 GMT
CMD ["/bin/sh"]
# Mon, 18 Sep 2023 19:52:54 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 21 Sep 2023 04:37:13 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 21 Sep 2023 04:37:13 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 21 Sep 2023 04:37:14 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 21 Sep 2023 04:37:14 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 21 Sep 2023 04:37:14 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 21 Sep 2023 04:37:14 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 21 Sep 2023 04:37:14 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 21 Sep 2023 04:37:14 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 21 Sep 2023 04:37:14 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Thu, 21 Sep 2023 04:37:14 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Sep 2023 04:38:26 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Sep 2023 04:38:27 GMT
WORKDIR /etc/varnish
# Thu, 21 Sep 2023 04:38:27 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 21 Sep 2023 04:38:27 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Sep 2023 04:38:27 GMT
USER varnish
# Thu, 21 Sep 2023 04:38:27 GMT
EXPOSE 80 8443
# Thu, 21 Sep 2023 04:38:27 GMT
CMD []
```

-	Layers:
	-	`sha256:ad3fa0ea069c04e4ee9be58cf0ae9e1a8a56f649b96a96298203b055e8c903ff`  
		Last Modified: Mon, 07 Aug 2023 19:40:16 GMT  
		Size: 2.7 MB (2720868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43115af36871113661de523d5f39c294c446e845b191847bee9039f91080b5e5`  
		Last Modified: Thu, 21 Sep 2023 04:41:44 GMT  
		Size: 49.5 MB (49503372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f08a4e7fb6fee04d2a988db665d17b65b17707f7325f9ec73cb624907e43a2`  
		Last Modified: Thu, 21 Sep 2023 04:41:38 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; 386

```console
$ docker pull varnish@sha256:5aa6916b378447ac7ce3bce16083f21640ed77f346d9c6b6110232d87f9c8a01
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.1 MB (61137578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e205d190ad66189082289bc366ecf0ec42f35f54efea247d7e628253d2ba02c6`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:38:38 GMT
ADD file:2d8ac62dd229ef26536f5a9af9e61df30ea68d609fa969786dfd531aea18cf3c in / 
# Mon, 07 Aug 2023 19:38:38 GMT
CMD ["/bin/sh"]
# Mon, 18 Sep 2023 19:42:30 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 21 Sep 2023 02:30:06 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 21 Sep 2023 02:30:06 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 21 Sep 2023 02:30:06 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 21 Sep 2023 02:30:06 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 21 Sep 2023 02:30:06 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 21 Sep 2023 02:30:06 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 21 Sep 2023 02:30:07 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 21 Sep 2023 02:30:07 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 21 Sep 2023 02:30:07 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Thu, 21 Sep 2023 02:30:07 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Sep 2023 02:32:23 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Sep 2023 02:32:23 GMT
WORKDIR /etc/varnish
# Thu, 21 Sep 2023 02:32:24 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 21 Sep 2023 02:32:24 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Sep 2023 02:32:24 GMT
USER varnish
# Thu, 21 Sep 2023 02:32:24 GMT
EXPOSE 80 8443
# Thu, 21 Sep 2023 02:32:24 GMT
CMD []
```

-	Layers:
	-	`sha256:add53095769493cde9110fd91f113357e53b9e0d94abf216b811fcf00107674e`  
		Last Modified: Mon, 07 Aug 2023 19:39:29 GMT  
		Size: 2.8 MB (2832316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c150ec529b4641ae75ebddb680c40d4461ff6cb20cc9de9000d09e55c4cc77ae`  
		Last Modified: Thu, 21 Sep 2023 02:39:33 GMT  
		Size: 58.3 MB (58304764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d857ef55991e2baf89bc4c3c90d9b09873a4a3f98625ef9aff38572db418bdc`  
		Last Modified: Thu, 21 Sep 2023 02:39:22 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:6e774ae86d3ccd908f2effc52757ac4d1253f3a19bc81f2aa0fe7bcff9aa1f1b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49267291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d42006d222979c85edb1b343cc64120bcfde800a88fe802c42c9983c8491b645`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 20:16:50 GMT
ADD file:f730d2cd05a420ffd38548ae1611345fc40a7db59dea5ff41328caa60ee42608 in / 
# Mon, 07 Aug 2023 20:16:51 GMT
CMD ["/bin/sh"]
# Mon, 18 Sep 2023 19:23:54 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 21 Sep 2023 01:05:18 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 21 Sep 2023 01:05:18 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 21 Sep 2023 01:05:18 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 21 Sep 2023 01:05:19 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 21 Sep 2023 01:05:19 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 21 Sep 2023 01:05:19 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 21 Sep 2023 01:05:19 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 21 Sep 2023 01:05:20 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 21 Sep 2023 01:05:20 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Thu, 21 Sep 2023 01:05:20 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Sep 2023 01:07:35 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Sep 2023 01:07:37 GMT
WORKDIR /etc/varnish
# Thu, 21 Sep 2023 01:07:37 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 21 Sep 2023 01:07:38 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Sep 2023 01:07:38 GMT
USER varnish
# Thu, 21 Sep 2023 01:07:38 GMT
EXPOSE 80 8443
# Thu, 21 Sep 2023 01:07:38 GMT
CMD []
```

-	Layers:
	-	`sha256:f1ecf55aa97fb0011a1c90ffc58e5cb218908bc85a13afe003aea5a46e045ac8`  
		Last Modified: Mon, 07 Aug 2023 20:18:07 GMT  
		Size: 2.8 MB (2812358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:487e7414b13c044e2fe3ed2d0c178b35a7c77da1716fd0f18713c4b30bf0e8e2`  
		Last Modified: Thu, 21 Sep 2023 01:18:59 GMT  
		Size: 46.5 MB (46454433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e361115526684bb9e4ffadc8f804eff285d2ec63f814fb32981a3580974deded`  
		Last Modified: Thu, 21 Sep 2023 01:18:48 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; s390x

```console
$ docker pull varnish@sha256:b098d4b1fdb99444ed73a7bbf08befce53f939ac48d20b65305b2819cbdbbe52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48935923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:357502947ec9a8ad3bdb2f0ed4673f3787524c7ebda92b216c258af34a941513`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:42:16 GMT
ADD file:db6cafb0897c5e32510edd0166d1e1b23001bef271dad57e4157d560bd09dd93 in / 
# Mon, 07 Aug 2023 19:42:16 GMT
CMD ["/bin/sh"]
# Mon, 18 Sep 2023 20:45:32 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 21 Sep 2023 01:49:29 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 21 Sep 2023 01:49:29 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 21 Sep 2023 01:49:29 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 21 Sep 2023 01:49:30 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 21 Sep 2023 01:49:30 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 21 Sep 2023 01:49:30 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 21 Sep 2023 01:49:30 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 21 Sep 2023 01:49:30 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 21 Sep 2023 01:49:30 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Thu, 21 Sep 2023 01:49:30 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Sep 2023 01:50:57 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Sep 2023 01:51:00 GMT
WORKDIR /etc/varnish
# Thu, 21 Sep 2023 01:51:00 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 21 Sep 2023 01:51:00 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Sep 2023 01:51:00 GMT
USER varnish
# Thu, 21 Sep 2023 01:51:00 GMT
EXPOSE 80 8443
# Thu, 21 Sep 2023 01:51:00 GMT
CMD []
```

-	Layers:
	-	`sha256:ec103030fda7a896185e8eb8a4f00b7f611725434956faa395cf74a993a2742e`  
		Last Modified: Mon, 07 Aug 2023 19:43:01 GMT  
		Size: 2.6 MB (2609002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c222777618072a84cbc1cc334e324f1cf6549d9aec24add4de60d61b25f04bf`  
		Last Modified: Thu, 21 Sep 2023 01:54:50 GMT  
		Size: 46.3 MB (46326423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f13e8e461de6c2bbbcf5890fd1669c82689bfea1ce6d63af764a6d281a801cf`  
		Last Modified: Thu, 21 Sep 2023 01:54:43 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:fresh`

```console
$ docker pull varnish@sha256:8aebb0e2fdb98f8c8f08529f42264f599ce08a7ab0179236767aebaaa62d6d7e
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
$ docker pull varnish@sha256:e03566ef6752192c478b1aa7bba603dc26f1ee563934c03f28e9c6a7a5396d59
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134737591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:266771d9cf5c42149096e6813c1b152608a114703951e87c69ce3220c862ab70`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 18:34:50 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 11 Oct 2023 18:34:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:27:13 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Wed, 11 Oct 2023 21:27:13 GMT
ARG VARNISH_VERSION=7.4.1
# Wed, 11 Oct 2023 21:27:13 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Wed, 11 Oct 2023 21:27:14 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 11 Oct 2023 21:27:14 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 11 Oct 2023 21:27:14 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Wed, 11 Oct 2023 21:27:14 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Wed, 11 Oct 2023 21:27:14 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Wed, 11 Oct 2023 21:27:14 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Wed, 11 Oct 2023 21:27:14 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Wed, 11 Oct 2023 21:27:14 GMT
ENV VARNISH_SIZE=100M
# Wed, 11 Oct 2023 21:30:00 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.1.tgz -o $tmpdir/orig.tgz;     echo "d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 11 Oct 2023 21:30:01 GMT
WORKDIR /etc/varnish
# Wed, 11 Oct 2023 21:30:01 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 11 Oct 2023 21:30:01 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 11 Oct 2023 21:30:01 GMT
USER varnish
# Wed, 11 Oct 2023 21:30:01 GMT
EXPOSE 80 8443
# Wed, 11 Oct 2023 21:30:01 GMT
CMD []
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73d3b02baeacb05096f1d533167545798575b4b39a4f516a201ad8a3c0fd9e0`  
		Last Modified: Wed, 11 Oct 2023 21:35:14 GMT  
		Size: 105.6 MB (105587228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c88afe6700045cede25a79c7cae3b4fd9c2630ea13c3445c62ee292dc732123`  
		Last Modified: Wed, 11 Oct 2023 21:34:59 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; arm variant v7

```console
$ docker pull varnish@sha256:1feecff1374e6c3d603761b67362c81d8a15190b4fce34911d6257281a848cad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105036990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91cb20c34e8cd2ad07e5e4d7fb9e378a81db336a803bd894fda058508b99013f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:42:11 GMT
ADD file:da08fed31a161a2210fd920a1b5e43aa3f4199985cdeaa0d5d24c0a0f19044aa in / 
# Wed, 11 Oct 2023 17:42:11 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:09:22 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Wed, 11 Oct 2023 18:09:22 GMT
ARG VARNISH_VERSION=7.4.1
# Wed, 11 Oct 2023 18:09:22 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Wed, 11 Oct 2023 18:09:22 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 11 Oct 2023 18:09:22 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 11 Oct 2023 18:09:22 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Wed, 11 Oct 2023 18:09:22 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Wed, 11 Oct 2023 18:09:22 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Wed, 11 Oct 2023 18:09:22 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Wed, 11 Oct 2023 18:09:22 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Wed, 11 Oct 2023 18:09:23 GMT
ENV VARNISH_SIZE=100M
# Wed, 11 Oct 2023 18:12:11 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.1.tgz -o $tmpdir/orig.tgz;     echo "d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 11 Oct 2023 18:12:12 GMT
WORKDIR /etc/varnish
# Wed, 11 Oct 2023 18:12:12 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 11 Oct 2023 18:12:12 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 11 Oct 2023 18:12:12 GMT
USER varnish
# Wed, 11 Oct 2023 18:12:12 GMT
EXPOSE 80 8443
# Wed, 11 Oct 2023 18:12:12 GMT
CMD []
```

-	Layers:
	-	`sha256:2f11c34abc7b59f09b58bb6e2cf54f260f4b4142ecf8023a114e281ea4b532d1`  
		Last Modified: Wed, 11 Oct 2023 17:46:22 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3d75364756f4e459e71b5941b35371acb082f8bb2f09c42230d48ff70cfa56`  
		Last Modified: Wed, 11 Oct 2023 18:17:46 GMT  
		Size: 80.3 MB (80287576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd120edc727486131696ee7b8fb97154d80d4812e8c1865198e8b909d2e8e457`  
		Last Modified: Wed, 11 Oct 2023 18:17:34 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:472bd27e1d4a42daf22c320d58944cf4ea8243a2a3dd9300e1cb7b76264bedda
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.2 MB (129197485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6368c63db1f983c26740d4676cf9ae4da73811320dd0f21fabf6191e6e872ca`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 20 Sep 2023 02:44:13 GMT
ADD file:ec1a6e0aedd76c8fdc8544775f8b553f58950e9435f5cfe919f39374e222cfbb in / 
# Wed, 20 Sep 2023 02:44:14 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 17:48:56 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 21 Sep 2023 04:34:35 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 21 Sep 2023 04:34:36 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 21 Sep 2023 04:34:36 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 21 Sep 2023 04:34:36 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 21 Sep 2023 04:34:36 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 21 Sep 2023 04:34:36 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 21 Sep 2023 04:34:36 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 21 Sep 2023 04:34:36 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 21 Sep 2023 04:34:36 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Thu, 21 Sep 2023 04:34:36 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Sep 2023 04:37:04 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.1.tgz -o $tmpdir/orig.tgz;     echo "d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 21 Sep 2023 04:37:06 GMT
WORKDIR /etc/varnish
# Thu, 21 Sep 2023 04:37:06 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 21 Sep 2023 04:37:06 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Sep 2023 04:37:06 GMT
USER varnish
# Thu, 21 Sep 2023 04:37:06 GMT
EXPOSE 80 8443
# Thu, 21 Sep 2023 04:37:06 GMT
CMD []
```

-	Layers:
	-	`sha256:e886f0f47ef56fcadb6ecaf2116056bbdb273e0afe07ed034498b198d386c04e`  
		Last Modified: Wed, 20 Sep 2023 02:47:36 GMT  
		Size: 29.2 MB (29157221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d168552ad41a2f9b1ae51e74b416a1fbf5f899631badf1ecf74bb5962f131c8`  
		Last Modified: Thu, 21 Sep 2023 04:41:26 GMT  
		Size: 100.0 MB (100039772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aee0db284127fd79a1e633f9ee036d58c5817770e41d69607d88963d53c073f`  
		Last Modified: Thu, 21 Sep 2023 04:41:15 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; 386

```console
$ docker pull varnish@sha256:b0b281bd04e70c06c4d95562ddc165603c7fcb63797a5307ea577d0854a46ba0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131877976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8763c9a49d7d742b60afd31d81ea0e3816bba8e58111f0d3bfc26b36fc3c66f5`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:40:42 GMT
ADD file:31318c1b1f05d559cce42f5b12eef97d916932217e0b987fb07c0fc11bf0a14a in / 
# Wed, 11 Oct 2023 17:40:42 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 08:38:19 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 12 Oct 2023 08:38:19 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 12 Oct 2023 08:38:20 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 12 Oct 2023 08:38:20 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 12 Oct 2023 08:38:20 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 12 Oct 2023 08:38:20 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 12 Oct 2023 08:38:20 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 12 Oct 2023 08:38:20 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 12 Oct 2023 08:38:20 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 12 Oct 2023 08:38:20 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Thu, 12 Oct 2023 08:38:20 GMT
ENV VARNISH_SIZE=100M
# Thu, 12 Oct 2023 08:42:04 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.1.tgz -o $tmpdir/orig.tgz;     echo "d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 12 Oct 2023 08:42:05 GMT
WORKDIR /etc/varnish
# Thu, 12 Oct 2023 08:42:05 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 12 Oct 2023 08:42:05 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 12 Oct 2023 08:42:06 GMT
USER varnish
# Thu, 12 Oct 2023 08:42:06 GMT
EXPOSE 80 8443
# Thu, 12 Oct 2023 08:42:06 GMT
CMD []
```

-	Layers:
	-	`sha256:b27d0f1369837277a82877763487cdd2535037988fc27e16f11cf74e103ae4cd`  
		Last Modified: Wed, 11 Oct 2023 17:45:31 GMT  
		Size: 30.2 MB (30164118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4d7224a6538ed66733bc96ac79177a58d0039e0e68594173cc295e2ea9b504`  
		Last Modified: Thu, 12 Oct 2023 08:48:35 GMT  
		Size: 101.7 MB (101713366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:621ed1744001a5b482de115c1a397507d44f792c45cdd41dce56ecb1fca9cbe3`  
		Last Modified: Thu, 12 Oct 2023 08:48:15 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; ppc64le

```console
$ docker pull varnish@sha256:180fe86166e9d0d3b446cedb5e1b6b04f386a146b06c3e5faa0c574866f91999
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.7 MB (137667538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b6eb4c889e8ef2ee0187d1b231a86f99e559d96be323785f2739b97ea92f83d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:44:19 GMT
ADD file:53c83bdd58e7c4003ae769596cc2f8e6b72c0bbb854dbe7f006a39f273848b1b in / 
# Wed, 11 Oct 2023 17:44:21 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 12:12:26 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 12 Oct 2023 12:12:27 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 12 Oct 2023 12:12:27 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 12 Oct 2023 12:12:27 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 12 Oct 2023 12:12:28 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 12 Oct 2023 12:12:28 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 12 Oct 2023 12:12:29 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 12 Oct 2023 12:12:29 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 12 Oct 2023 12:12:29 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 12 Oct 2023 12:12:30 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Thu, 12 Oct 2023 12:12:30 GMT
ENV VARNISH_SIZE=100M
# Thu, 12 Oct 2023 12:19:14 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.1.tgz -o $tmpdir/orig.tgz;     echo "d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 12 Oct 2023 12:19:21 GMT
WORKDIR /etc/varnish
# Thu, 12 Oct 2023 12:19:21 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 12 Oct 2023 12:19:22 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 12 Oct 2023 12:19:22 GMT
USER varnish
# Thu, 12 Oct 2023 12:19:23 GMT
EXPOSE 80 8443
# Thu, 12 Oct 2023 12:19:24 GMT
CMD []
```

-	Layers:
	-	`sha256:54813908ce8a5d8a81f2db88ad0366eb5266484c7c402e5e93ef26e764f7a0e2`  
		Last Modified: Wed, 11 Oct 2023 17:49:58 GMT  
		Size: 33.1 MB (33141653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30256924f5530cebc1ea042b5fde8499f912e388dc12580b7f4bfb886ed621b9`  
		Last Modified: Thu, 12 Oct 2023 12:31:24 GMT  
		Size: 104.5 MB (104525394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2d85d3edf39adfb61ceeaf1b92b4960089dd68c909e2f2668a96803ddb162b`  
		Last Modified: Thu, 12 Oct 2023 12:30:58 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; s390x

```console
$ docker pull varnish@sha256:c16359d33b507ad0702a5be497bc4d3bf1dc9550a6b72a01fbfef0d10a15d9e3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112330094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd8caa54cdeafd2ed33943de55ef8effd990147fcb9b0311032a90892878efb1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:50:28 GMT
ADD file:b85ed0ed01200dd3626d66cf5205d989fc48e61b3dd3498f777ee72d91e64870 in / 
# Wed, 11 Oct 2023 17:50:30 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 00:48:18 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 12 Oct 2023 00:48:18 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 12 Oct 2023 00:48:18 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 12 Oct 2023 00:48:18 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 12 Oct 2023 00:48:19 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 12 Oct 2023 00:48:19 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 12 Oct 2023 00:48:19 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 12 Oct 2023 00:48:19 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 12 Oct 2023 00:48:19 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 12 Oct 2023 00:48:19 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Thu, 12 Oct 2023 00:48:19 GMT
ENV VARNISH_SIZE=100M
# Thu, 12 Oct 2023 01:06:58 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.1.tgz -o $tmpdir/orig.tgz;     echo "d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 12 Oct 2023 01:07:08 GMT
WORKDIR /etc/varnish
# Thu, 12 Oct 2023 01:07:08 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 12 Oct 2023 01:07:08 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 12 Oct 2023 01:07:08 GMT
USER varnish
# Thu, 12 Oct 2023 01:07:09 GMT
EXPOSE 80 8443
# Thu, 12 Oct 2023 01:07:09 GMT
CMD []
```

-	Layers:
	-	`sha256:f270c1bb05fa46b165ce3680225dc9fa5bbfe4d69420a467350e80f692c78eb2`  
		Last Modified: Wed, 11 Oct 2023 17:56:03 GMT  
		Size: 27.5 MB (27512850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1ecabb8eb208085a0cd1ccad185b3741ef91253ac090a644273393b03d5ba9`  
		Last Modified: Thu, 12 Oct 2023 01:15:40 GMT  
		Size: 84.8 MB (84816753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b8069a9787fb8bc5a96e8c2c9afaa0c689c46501adc3724923dd883a96e1fd7`  
		Last Modified: Thu, 12 Oct 2023 01:15:29 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:fresh-alpine`

```console
$ docker pull varnish@sha256:ecf79e7945d24f92b505735170fac696ead578391da5e81183bb814d058841d4
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
$ docker pull varnish@sha256:8fd5e0d68a7bcb6c3a41155bb3b27a8cdc1ac3ebda8bc380de9b1448c958933b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (60984690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a672dc2e7c14234d749faf94e5af11adbc33c7f66fc1a0aebb3f95e34e893bb3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:20:37 GMT
ADD file:4faae297b6caba92e1791a5ff667be0fcb4de6a4de2df155395957ef9d8ad5e5 in / 
# Mon, 07 Aug 2023 19:20:37 GMT
CMD ["/bin/sh"]
# Mon, 18 Sep 2023 19:25:17 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 21 Sep 2023 10:03:06 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 21 Sep 2023 10:03:06 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 21 Sep 2023 10:03:06 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 21 Sep 2023 10:03:07 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 21 Sep 2023 10:03:07 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 21 Sep 2023 10:03:07 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 21 Sep 2023 10:03:07 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 21 Sep 2023 10:03:07 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 21 Sep 2023 10:03:07 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Thu, 21 Sep 2023 10:03:07 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Sep 2023 10:04:27 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Sep 2023 10:04:27 GMT
WORKDIR /etc/varnish
# Thu, 21 Sep 2023 10:04:27 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 21 Sep 2023 10:04:28 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Sep 2023 10:04:28 GMT
USER varnish
# Thu, 21 Sep 2023 10:04:28 GMT
EXPOSE 80 8443
# Thu, 21 Sep 2023 10:04:28 GMT
CMD []
```

-	Layers:
	-	`sha256:3695f6c099b80e503148dbb435d044c35147f81d34b9d6fbb27b3dcf1fd7ecaf`  
		Last Modified: Mon, 07 Aug 2023 19:21:27 GMT  
		Size: 2.8 MB (2826006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39051c6545f1b0c198fe83b7ffacdadb4c62c1a65bb4548192143c3c7a006ab`  
		Last Modified: Thu, 21 Sep 2023 10:08:31 GMT  
		Size: 58.2 MB (58158186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d139fff6dbe170e2eadf9014aa5ff95a6127606f4325169031bdc1f8c1b9c834`  
		Last Modified: Thu, 21 Sep 2023 10:08:23 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:53f9b3af759587518f192eec1f3c70599bcea9f9eda6a87fbf32ba90f3fec2a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.3 MB (45251077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb9c94e956b808d696f8ad9a59e811e54a348f0230eba580630885aaee1ca603`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:57:37 GMT
ADD file:842dfa6e14e0537b53781830cfb26da9fa7a63229a7a1decc0fe08d8c000b5a9 in / 
# Mon, 07 Aug 2023 19:57:37 GMT
CMD ["/bin/sh"]
# Mon, 18 Sep 2023 20:16:10 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Wed, 20 Sep 2023 22:07:41 GMT
ARG VARNISH_VERSION=7.4.1
# Wed, 20 Sep 2023 22:07:41 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Wed, 20 Sep 2023 22:07:41 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 20 Sep 2023 22:07:41 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 20 Sep 2023 22:07:42 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Wed, 20 Sep 2023 22:07:42 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Wed, 20 Sep 2023 22:07:42 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Wed, 20 Sep 2023 22:07:42 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Wed, 20 Sep 2023 22:07:42 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Wed, 20 Sep 2023 22:07:43 GMT
ENV VARNISH_SIZE=100M
# Wed, 20 Sep 2023 22:10:33 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Wed, 20 Sep 2023 22:10:34 GMT
WORKDIR /etc/varnish
# Wed, 20 Sep 2023 22:10:34 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:10:34 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 20 Sep 2023 22:10:34 GMT
USER varnish
# Wed, 20 Sep 2023 22:10:35 GMT
EXPOSE 80 8443
# Wed, 20 Sep 2023 22:10:35 GMT
CMD []
```

-	Layers:
	-	`sha256:c25753df0ee4b6d3db1dacebcfb1839260ed067556f1f3ff52ddb574cab51045`  
		Last Modified: Mon, 07 Aug 2023 19:58:28 GMT  
		Size: 2.4 MB (2436761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3edaa1bb34a769d2a617d179c3a121ce323795b2d86f371adf2b18198108ff`  
		Last Modified: Wed, 20 Sep 2023 22:17:51 GMT  
		Size: 42.8 MB (42813817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571ba818c66eb7ccee714ee8e27bf848d97144ffa2ee3885ce0d1ba9bc5edf66`  
		Last Modified: Wed, 20 Sep 2023 22:17:46 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:97de9f09c69852f96f7c296187539c50dea1aea1f5104e0c5c0c300ae8683af8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.2 MB (52224736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03377611cb0f40f9ce132047f83c95c50a27b27b11429d16a7be1312b16fa719`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:39:29 GMT
ADD file:21f240e1e33b25dacee7291cdd8c7750995aa0f460d13496a08c4a2dd92323aa in / 
# Mon, 07 Aug 2023 19:39:29 GMT
CMD ["/bin/sh"]
# Mon, 18 Sep 2023 19:52:54 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 21 Sep 2023 04:37:13 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 21 Sep 2023 04:37:13 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 21 Sep 2023 04:37:14 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 21 Sep 2023 04:37:14 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 21 Sep 2023 04:37:14 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 21 Sep 2023 04:37:14 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 21 Sep 2023 04:37:14 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 21 Sep 2023 04:37:14 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 21 Sep 2023 04:37:14 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Thu, 21 Sep 2023 04:37:14 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Sep 2023 04:38:26 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Sep 2023 04:38:27 GMT
WORKDIR /etc/varnish
# Thu, 21 Sep 2023 04:38:27 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 21 Sep 2023 04:38:27 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Sep 2023 04:38:27 GMT
USER varnish
# Thu, 21 Sep 2023 04:38:27 GMT
EXPOSE 80 8443
# Thu, 21 Sep 2023 04:38:27 GMT
CMD []
```

-	Layers:
	-	`sha256:ad3fa0ea069c04e4ee9be58cf0ae9e1a8a56f649b96a96298203b055e8c903ff`  
		Last Modified: Mon, 07 Aug 2023 19:40:16 GMT  
		Size: 2.7 MB (2720868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43115af36871113661de523d5f39c294c446e845b191847bee9039f91080b5e5`  
		Last Modified: Thu, 21 Sep 2023 04:41:44 GMT  
		Size: 49.5 MB (49503372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f08a4e7fb6fee04d2a988db665d17b65b17707f7325f9ec73cb624907e43a2`  
		Last Modified: Thu, 21 Sep 2023 04:41:38 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; 386

```console
$ docker pull varnish@sha256:5aa6916b378447ac7ce3bce16083f21640ed77f346d9c6b6110232d87f9c8a01
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.1 MB (61137578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e205d190ad66189082289bc366ecf0ec42f35f54efea247d7e628253d2ba02c6`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:38:38 GMT
ADD file:2d8ac62dd229ef26536f5a9af9e61df30ea68d609fa969786dfd531aea18cf3c in / 
# Mon, 07 Aug 2023 19:38:38 GMT
CMD ["/bin/sh"]
# Mon, 18 Sep 2023 19:42:30 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 21 Sep 2023 02:30:06 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 21 Sep 2023 02:30:06 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 21 Sep 2023 02:30:06 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 21 Sep 2023 02:30:06 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 21 Sep 2023 02:30:06 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 21 Sep 2023 02:30:06 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 21 Sep 2023 02:30:07 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 21 Sep 2023 02:30:07 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 21 Sep 2023 02:30:07 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Thu, 21 Sep 2023 02:30:07 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Sep 2023 02:32:23 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Sep 2023 02:32:23 GMT
WORKDIR /etc/varnish
# Thu, 21 Sep 2023 02:32:24 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 21 Sep 2023 02:32:24 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Sep 2023 02:32:24 GMT
USER varnish
# Thu, 21 Sep 2023 02:32:24 GMT
EXPOSE 80 8443
# Thu, 21 Sep 2023 02:32:24 GMT
CMD []
```

-	Layers:
	-	`sha256:add53095769493cde9110fd91f113357e53b9e0d94abf216b811fcf00107674e`  
		Last Modified: Mon, 07 Aug 2023 19:39:29 GMT  
		Size: 2.8 MB (2832316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c150ec529b4641ae75ebddb680c40d4461ff6cb20cc9de9000d09e55c4cc77ae`  
		Last Modified: Thu, 21 Sep 2023 02:39:33 GMT  
		Size: 58.3 MB (58304764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d857ef55991e2baf89bc4c3c90d9b09873a4a3f98625ef9aff38572db418bdc`  
		Last Modified: Thu, 21 Sep 2023 02:39:22 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:6e774ae86d3ccd908f2effc52757ac4d1253f3a19bc81f2aa0fe7bcff9aa1f1b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49267291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d42006d222979c85edb1b343cc64120bcfde800a88fe802c42c9983c8491b645`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 20:16:50 GMT
ADD file:f730d2cd05a420ffd38548ae1611345fc40a7db59dea5ff41328caa60ee42608 in / 
# Mon, 07 Aug 2023 20:16:51 GMT
CMD ["/bin/sh"]
# Mon, 18 Sep 2023 19:23:54 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 21 Sep 2023 01:05:18 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 21 Sep 2023 01:05:18 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 21 Sep 2023 01:05:18 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 21 Sep 2023 01:05:19 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 21 Sep 2023 01:05:19 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 21 Sep 2023 01:05:19 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 21 Sep 2023 01:05:19 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 21 Sep 2023 01:05:20 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 21 Sep 2023 01:05:20 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Thu, 21 Sep 2023 01:05:20 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Sep 2023 01:07:35 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Sep 2023 01:07:37 GMT
WORKDIR /etc/varnish
# Thu, 21 Sep 2023 01:07:37 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 21 Sep 2023 01:07:38 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Sep 2023 01:07:38 GMT
USER varnish
# Thu, 21 Sep 2023 01:07:38 GMT
EXPOSE 80 8443
# Thu, 21 Sep 2023 01:07:38 GMT
CMD []
```

-	Layers:
	-	`sha256:f1ecf55aa97fb0011a1c90ffc58e5cb218908bc85a13afe003aea5a46e045ac8`  
		Last Modified: Mon, 07 Aug 2023 20:18:07 GMT  
		Size: 2.8 MB (2812358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:487e7414b13c044e2fe3ed2d0c178b35a7c77da1716fd0f18713c4b30bf0e8e2`  
		Last Modified: Thu, 21 Sep 2023 01:18:59 GMT  
		Size: 46.5 MB (46454433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e361115526684bb9e4ffadc8f804eff285d2ec63f814fb32981a3580974deded`  
		Last Modified: Thu, 21 Sep 2023 01:18:48 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:b098d4b1fdb99444ed73a7bbf08befce53f939ac48d20b65305b2819cbdbbe52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48935923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:357502947ec9a8ad3bdb2f0ed4673f3787524c7ebda92b216c258af34a941513`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:42:16 GMT
ADD file:db6cafb0897c5e32510edd0166d1e1b23001bef271dad57e4157d560bd09dd93 in / 
# Mon, 07 Aug 2023 19:42:16 GMT
CMD ["/bin/sh"]
# Mon, 18 Sep 2023 20:45:32 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 21 Sep 2023 01:49:29 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 21 Sep 2023 01:49:29 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 21 Sep 2023 01:49:29 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 21 Sep 2023 01:49:30 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 21 Sep 2023 01:49:30 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 21 Sep 2023 01:49:30 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 21 Sep 2023 01:49:30 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 21 Sep 2023 01:49:30 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 21 Sep 2023 01:49:30 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Thu, 21 Sep 2023 01:49:30 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Sep 2023 01:50:57 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Sep 2023 01:51:00 GMT
WORKDIR /etc/varnish
# Thu, 21 Sep 2023 01:51:00 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 21 Sep 2023 01:51:00 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Sep 2023 01:51:00 GMT
USER varnish
# Thu, 21 Sep 2023 01:51:00 GMT
EXPOSE 80 8443
# Thu, 21 Sep 2023 01:51:00 GMT
CMD []
```

-	Layers:
	-	`sha256:ec103030fda7a896185e8eb8a4f00b7f611725434956faa395cf74a993a2742e`  
		Last Modified: Mon, 07 Aug 2023 19:43:01 GMT  
		Size: 2.6 MB (2609002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c222777618072a84cbc1cc334e324f1cf6549d9aec24add4de60d61b25f04bf`  
		Last Modified: Thu, 21 Sep 2023 01:54:50 GMT  
		Size: 46.3 MB (46326423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f13e8e461de6c2bbbcf5890fd1669c82689bfea1ce6d63af764a6d281a801cf`  
		Last Modified: Thu, 21 Sep 2023 01:54:43 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:latest`

```console
$ docker pull varnish@sha256:8aebb0e2fdb98f8c8f08529f42264f599ce08a7ab0179236767aebaaa62d6d7e
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
$ docker pull varnish@sha256:e03566ef6752192c478b1aa7bba603dc26f1ee563934c03f28e9c6a7a5396d59
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134737591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:266771d9cf5c42149096e6813c1b152608a114703951e87c69ce3220c862ab70`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 18:34:50 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 11 Oct 2023 18:34:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:27:13 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Wed, 11 Oct 2023 21:27:13 GMT
ARG VARNISH_VERSION=7.4.1
# Wed, 11 Oct 2023 21:27:13 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Wed, 11 Oct 2023 21:27:14 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 11 Oct 2023 21:27:14 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 11 Oct 2023 21:27:14 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Wed, 11 Oct 2023 21:27:14 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Wed, 11 Oct 2023 21:27:14 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Wed, 11 Oct 2023 21:27:14 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Wed, 11 Oct 2023 21:27:14 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Wed, 11 Oct 2023 21:27:14 GMT
ENV VARNISH_SIZE=100M
# Wed, 11 Oct 2023 21:30:00 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.1.tgz -o $tmpdir/orig.tgz;     echo "d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 11 Oct 2023 21:30:01 GMT
WORKDIR /etc/varnish
# Wed, 11 Oct 2023 21:30:01 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 11 Oct 2023 21:30:01 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 11 Oct 2023 21:30:01 GMT
USER varnish
# Wed, 11 Oct 2023 21:30:01 GMT
EXPOSE 80 8443
# Wed, 11 Oct 2023 21:30:01 GMT
CMD []
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73d3b02baeacb05096f1d533167545798575b4b39a4f516a201ad8a3c0fd9e0`  
		Last Modified: Wed, 11 Oct 2023 21:35:14 GMT  
		Size: 105.6 MB (105587228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c88afe6700045cede25a79c7cae3b4fd9c2630ea13c3445c62ee292dc732123`  
		Last Modified: Wed, 11 Oct 2023 21:34:59 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; arm variant v7

```console
$ docker pull varnish@sha256:1feecff1374e6c3d603761b67362c81d8a15190b4fce34911d6257281a848cad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105036990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91cb20c34e8cd2ad07e5e4d7fb9e378a81db336a803bd894fda058508b99013f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:42:11 GMT
ADD file:da08fed31a161a2210fd920a1b5e43aa3f4199985cdeaa0d5d24c0a0f19044aa in / 
# Wed, 11 Oct 2023 17:42:11 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:09:22 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Wed, 11 Oct 2023 18:09:22 GMT
ARG VARNISH_VERSION=7.4.1
# Wed, 11 Oct 2023 18:09:22 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Wed, 11 Oct 2023 18:09:22 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 11 Oct 2023 18:09:22 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 11 Oct 2023 18:09:22 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Wed, 11 Oct 2023 18:09:22 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Wed, 11 Oct 2023 18:09:22 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Wed, 11 Oct 2023 18:09:22 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Wed, 11 Oct 2023 18:09:22 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Wed, 11 Oct 2023 18:09:23 GMT
ENV VARNISH_SIZE=100M
# Wed, 11 Oct 2023 18:12:11 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.1.tgz -o $tmpdir/orig.tgz;     echo "d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 11 Oct 2023 18:12:12 GMT
WORKDIR /etc/varnish
# Wed, 11 Oct 2023 18:12:12 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 11 Oct 2023 18:12:12 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 11 Oct 2023 18:12:12 GMT
USER varnish
# Wed, 11 Oct 2023 18:12:12 GMT
EXPOSE 80 8443
# Wed, 11 Oct 2023 18:12:12 GMT
CMD []
```

-	Layers:
	-	`sha256:2f11c34abc7b59f09b58bb6e2cf54f260f4b4142ecf8023a114e281ea4b532d1`  
		Last Modified: Wed, 11 Oct 2023 17:46:22 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3d75364756f4e459e71b5941b35371acb082f8bb2f09c42230d48ff70cfa56`  
		Last Modified: Wed, 11 Oct 2023 18:17:46 GMT  
		Size: 80.3 MB (80287576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd120edc727486131696ee7b8fb97154d80d4812e8c1865198e8b909d2e8e457`  
		Last Modified: Wed, 11 Oct 2023 18:17:34 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:472bd27e1d4a42daf22c320d58944cf4ea8243a2a3dd9300e1cb7b76264bedda
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.2 MB (129197485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6368c63db1f983c26740d4676cf9ae4da73811320dd0f21fabf6191e6e872ca`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 20 Sep 2023 02:44:13 GMT
ADD file:ec1a6e0aedd76c8fdc8544775f8b553f58950e9435f5cfe919f39374e222cfbb in / 
# Wed, 20 Sep 2023 02:44:14 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 17:48:56 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 21 Sep 2023 04:34:35 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 21 Sep 2023 04:34:36 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 21 Sep 2023 04:34:36 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 21 Sep 2023 04:34:36 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 21 Sep 2023 04:34:36 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 21 Sep 2023 04:34:36 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 21 Sep 2023 04:34:36 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 21 Sep 2023 04:34:36 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 21 Sep 2023 04:34:36 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Thu, 21 Sep 2023 04:34:36 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Sep 2023 04:37:04 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.1.tgz -o $tmpdir/orig.tgz;     echo "d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 21 Sep 2023 04:37:06 GMT
WORKDIR /etc/varnish
# Thu, 21 Sep 2023 04:37:06 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 21 Sep 2023 04:37:06 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Sep 2023 04:37:06 GMT
USER varnish
# Thu, 21 Sep 2023 04:37:06 GMT
EXPOSE 80 8443
# Thu, 21 Sep 2023 04:37:06 GMT
CMD []
```

-	Layers:
	-	`sha256:e886f0f47ef56fcadb6ecaf2116056bbdb273e0afe07ed034498b198d386c04e`  
		Last Modified: Wed, 20 Sep 2023 02:47:36 GMT  
		Size: 29.2 MB (29157221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d168552ad41a2f9b1ae51e74b416a1fbf5f899631badf1ecf74bb5962f131c8`  
		Last Modified: Thu, 21 Sep 2023 04:41:26 GMT  
		Size: 100.0 MB (100039772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aee0db284127fd79a1e633f9ee036d58c5817770e41d69607d88963d53c073f`  
		Last Modified: Thu, 21 Sep 2023 04:41:15 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; 386

```console
$ docker pull varnish@sha256:b0b281bd04e70c06c4d95562ddc165603c7fcb63797a5307ea577d0854a46ba0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131877976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8763c9a49d7d742b60afd31d81ea0e3816bba8e58111f0d3bfc26b36fc3c66f5`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:40:42 GMT
ADD file:31318c1b1f05d559cce42f5b12eef97d916932217e0b987fb07c0fc11bf0a14a in / 
# Wed, 11 Oct 2023 17:40:42 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 08:38:19 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 12 Oct 2023 08:38:19 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 12 Oct 2023 08:38:20 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 12 Oct 2023 08:38:20 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 12 Oct 2023 08:38:20 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 12 Oct 2023 08:38:20 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 12 Oct 2023 08:38:20 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 12 Oct 2023 08:38:20 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 12 Oct 2023 08:38:20 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 12 Oct 2023 08:38:20 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Thu, 12 Oct 2023 08:38:20 GMT
ENV VARNISH_SIZE=100M
# Thu, 12 Oct 2023 08:42:04 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.1.tgz -o $tmpdir/orig.tgz;     echo "d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 12 Oct 2023 08:42:05 GMT
WORKDIR /etc/varnish
# Thu, 12 Oct 2023 08:42:05 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 12 Oct 2023 08:42:05 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 12 Oct 2023 08:42:06 GMT
USER varnish
# Thu, 12 Oct 2023 08:42:06 GMT
EXPOSE 80 8443
# Thu, 12 Oct 2023 08:42:06 GMT
CMD []
```

-	Layers:
	-	`sha256:b27d0f1369837277a82877763487cdd2535037988fc27e16f11cf74e103ae4cd`  
		Last Modified: Wed, 11 Oct 2023 17:45:31 GMT  
		Size: 30.2 MB (30164118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4d7224a6538ed66733bc96ac79177a58d0039e0e68594173cc295e2ea9b504`  
		Last Modified: Thu, 12 Oct 2023 08:48:35 GMT  
		Size: 101.7 MB (101713366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:621ed1744001a5b482de115c1a397507d44f792c45cdd41dce56ecb1fca9cbe3`  
		Last Modified: Thu, 12 Oct 2023 08:48:15 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; ppc64le

```console
$ docker pull varnish@sha256:180fe86166e9d0d3b446cedb5e1b6b04f386a146b06c3e5faa0c574866f91999
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.7 MB (137667538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b6eb4c889e8ef2ee0187d1b231a86f99e559d96be323785f2739b97ea92f83d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:44:19 GMT
ADD file:53c83bdd58e7c4003ae769596cc2f8e6b72c0bbb854dbe7f006a39f273848b1b in / 
# Wed, 11 Oct 2023 17:44:21 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 12:12:26 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 12 Oct 2023 12:12:27 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 12 Oct 2023 12:12:27 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 12 Oct 2023 12:12:27 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 12 Oct 2023 12:12:28 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 12 Oct 2023 12:12:28 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 12 Oct 2023 12:12:29 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 12 Oct 2023 12:12:29 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 12 Oct 2023 12:12:29 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 12 Oct 2023 12:12:30 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Thu, 12 Oct 2023 12:12:30 GMT
ENV VARNISH_SIZE=100M
# Thu, 12 Oct 2023 12:19:14 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.1.tgz -o $tmpdir/orig.tgz;     echo "d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 12 Oct 2023 12:19:21 GMT
WORKDIR /etc/varnish
# Thu, 12 Oct 2023 12:19:21 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 12 Oct 2023 12:19:22 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 12 Oct 2023 12:19:22 GMT
USER varnish
# Thu, 12 Oct 2023 12:19:23 GMT
EXPOSE 80 8443
# Thu, 12 Oct 2023 12:19:24 GMT
CMD []
```

-	Layers:
	-	`sha256:54813908ce8a5d8a81f2db88ad0366eb5266484c7c402e5e93ef26e764f7a0e2`  
		Last Modified: Wed, 11 Oct 2023 17:49:58 GMT  
		Size: 33.1 MB (33141653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30256924f5530cebc1ea042b5fde8499f912e388dc12580b7f4bfb886ed621b9`  
		Last Modified: Thu, 12 Oct 2023 12:31:24 GMT  
		Size: 104.5 MB (104525394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2d85d3edf39adfb61ceeaf1b92b4960089dd68c909e2f2668a96803ddb162b`  
		Last Modified: Thu, 12 Oct 2023 12:30:58 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; s390x

```console
$ docker pull varnish@sha256:c16359d33b507ad0702a5be497bc4d3bf1dc9550a6b72a01fbfef0d10a15d9e3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112330094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd8caa54cdeafd2ed33943de55ef8effd990147fcb9b0311032a90892878efb1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:50:28 GMT
ADD file:b85ed0ed01200dd3626d66cf5205d989fc48e61b3dd3498f777ee72d91e64870 in / 
# Wed, 11 Oct 2023 17:50:30 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 00:48:18 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 12 Oct 2023 00:48:18 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 12 Oct 2023 00:48:18 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 12 Oct 2023 00:48:18 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 12 Oct 2023 00:48:19 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 12 Oct 2023 00:48:19 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 12 Oct 2023 00:48:19 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 12 Oct 2023 00:48:19 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 12 Oct 2023 00:48:19 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 12 Oct 2023 00:48:19 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Thu, 12 Oct 2023 00:48:19 GMT
ENV VARNISH_SIZE=100M
# Thu, 12 Oct 2023 01:06:58 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.1.tgz -o $tmpdir/orig.tgz;     echo "d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 12 Oct 2023 01:07:08 GMT
WORKDIR /etc/varnish
# Thu, 12 Oct 2023 01:07:08 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 12 Oct 2023 01:07:08 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 12 Oct 2023 01:07:08 GMT
USER varnish
# Thu, 12 Oct 2023 01:07:09 GMT
EXPOSE 80 8443
# Thu, 12 Oct 2023 01:07:09 GMT
CMD []
```

-	Layers:
	-	`sha256:f270c1bb05fa46b165ce3680225dc9fa5bbfe4d69420a467350e80f692c78eb2`  
		Last Modified: Wed, 11 Oct 2023 17:56:03 GMT  
		Size: 27.5 MB (27512850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1ecabb8eb208085a0cd1ccad185b3741ef91253ac090a644273393b03d5ba9`  
		Last Modified: Thu, 12 Oct 2023 01:15:40 GMT  
		Size: 84.8 MB (84816753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b8069a9787fb8bc5a96e8c2c9afaa0c689c46501adc3724923dd883a96e1fd7`  
		Last Modified: Thu, 12 Oct 2023 01:15:29 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:old`

```console
$ docker pull varnish@sha256:127e17b1c06f1f4cf5d029c6711bcfee9354d75906651bd50ffdf32b79d85aa0
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
$ docker pull varnish@sha256:a472ccc3c27a471ada7e8366395dc79a818e71d630050b0071309d2c471dba72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101925092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2470d3cdd052769b3be290f06eb7865b5bfab4d102d4f8c5889eb5fec29c7b5`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:30:09 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 11 Oct 2023 21:30:10 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 11 Oct 2023 21:30:10 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 11 Oct 2023 21:30:10 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 11 Oct 2023 21:30:10 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 11 Oct 2023 21:30:10 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 11 Oct 2023 21:30:10 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 11 Oct 2023 21:30:10 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 11 Oct 2023 21:30:10 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Wed, 11 Oct 2023 21:30:10 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Wed, 11 Oct 2023 21:30:10 GMT
ENV VARNISH_SIZE=100M
# Wed, 11 Oct 2023 21:32:39 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 11 Oct 2023 21:32:40 GMT
WORKDIR /etc/varnish
# Wed, 11 Oct 2023 21:32:40 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 11 Oct 2023 21:32:40 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 11 Oct 2023 21:32:40 GMT
USER varnish
# Wed, 11 Oct 2023 21:32:40 GMT
EXPOSE 80 8443
# Wed, 11 Oct 2023 21:32:40 GMT
CMD []
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c964cf9eb5e581139a408a0283a55a73a0ac0b387e3bee71059aa21eaaae36`  
		Last Modified: Wed, 11 Oct 2023 21:35:39 GMT  
		Size: 70.5 MB (70506739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a678d3c9d19dd5252a4e5f98e08a7e6a8d6452f8de01f3dc152d30a8d93623`  
		Last Modified: Wed, 11 Oct 2023 21:35:30 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; arm variant v7

```console
$ docker pull varnish@sha256:a9d7925fd2833c99dd825f73189e690aa38ff111448711f53330829302b362bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.7 MB (78707317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02d5d5ec333f1684a11cdbabbb53763153cbcde422823880fc9915cae78872bc`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:42:29 GMT
ADD file:0d1753bfedd7193184780166819d0407867a22d82804c0045274f1f13afecac0 in / 
# Wed, 11 Oct 2023 17:42:29 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:12:16 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 11 Oct 2023 18:12:16 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 11 Oct 2023 18:12:16 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 11 Oct 2023 18:12:16 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 11 Oct 2023 18:12:16 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 11 Oct 2023 18:12:16 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 11 Oct 2023 18:12:16 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 11 Oct 2023 18:12:17 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 11 Oct 2023 18:12:17 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Wed, 11 Oct 2023 18:12:17 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Wed, 11 Oct 2023 18:12:17 GMT
ENV VARNISH_SIZE=100M
# Wed, 11 Oct 2023 18:15:16 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 11 Oct 2023 18:15:16 GMT
WORKDIR /etc/varnish
# Wed, 11 Oct 2023 18:15:17 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 11 Oct 2023 18:15:17 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 11 Oct 2023 18:15:17 GMT
USER varnish
# Wed, 11 Oct 2023 18:15:17 GMT
EXPOSE 80 8443
# Wed, 11 Oct 2023 18:15:17 GMT
CMD []
```

-	Layers:
	-	`sha256:bb9c59b28e9fb9c31ffdb002ca9a6656677eee093c8093fcbea8818e927df70a`  
		Last Modified: Wed, 11 Oct 2023 17:47:06 GMT  
		Size: 26.6 MB (26579008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38680172be1c560e622889d04d9c977f9d93f880d53d1e3d2f84f70ef22b3a64`  
		Last Modified: Wed, 11 Oct 2023 18:18:07 GMT  
		Size: 52.1 MB (52127820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22797eea0f7d1b6cf952632b0be79cac85a2fb2ffa9e162de7ad6efe3026ead6`  
		Last Modified: Wed, 11 Oct 2023 18:18:00 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:e8ade371f73b19375bfd39a503bf3fec6b9e3ba7a9bafc5c3ba88ffeb9f27797
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.7 MB (95748930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3603bd166369d9986732f8f2a43d559412758d24ee0ac9ecd035f46ef49585d0`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:27:25 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 11 Oct 2023 22:27:25 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 11 Oct 2023 22:27:25 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 11 Oct 2023 22:27:25 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 11 Oct 2023 22:27:25 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 11 Oct 2023 22:27:26 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 11 Oct 2023 22:27:26 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 11 Oct 2023 22:27:26 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 11 Oct 2023 22:27:26 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Wed, 11 Oct 2023 22:27:26 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Wed, 11 Oct 2023 22:27:26 GMT
ENV VARNISH_SIZE=100M
# Wed, 11 Oct 2023 22:29:57 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 11 Oct 2023 22:29:57 GMT
WORKDIR /etc/varnish
# Wed, 11 Oct 2023 22:29:57 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 11 Oct 2023 22:29:57 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 11 Oct 2023 22:29:58 GMT
USER varnish
# Wed, 11 Oct 2023 22:29:58 GMT
EXPOSE 80 8443
# Wed, 11 Oct 2023 22:29:58 GMT
CMD []
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a10b543b10fa7fe9ead7538159ed2a4a3f37453153e60f65860b28bf2b4636c`  
		Last Modified: Wed, 11 Oct 2023 22:32:03 GMT  
		Size: 65.7 MB (65684356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e9d1d8ab82d707c25944e2f98cc9a834f8688d17efa7d0e7223762c92326e6`  
		Last Modified: Wed, 11 Oct 2023 22:31:56 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; 386

```console
$ docker pull varnish@sha256:cf5384fe85789a6ec705bfd6f37bb749b01d363bad340ce22cbdd9b7f474f5f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.2 MB (103168532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ef8f5b869005d0b5d34f2bb62212faef600ff5004337126ae91e3df8b379da1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:41:03 GMT
ADD file:ec6d51df021532be6c52d882f60a33d5cce8c3bff039efe8b98e923f2658ba45 in / 
# Wed, 11 Oct 2023 17:41:03 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 08:42:14 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Thu, 12 Oct 2023 08:42:14 GMT
ARG VARNISH_VERSION=7.3.0
# Thu, 12 Oct 2023 08:42:14 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Thu, 12 Oct 2023 08:42:14 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 12 Oct 2023 08:42:14 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 12 Oct 2023 08:42:14 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 12 Oct 2023 08:42:15 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Thu, 12 Oct 2023 08:42:15 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Thu, 12 Oct 2023 08:42:15 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 12 Oct 2023 08:42:15 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Thu, 12 Oct 2023 08:42:15 GMT
ENV VARNISH_SIZE=100M
# Thu, 12 Oct 2023 08:45:37 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 12 Oct 2023 08:45:37 GMT
WORKDIR /etc/varnish
# Thu, 12 Oct 2023 08:45:38 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 12 Oct 2023 08:45:38 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 12 Oct 2023 08:45:38 GMT
USER varnish
# Thu, 12 Oct 2023 08:45:38 GMT
EXPOSE 80 8443
# Thu, 12 Oct 2023 08:45:38 GMT
CMD []
```

-	Layers:
	-	`sha256:f088164df28359c53d5766709e069e084073984ecf4688687b4c7c529a8926a5`  
		Last Modified: Wed, 11 Oct 2023 17:46:21 GMT  
		Size: 32.4 MB (32402649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7276ed813d357be91f70a38731c43be595eea25c4c272cf07f899866ffef3133`  
		Last Modified: Thu, 12 Oct 2023 08:49:04 GMT  
		Size: 70.8 MB (70765390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5e53d3521a45c593fa0ce54a8ba6c98748e7adf2ceda330ab6c1a54594f4d56`  
		Last Modified: Thu, 12 Oct 2023 08:48:51 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; ppc64le

```console
$ docker pull varnish@sha256:1dfdb622e87f19c7b5d56aa688bf9c954001b5880a9adf745686f09c0c810f49
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.8 MB (100847499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fffc62d9a1870537e7026dec2307845cfa49a5b6a5a048770f7e6828fd747efe`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:44:53 GMT
ADD file:96450fb62af4cd68105cbbf612cb5d2f79139cc9416835b6c2fdf40727635939 in / 
# Wed, 11 Oct 2023 17:44:55 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 12:19:39 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Thu, 12 Oct 2023 12:19:39 GMT
ARG VARNISH_VERSION=7.3.0
# Thu, 12 Oct 2023 12:19:40 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Thu, 12 Oct 2023 12:19:40 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 12 Oct 2023 12:19:40 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 12 Oct 2023 12:19:41 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 12 Oct 2023 12:19:41 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Thu, 12 Oct 2023 12:19:42 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Thu, 12 Oct 2023 12:19:43 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 12 Oct 2023 12:19:43 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Thu, 12 Oct 2023 12:19:43 GMT
ENV VARNISH_SIZE=100M
# Thu, 12 Oct 2023 12:24:47 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 12 Oct 2023 12:24:49 GMT
WORKDIR /etc/varnish
# Thu, 12 Oct 2023 12:24:50 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 12 Oct 2023 12:24:50 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 12 Oct 2023 12:24:50 GMT
USER varnish
# Thu, 12 Oct 2023 12:24:50 GMT
EXPOSE 80 8443
# Thu, 12 Oct 2023 12:24:51 GMT
CMD []
```

-	Layers:
	-	`sha256:cde4df93466f96fbb1bbc513d09d354ea1e58d3e619c19fcf9120dbba87405ea`  
		Last Modified: Wed, 11 Oct 2023 17:50:55 GMT  
		Size: 35.3 MB (35293715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f55666fce1391d828fed4ccaa48b5dfe237758aab33c149d33d9d3c843c08a`  
		Last Modified: Thu, 12 Oct 2023 12:31:56 GMT  
		Size: 65.6 MB (65553292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ace75fc704ec4e7022d88d22c2d18dc2130858cc6939340483e46c3adca952`  
		Last Modified: Thu, 12 Oct 2023 12:31:40 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; s390x

```console
$ docker pull varnish@sha256:79828902a6814eedb26de74d04e0584b230792099854ce12010480292b1a1289
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.3 MB (82301300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ecbfad0f4fbd761fe1f432160333f1b520d1128cde705f2162200f8d47a63bb`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:50:58 GMT
ADD file:0cfc89fea6da8404b2bccfb0c408dde9e7497e8a93304c4ced9e51bd2b3a319a in / 
# Wed, 11 Oct 2023 17:51:00 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 01:07:22 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Thu, 12 Oct 2023 01:07:22 GMT
ARG VARNISH_VERSION=7.3.0
# Thu, 12 Oct 2023 01:07:22 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Thu, 12 Oct 2023 01:07:22 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 12 Oct 2023 01:07:23 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 12 Oct 2023 01:07:23 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Thu, 12 Oct 2023 01:07:23 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Thu, 12 Oct 2023 01:07:23 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Thu, 12 Oct 2023 01:07:24 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 12 Oct 2023 01:07:24 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Thu, 12 Oct 2023 01:07:24 GMT
ENV VARNISH_SIZE=100M
# Thu, 12 Oct 2023 01:12:57 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.0.tgz -o $tmpdir/orig.tgz;     echo "2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 12 Oct 2023 01:13:00 GMT
WORKDIR /etc/varnish
# Thu, 12 Oct 2023 01:13:00 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 12 Oct 2023 01:13:00 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 12 Oct 2023 01:13:00 GMT
USER varnish
# Thu, 12 Oct 2023 01:13:01 GMT
EXPOSE 80 8443
# Thu, 12 Oct 2023 01:13:01 GMT
CMD []
```

-	Layers:
	-	`sha256:a12df18f4c86c0f825c6b30eb023dc9f30ba0de34f6b97dca708a7247f4f6c49`  
		Last Modified: Wed, 11 Oct 2023 17:57:36 GMT  
		Size: 29.7 MB (29656917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bcbf52c84564aa12a68365a8ebf7a38a9a32fcd14d02b393dca8b9cba346789`  
		Last Modified: Thu, 12 Oct 2023 01:16:19 GMT  
		Size: 52.6 MB (52643890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6b13ce2c8b747fb0a75dc838a5b709fa75c3ae125301058f70da5e25c7ba79`  
		Last Modified: Thu, 12 Oct 2023 01:16:11 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:old-alpine`

```console
$ docker pull varnish@sha256:1eaaf02632201e9eb10980f58574e4d5b9bce3a96f4f146313e50d92901ae5de
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
$ docker pull varnish@sha256:c50109176635d4d06d1e3e8e2d6935d30a999947a87a9915adfc38911c3edbf0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.4 MB (59353279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6814db3789c866db3caba06dcbf3a5af9894ab56e19d8e605215f65f9f63d01`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:20:37 GMT
ADD file:4faae297b6caba92e1791a5ff667be0fcb4de6a4de2df155395957ef9d8ad5e5 in / 
# Mon, 07 Aug 2023 19:20:37 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:07:42 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 09 Aug 2023 04:07:43 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 09 Aug 2023 04:07:43 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 09 Aug 2023 04:07:43 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 09 Aug 2023 04:07:43 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 09 Aug 2023 04:07:43 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 09 Aug 2023 04:07:43 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 09 Aug 2023 04:07:43 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 09 Aug 2023 04:07:43 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Wed, 09 Aug 2023 04:07:43 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Wed, 09 Aug 2023 04:07:43 GMT
ENV VARNISH_SIZE=100M
# Wed, 09 Aug 2023 04:09:00 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Wed, 09 Aug 2023 04:09:01 GMT
WORKDIR /etc/varnish
# Wed, 09 Aug 2023 04:09:01 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 09 Aug 2023 04:09:01 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 09 Aug 2023 04:09:01 GMT
USER varnish
# Wed, 09 Aug 2023 04:09:01 GMT
EXPOSE 80 8443
# Wed, 09 Aug 2023 04:09:01 GMT
CMD []
```

-	Layers:
	-	`sha256:3695f6c099b80e503148dbb435d044c35147f81d34b9d6fbb27b3dcf1fd7ecaf`  
		Last Modified: Mon, 07 Aug 2023 19:21:27 GMT  
		Size: 2.8 MB (2826006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a571445311e41e13f2fc1c6ace8610ded14d6ac0c9a00d88f8fc8907d48e2f`  
		Last Modified: Wed, 09 Aug 2023 04:10:57 GMT  
		Size: 56.5 MB (56526777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f0487466108411358ef19a0fa4e224b5368812219ee7a97f6fca2b9c34e188`  
		Last Modified: Wed, 09 Aug 2023 04:10:50 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:a9066203838a2bbf6acd2a4af3dc33997546bf8e67c2502c6185b3e9d983cad7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45110187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e147f405a969edfd9f1c37b4f1a4429593d5975f3c68e98d04bc95c209c112be`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:57:37 GMT
ADD file:842dfa6e14e0537b53781830cfb26da9fa7a63229a7a1decc0fe08d8c000b5a9 in / 
# Mon, 07 Aug 2023 19:57:37 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 21:52:52 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Tue, 08 Aug 2023 21:52:52 GMT
ARG VARNISH_VERSION=7.3.0
# Tue, 08 Aug 2023 21:52:53 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Tue, 08 Aug 2023 21:52:53 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 08 Aug 2023 21:52:54 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 08 Aug 2023 21:52:54 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Tue, 08 Aug 2023 21:52:54 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Tue, 08 Aug 2023 21:52:54 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Tue, 08 Aug 2023 21:52:54 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 08 Aug 2023 21:52:55 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Tue, 08 Aug 2023 21:52:55 GMT
ENV VARNISH_SIZE=100M
# Tue, 08 Aug 2023 21:54:47 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Tue, 08 Aug 2023 21:54:47 GMT
WORKDIR /etc/varnish
# Tue, 08 Aug 2023 21:54:47 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 08 Aug 2023 21:54:47 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 08 Aug 2023 21:54:47 GMT
USER varnish
# Tue, 08 Aug 2023 21:54:47 GMT
EXPOSE 80 8443
# Tue, 08 Aug 2023 21:54:47 GMT
CMD []
```

-	Layers:
	-	`sha256:c25753df0ee4b6d3db1dacebcfb1839260ed067556f1f3ff52ddb574cab51045`  
		Last Modified: Mon, 07 Aug 2023 19:58:28 GMT  
		Size: 2.4 MB (2436761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3835c5b95f60e45f72f9756939da73ac2e053ce0e8b25927e9c38eafaa28134d`  
		Last Modified: Tue, 08 Aug 2023 21:57:08 GMT  
		Size: 42.7 MB (42672929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d6e8e8160593ed0c9c95f9057b778ef9a351adb3eaace602c4d2313dbb2d80`  
		Last Modified: Tue, 08 Aug 2023 21:57:00 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:fa2793323936a2a39bc749fe8c9f4d57ed1f5cacfc7bebd45acab4714d719ac6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52090034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73f5f31a9b25c2236a27ca4ea7326c16321adb4109342c0f4b66cb18945fc936`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:39:29 GMT
ADD file:21f240e1e33b25dacee7291cdd8c7750995aa0f460d13496a08c4a2dd92323aa in / 
# Mon, 07 Aug 2023 19:39:29 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:27:59 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 09 Aug 2023 04:27:59 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 09 Aug 2023 04:27:59 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 09 Aug 2023 04:28:00 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 09 Aug 2023 04:28:00 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 09 Aug 2023 04:28:00 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 09 Aug 2023 04:28:00 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 09 Aug 2023 04:28:00 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 09 Aug 2023 04:28:00 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Wed, 09 Aug 2023 04:28:00 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Wed, 09 Aug 2023 04:28:00 GMT
ENV VARNISH_SIZE=100M
# Wed, 09 Aug 2023 04:29:12 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Wed, 09 Aug 2023 04:29:13 GMT
WORKDIR /etc/varnish
# Wed, 09 Aug 2023 04:29:13 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 09 Aug 2023 04:29:13 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 09 Aug 2023 04:29:13 GMT
USER varnish
# Wed, 09 Aug 2023 04:29:13 GMT
EXPOSE 80 8443
# Wed, 09 Aug 2023 04:29:13 GMT
CMD []
```

-	Layers:
	-	`sha256:ad3fa0ea069c04e4ee9be58cf0ae9e1a8a56f649b96a96298203b055e8c903ff`  
		Last Modified: Mon, 07 Aug 2023 19:40:16 GMT  
		Size: 2.7 MB (2720868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af416d837d369577895656da730e7b9045ced484cb509a3c8d24ea5651f2b72b`  
		Last Modified: Wed, 09 Aug 2023 04:30:54 GMT  
		Size: 49.4 MB (49368670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72ad8cfaa77fff8808621330b797c9dcd268d87ee399f1cadc48654257351c9`  
		Last Modified: Wed, 09 Aug 2023 04:30:49 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; 386

```console
$ docker pull varnish@sha256:40db9d7b920acf3c24a1f0fc818151592d3d617cd98e20b08149fc9526fc24c1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59534324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7db33e169f8fc0973f7d7ebf8d7a395cf221ac4eb15d75050d00bbf746d39e28`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:38:38 GMT
ADD file:2d8ac62dd229ef26536f5a9af9e61df30ea68d609fa969786dfd531aea18cf3c in / 
# Mon, 07 Aug 2023 19:38:38 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 22:26:01 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Tue, 08 Aug 2023 22:26:01 GMT
ARG VARNISH_VERSION=7.3.0
# Tue, 08 Aug 2023 22:26:01 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Tue, 08 Aug 2023 22:26:01 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 08 Aug 2023 22:26:01 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 08 Aug 2023 22:26:01 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Tue, 08 Aug 2023 22:26:01 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Tue, 08 Aug 2023 22:26:02 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Tue, 08 Aug 2023 22:26:02 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 08 Aug 2023 22:26:02 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Tue, 08 Aug 2023 22:26:02 GMT
ENV VARNISH_SIZE=100M
# Tue, 08 Aug 2023 22:28:20 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Tue, 08 Aug 2023 22:28:21 GMT
WORKDIR /etc/varnish
# Tue, 08 Aug 2023 22:28:21 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 08 Aug 2023 22:28:21 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 08 Aug 2023 22:28:21 GMT
USER varnish
# Tue, 08 Aug 2023 22:28:21 GMT
EXPOSE 80 8443
# Tue, 08 Aug 2023 22:28:22 GMT
CMD []
```

-	Layers:
	-	`sha256:add53095769493cde9110fd91f113357e53b9e0d94abf216b811fcf00107674e`  
		Last Modified: Mon, 07 Aug 2023 19:39:29 GMT  
		Size: 2.8 MB (2832316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f647a86d2fc80d9f872ddaf183a99650a85e6bb6db7ab28df1aa47f8c766c37a`  
		Last Modified: Tue, 08 Aug 2023 22:30:58 GMT  
		Size: 56.7 MB (56701511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4a6dc8cb05579dc1a1b1fcb6f15a0661ae9a7feaf8ba4eb6397236e86e4143`  
		Last Modified: Tue, 08 Aug 2023 22:30:48 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:c3a57b142209c5534422dc949c7c67a1ec15ef65f53837b3ecdce1507c22ad17
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49132355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78138cefb19943eea37fdcc772c9f4065c5177abf063d6fcb02c473414a5e3c4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 20:16:50 GMT
ADD file:f730d2cd05a420ffd38548ae1611345fc40a7db59dea5ff41328caa60ee42608 in / 
# Mon, 07 Aug 2023 20:16:51 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:50:57 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Tue, 08 Aug 2023 23:50:58 GMT
ARG VARNISH_VERSION=7.3.0
# Tue, 08 Aug 2023 23:50:58 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Tue, 08 Aug 2023 23:50:59 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 08 Aug 2023 23:50:59 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 08 Aug 2023 23:51:00 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Tue, 08 Aug 2023 23:51:00 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Tue, 08 Aug 2023 23:51:01 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Tue, 08 Aug 2023 23:51:01 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 08 Aug 2023 23:51:02 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Tue, 08 Aug 2023 23:51:02 GMT
ENV VARNISH_SIZE=100M
# Tue, 08 Aug 2023 23:53:25 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Tue, 08 Aug 2023 23:53:28 GMT
WORKDIR /etc/varnish
# Tue, 08 Aug 2023 23:53:28 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 08 Aug 2023 23:53:28 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 08 Aug 2023 23:53:28 GMT
USER varnish
# Tue, 08 Aug 2023 23:53:29 GMT
EXPOSE 80 8443
# Tue, 08 Aug 2023 23:53:29 GMT
CMD []
```

-	Layers:
	-	`sha256:f1ecf55aa97fb0011a1c90ffc58e5cb218908bc85a13afe003aea5a46e045ac8`  
		Last Modified: Mon, 07 Aug 2023 20:18:07 GMT  
		Size: 2.8 MB (2812358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e313b1b6994e0de7da0d5b504d453dd6890fafeb0e8debf9808e953fcfc3e1d1`  
		Last Modified: Tue, 08 Aug 2023 23:56:42 GMT  
		Size: 46.3 MB (46319501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f91dcda5c6dfcb572578877b768d18db70e587fc1cc7ce78429376e9546b94`  
		Last Modified: Tue, 08 Aug 2023 23:56:31 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:4d0ba154b6574f740056123e5f8384b43d90feab3dd12fb2bc6d4eca68a6bcd0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47593252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00fb757c92f0c2efeaa1eb32bcafb1400510fc0fb7ff5c160bd2714a1325cff4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:42:16 GMT
ADD file:db6cafb0897c5e32510edd0166d1e1b23001bef271dad57e4157d560bd09dd93 in / 
# Mon, 07 Aug 2023 19:42:16 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:19:26 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Wed, 09 Aug 2023 04:19:27 GMT
ARG VARNISH_VERSION=7.3.0
# Wed, 09 Aug 2023 04:19:27 GMT
ARG DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165
# Wed, 09 Aug 2023 04:19:28 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 09 Aug 2023 04:19:29 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 09 Aug 2023 04:19:30 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 09 Aug 2023 04:19:30 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Wed, 09 Aug 2023 04:19:31 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Wed, 09 Aug 2023 04:19:32 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Wed, 09 Aug 2023 04:19:33 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Wed, 09 Aug 2023 04:19:34 GMT
ENV VARNISH_SIZE=100M
# Wed, 09 Aug 2023 04:21:51 GMT
# ARGS: DIST_SHA512=2693ed52dccc889e0bb1035ef1e3e5e12b8060ff3be6e6b78593b83f60408035649185dc29dd92265e18d362c3bff2f82cd74b7ae0aa68b94b40013824f3c165 PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.0 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Wed, 09 Aug 2023 04:22:01 GMT
WORKDIR /etc/varnish
# Wed, 09 Aug 2023 04:22:01 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 09 Aug 2023 04:22:02 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 09 Aug 2023 04:22:03 GMT
USER varnish
# Wed, 09 Aug 2023 04:22:03 GMT
EXPOSE 80 8443
# Wed, 09 Aug 2023 04:22:04 GMT
CMD []
```

-	Layers:
	-	`sha256:ec103030fda7a896185e8eb8a4f00b7f611725434956faa395cf74a993a2742e`  
		Last Modified: Mon, 07 Aug 2023 19:43:01 GMT  
		Size: 2.6 MB (2609002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161846c9c73015426cc80840fbb38cd2016810411f252eb724f4fee1ea84cfbc`  
		Last Modified: Wed, 09 Aug 2023 04:25:34 GMT  
		Size: 45.0 MB (44983753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893cc747d7f6b07b13980f3ceffbd432e9f4f78e9025f02e37ce6eb64e576b48`  
		Last Modified: Wed, 09 Aug 2023 04:25:28 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:stable`

```console
$ docker pull varnish@sha256:fb2e04b1f54164cddf211eebf12b28454c53ca3a9f7cdce988139b686e32746d
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
$ docker pull varnish@sha256:a2fedd4b349bef78954711ebf0c48d29529d9665b24c87be8d68469f7b301601
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.8 MB (95777272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:088201a03c09141b578de5f1a90431a08261d79560690ceec3a8611cd3cb8139`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:32:51 GMT
ENV VARNISH_SIZE=100M
# Wed, 11 Oct 2023 21:34:27 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 11 Oct 2023 21:34:28 GMT
WORKDIR /etc/varnish
# Wed, 11 Oct 2023 21:34:28 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 11 Oct 2023 21:34:28 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 11 Oct 2023 21:34:28 GMT
EXPOSE 80 8443
# Wed, 11 Oct 2023 21:34:28 GMT
CMD []
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f466157a7a5fef1673f33f132f409dc74a64a07cb115ed2c205c6fb160f57db8`  
		Last Modified: Wed, 11 Oct 2023 21:36:01 GMT  
		Size: 64.4 MB (64358708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ce6e3334e93dd03918524df1b07da65b86555a5dd2e0b3a8d1758967710f2b`  
		Last Modified: Wed, 11 Oct 2023 21:35:52 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; arm variant v7

```console
$ docker pull varnish@sha256:31b618463c24e16717213a163e6fdfda57f5ebb66af4f243fb975047a1e5c306
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.8 MB (72779237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1cae40c71c4d7501687eb440e432afdd6a26e012aba587fb1b0dace08c63301`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:42:29 GMT
ADD file:0d1753bfedd7193184780166819d0407867a22d82804c0045274f1f13afecac0 in / 
# Wed, 11 Oct 2023 17:42:29 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:15:25 GMT
ENV VARNISH_SIZE=100M
# Wed, 11 Oct 2023 18:17:06 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 11 Oct 2023 18:17:06 GMT
WORKDIR /etc/varnish
# Wed, 11 Oct 2023 18:17:06 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 11 Oct 2023 18:17:06 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 11 Oct 2023 18:17:06 GMT
EXPOSE 80 8443
# Wed, 11 Oct 2023 18:17:06 GMT
CMD []
```

-	Layers:
	-	`sha256:bb9c59b28e9fb9c31ffdb002ca9a6656677eee093c8093fcbea8818e927df70a`  
		Last Modified: Wed, 11 Oct 2023 17:47:06 GMT  
		Size: 26.6 MB (26579008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49121c62882c0fa09c7201e9a0342332b2b0e9c98b2a44964bf44876393d157e`  
		Last Modified: Wed, 11 Oct 2023 18:18:28 GMT  
		Size: 46.2 MB (46199529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4edd845338656f474cd4df537619e975b66eb14023de26b5fefc3e26b0bbe7`  
		Last Modified: Wed, 11 Oct 2023 18:18:21 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:931582d1753bfcdf601c1c014cd7f76bff9b35086ee2ea9f986c1b36a0a09088
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.9 MB (89876950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e62a2aa115496a1b3f5ba28121d5244d477851e9d4771b51c6fec40210b7c094`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:30:05 GMT
ENV VARNISH_SIZE=100M
# Wed, 11 Oct 2023 22:31:33 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 11 Oct 2023 22:31:34 GMT
WORKDIR /etc/varnish
# Wed, 11 Oct 2023 22:31:34 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 11 Oct 2023 22:31:34 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 11 Oct 2023 22:31:34 GMT
EXPOSE 80 8443
# Wed, 11 Oct 2023 22:31:34 GMT
CMD []
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9307d4506e3c009b9b9dec476e7a7b4a26706727b77cb98af3a2766eacb7993`  
		Last Modified: Wed, 11 Oct 2023 22:32:21 GMT  
		Size: 59.8 MB (59812161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3fd3fac24ecb46472db6ad2cb107ff688bf54d794ec2ab3dc6ce4263e712ae`  
		Last Modified: Wed, 11 Oct 2023 22:32:15 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; 386

```console
$ docker pull varnish@sha256:8f220404a10d593f6c07faddc6d5b32c252eafe3e3e918fa513996b10b532091
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.1 MB (97073360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a12489d0673cd00fd3b59c177e4e6a0772510a4a1f409d06e1394f3bfb07c9a8`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:41:03 GMT
ADD file:ec6d51df021532be6c52d882f60a33d5cce8c3bff039efe8b98e923f2658ba45 in / 
# Wed, 11 Oct 2023 17:41:03 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 08:45:53 GMT
ENV VARNISH_SIZE=100M
# Thu, 12 Oct 2023 08:47:58 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 12 Oct 2023 08:47:59 GMT
WORKDIR /etc/varnish
# Thu, 12 Oct 2023 08:47:59 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 12 Oct 2023 08:47:59 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 12 Oct 2023 08:47:59 GMT
EXPOSE 80 8443
# Thu, 12 Oct 2023 08:47:59 GMT
CMD []
```

-	Layers:
	-	`sha256:f088164df28359c53d5766709e069e084073984ecf4688687b4c7c529a8926a5`  
		Last Modified: Wed, 11 Oct 2023 17:46:21 GMT  
		Size: 32.4 MB (32402649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6699d0944fb8112e17e8f107db82827a2c19e0d6474e5280ca826fb9ebb1785`  
		Last Modified: Thu, 12 Oct 2023 08:49:29 GMT  
		Size: 64.7 MB (64670008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98eb18751f2956df8a3185d1a7bb422b57927cb9a6419bc9c10fd19da1a884d9`  
		Last Modified: Thu, 12 Oct 2023 08:49:16 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; ppc64le

```console
$ docker pull varnish@sha256:dcb527bec6a95f326235868b2224d0adef2a46c5e77911fa97b66f283917bdb1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.6 MB (94589366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01a2cd1f691613607a05c5f1a52e65b5ea0bef282662a03029bcd8ec32a32ad2`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:44:53 GMT
ADD file:96450fb62af4cd68105cbbf612cb5d2f79139cc9416835b6c2fdf40727635939 in / 
# Wed, 11 Oct 2023 17:44:55 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 12:25:06 GMT
ENV VARNISH_SIZE=100M
# Thu, 12 Oct 2023 12:30:37 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 12 Oct 2023 12:30:40 GMT
WORKDIR /etc/varnish
# Thu, 12 Oct 2023 12:30:40 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 12 Oct 2023 12:30:41 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 12 Oct 2023 12:30:41 GMT
EXPOSE 80 8443
# Thu, 12 Oct 2023 12:30:42 GMT
CMD []
```

-	Layers:
	-	`sha256:cde4df93466f96fbb1bbc513d09d354ea1e58d3e619c19fcf9120dbba87405ea`  
		Last Modified: Wed, 11 Oct 2023 17:50:55 GMT  
		Size: 35.3 MB (35293715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970f2ad54c0186fe95658ba1e1a19f61aa59ff8d68e1c7fc1260bacb62521adf`  
		Last Modified: Thu, 12 Oct 2023 12:32:24 GMT  
		Size: 59.3 MB (59294948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a05cb5c5fbcca586645108664334a9d2183959a15e7a36924aa0aaed55e327`  
		Last Modified: Thu, 12 Oct 2023 12:32:09 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; s390x

```console
$ docker pull varnish@sha256:6312c151e13da2a594d0081723ae173f9d125bf486b37e5fe18cfa26283bbc71
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76186973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f0768ac525a10ed3e3ec2fbbece634f0e229fa4c406d5d998369342f29b27c0`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:50:58 GMT
ADD file:0cfc89fea6da8404b2bccfb0c408dde9e7497e8a93304c4ced9e51bd2b3a319a in / 
# Wed, 11 Oct 2023 17:51:00 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 01:13:22 GMT
ENV VARNISH_SIZE=100M
# Thu, 12 Oct 2023 01:14:52 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 12 Oct 2023 01:14:55 GMT
WORKDIR /etc/varnish
# Thu, 12 Oct 2023 01:14:55 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 12 Oct 2023 01:14:55 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 12 Oct 2023 01:14:56 GMT
EXPOSE 80 8443
# Thu, 12 Oct 2023 01:14:56 GMT
CMD []
```

-	Layers:
	-	`sha256:a12df18f4c86c0f825c6b30eb023dc9f30ba0de34f6b97dca708a7247f4f6c49`  
		Last Modified: Wed, 11 Oct 2023 17:57:36 GMT  
		Size: 29.7 MB (29656917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d80cc9733cb32eb8c5432a7e7c81b9a7a14ce628c02ee290d4327994dfd50c`  
		Last Modified: Thu, 12 Oct 2023 01:17:03 GMT  
		Size: 46.5 MB (46529355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c3cc48fdfae886d0a5d91252dc870bd710dbe7770bdcba9a8efb2e621c8d9c`  
		Last Modified: Thu, 12 Oct 2023 01:16:57 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
