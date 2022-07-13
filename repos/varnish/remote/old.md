## `varnish:old`

```console
$ docker pull varnish@sha256:51e0b96ba23c37d1b2da665603b63c11f9a50fad2be2dcfb6ddb72e5414e001f
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
$ docker pull varnish@sha256:80ca9c3ffd61c95e2e3bd468c5906e862e51052636ad1105793018e8d74e9e69
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101190038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a1d0d3f5afe71b234b6dce0b66cfade308ae48e137821cf3cdcdba874199813`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 15:04:25 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 15:06:39 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 12 Jul 2022 15:06:39 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 15:06:39 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 12 Jul 2022 15:06:40 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 15:06:40 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 15:06:40 GMT
CMD []
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02de66ed810206b73e0c9dab04edcb5ee5e063727b6d2d4288dcacf0b689f442`  
		Last Modified: Tue, 12 Jul 2022 15:10:08 GMT  
		Size: 69.8 MB (69822955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e847f66816c3e7530bb53d396f9f98bfe1dcb263d37ca0a260ceebccaa19563d`  
		Last Modified: Tue, 12 Jul 2022 15:09:58 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; arm variant v7

```console
$ docker pull varnish@sha256:7c3d802dc2e7fe766778ba54e48633421dc875a087efceea831a254ca4925622
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.8 MB (77807084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6585bbb533608729231065c84e1179362a919001751ec67b363f511c94016674`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Wed, 13 Jul 2022 07:01:15 GMT
ENV VARNISH_SIZE=100M
# Wed, 13 Jul 2022 07:06:57 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 13 Jul 2022 07:06:58 GMT
WORKDIR /etc/varnish
# Wed, 13 Jul 2022 07:06:58 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Wed, 13 Jul 2022 07:06:59 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 13 Jul 2022 07:06:59 GMT
EXPOSE 80 8443
# Wed, 13 Jul 2022 07:07:00 GMT
CMD []
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe4c1024f00f2d9e87fb8571a9a87263d63c9cdd8b3b504e1fb44cbe5beb732`  
		Last Modified: Wed, 13 Jul 2022 07:16:17 GMT  
		Size: 51.2 MB (51246051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5549d87b127deeb9dea5cfad2a1912bcabbb94e6827be9f2e0ce7573cd768889`  
		Last Modified: Wed, 13 Jul 2022 07:15:49 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:6498c5ad6d682b0076a0cbec21fef553b379504c201a87f0f7b5f14f80e9c60c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 MB (95301932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74e738a742894266ad16f79ecd4b9a3474041d4f12dbfb804dff57c7a5d2db21`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 14:18:59 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 14:21:07 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 12 Jul 2022 14:21:07 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 14:21:09 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 12 Jul 2022 14:21:09 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 14:21:10 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 14:21:11 GMT
CMD []
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e13c66f23d97c682dfc6fca33c4ba85b04f2b9b22f0a9d4a32679def5baa25b`  
		Last Modified: Tue, 12 Jul 2022 14:25:10 GMT  
		Size: 65.2 MB (65247234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e12339074edaf212e4dc9334de848255f4ef5e943ff9e7833cc7e9b636d52b4`  
		Last Modified: Tue, 12 Jul 2022 14:25:01 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; 386

```console
$ docker pull varnish@sha256:ec9290335f55e308e7023f5d8f4972eebc2b1ee671069d8820851417cc0f17df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.6 MB (102585121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b122adf5e34794ee172b03b3fab482bc31219a96195e1e8c300c8ae4cb9d064c`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Sat, 28 May 2022 00:39:33 GMT
ADD file:8320d7b95b9f68313e086faff974bb38977e0c9da4984afb6382eb0405742bde in / 
# Sat, 28 May 2022 00:39:33 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:15:19 GMT
ENV VARNISH_SIZE=100M
# Tue, 07 Jun 2022 00:17:33 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 07 Jun 2022 00:17:34 GMT
WORKDIR /etc/varnish
# Tue, 07 Jun 2022 00:17:36 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:17:36 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 07 Jun 2022 00:17:37 GMT
EXPOSE 80 8443
# Tue, 07 Jun 2022 00:17:38 GMT
CMD []
```

-	Layers:
	-	`sha256:5e7494d2ee6c81c73ce32f8bde3ea8658c6224c2cc22d7bb01df4bc3d42949aa`  
		Last Modified: Sat, 28 May 2022 00:46:43 GMT  
		Size: 32.4 MB (32390321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bf3f822dbf481370990594e81803141573a456e04899ad82fe6c4022627ebb`  
		Last Modified: Tue, 07 Jun 2022 00:21:08 GMT  
		Size: 70.2 MB (70194327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db7dae54c84b4938c9aaa05092d4faf306897f47702a337f22ca87439181cc5`  
		Last Modified: Tue, 07 Jun 2022 00:20:57 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; ppc64le

```console
$ docker pull varnish@sha256:8e668ccfb0305d42808450c5d542f712a89205bbb695cf3f36825c355933faa3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.4 MB (100364320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cb0d8edc39e2a368cd5ba2efdae74e7b6672303d912ad677b603ba99c1d8179`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 01:25:28 GMT
ADD file:9e1afe48f40d94f879aefb12a7e68da2f0772d701e95b8219bd1f79a83e1933a in / 
# Tue, 12 Jul 2022 01:25:32 GMT
CMD ["bash"]
# Wed, 13 Jul 2022 07:11:23 GMT
ENV VARNISH_SIZE=100M
# Wed, 13 Jul 2022 07:29:07 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 13 Jul 2022 07:29:13 GMT
WORKDIR /etc/varnish
# Wed, 13 Jul 2022 07:29:18 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Wed, 13 Jul 2022 07:29:26 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 13 Jul 2022 07:29:29 GMT
EXPOSE 80 8443
# Wed, 13 Jul 2022 07:29:33 GMT
CMD []
```

-	Layers:
	-	`sha256:bd3d68d1ce583727f6378a16916795b955cc0ad39e0ebe754a26007ef54744fa`  
		Last Modified: Tue, 12 Jul 2022 01:36:03 GMT  
		Size: 35.3 MB (35272500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d1ab9f3ba01143c4ffbfcd260cbc0159169c5379516de25bc82ab9f77aafb3`  
		Last Modified: Wed, 13 Jul 2022 07:59:25 GMT  
		Size: 65.1 MB (65091347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8bf85f3ee82e9ef01f54879daa7288065cccc18442cfe118afd693643636d6e`  
		Last Modified: Wed, 13 Jul 2022 07:59:13 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; s390x

```console
$ docker pull varnish@sha256:4b16cb3b466bbe809c4833e2631cd4a9ddf572227e11c2fb3ce158a52465a752
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.6 MB (81623472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:426be98166563a81501f737bf7edd9103507a566117a5395e75a6d54d80ada03`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 00:43:45 GMT
ADD file:70135711d42f7b2b32586e31afb57a0590019326efa82abf1402dc7a8f02a3f2 in / 
# Tue, 12 Jul 2022 00:43:49 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 19:13:57 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 19:19:47 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 12 Jul 2022 19:19:57 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 19:19:57 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 12 Jul 2022 19:19:58 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 19:19:59 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 19:20:00 GMT
CMD []
```

-	Layers:
	-	`sha256:447abc12b0c6da6e339b4fa17a2a7dd672d6f0631d30ee44c28b8b06e78884bd`  
		Last Modified: Tue, 12 Jul 2022 00:53:41 GMT  
		Size: 29.6 MB (29640209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f44713e40e8cd034f4c8f4dd815e5302835db628ffb0d6f606de6a30b3e909c`  
		Last Modified: Tue, 12 Jul 2022 19:28:33 GMT  
		Size: 52.0 MB (51982789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a43b712b028475ec29bca3a805cc61d86ec779b321fcd68dcdf093c4f9cfc1e`  
		Last Modified: Tue, 12 Jul 2022 19:28:25 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
