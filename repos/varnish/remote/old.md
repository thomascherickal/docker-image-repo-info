## `varnish:old`

```console
$ docker pull varnish@sha256:87dffb5c48c83cdcf12a3efeb6457d9e178f29604494e32b51701e1b2aa27cb7
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
$ docker pull varnish@sha256:df9b1ecb6e4ca0e98f9dbdf680885e16c7e510e2de4ddabc59ae2982e8c8cf99
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101966885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac6fda6c72241a94c1e31ff26a39609231e0b895e083619d8286a89b39030028`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Dec 2023 01:20:50 GMT
ADD file:bb44d67b03db8efaeb0c4171474f441d14ff35f328f13add32b289fca062fa2f in / 
# Tue, 19 Dec 2023 01:20:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:03:02 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Tue, 19 Dec 2023 08:03:02 GMT
ARG VARNISH_VERSION=7.3.1
# Tue, 19 Dec 2023 08:03:02 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Tue, 19 Dec 2023 08:03:03 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 19 Dec 2023 08:03:03 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 19 Dec 2023 08:03:03 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Tue, 19 Dec 2023 08:03:03 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Tue, 19 Dec 2023 08:03:03 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Tue, 19 Dec 2023 08:03:03 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 19 Dec 2023 08:03:03 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 19 Dec 2023 08:03:03 GMT
ENV VARNISH_SIZE=100M
# Tue, 19 Dec 2023 08:05:41 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.1.tgz -o $tmpdir/orig.tgz;     echo "57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 19 Dec 2023 08:05:42 GMT
WORKDIR /etc/varnish
# Tue, 19 Dec 2023 08:05:42 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 19 Dec 2023 08:05:42 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 19 Dec 2023 08:05:42 GMT
USER varnish
# Tue, 19 Dec 2023 08:05:42 GMT
EXPOSE 80 8443
# Tue, 19 Dec 2023 08:05:42 GMT
CMD []
```

-	Layers:
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e37b9699670384020e902a0ae2f3c71ef125515c77fb7f57f956fe2ab064bc8`  
		Last Modified: Tue, 19 Dec 2023 08:08:41 GMT  
		Size: 70.5 MB (70548520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbc9ee7e56bac88b0277ca7cd2409fa0ea1152bcdf965d290cd039497678c49`  
		Last Modified: Tue, 19 Dec 2023 08:08:32 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; arm variant v7

```console
$ docker pull varnish@sha256:ad549d82c4744321f31d836fa2757228ec9c6ee28a2fe56905d8606424ce55f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.8 MB (78751981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:580eedff14a9163d5717e74e0654d277448fd09bed4c6672badbf8cbbd32236f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Dec 2023 02:08:09 GMT
ADD file:496e70a34ff4dabb4eefdf40e4e2f0563bea0c120bb43206f8f52ab5a887b637 in / 
# Tue, 19 Dec 2023 02:08:09 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:15:00 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Tue, 19 Dec 2023 08:15:00 GMT
ARG VARNISH_VERSION=7.3.1
# Tue, 19 Dec 2023 08:15:00 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Tue, 19 Dec 2023 08:15:00 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 19 Dec 2023 08:15:01 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 19 Dec 2023 08:15:01 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Tue, 19 Dec 2023 08:15:01 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Tue, 19 Dec 2023 08:15:01 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Tue, 19 Dec 2023 08:15:01 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 19 Dec 2023 08:15:01 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 19 Dec 2023 08:15:01 GMT
ENV VARNISH_SIZE=100M
# Tue, 19 Dec 2023 08:17:37 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.1.tgz -o $tmpdir/orig.tgz;     echo "57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 19 Dec 2023 08:17:37 GMT
WORKDIR /etc/varnish
# Tue, 19 Dec 2023 08:17:37 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 19 Dec 2023 08:17:38 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 19 Dec 2023 08:17:38 GMT
USER varnish
# Tue, 19 Dec 2023 08:17:38 GMT
EXPOSE 80 8443
# Tue, 19 Dec 2023 08:17:38 GMT
CMD []
```

-	Layers:
	-	`sha256:19ccf4d6cc6956e4a5522352be94632923aa376a9939a4f45428a4f304c73bc8`  
		Last Modified: Tue, 19 Dec 2023 02:12:33 GMT  
		Size: 26.6 MB (26578972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8d700fb01496fa8c844f9ebb7e2c0de1106588b482a0aef5209b031c470c89`  
		Last Modified: Tue, 19 Dec 2023 08:20:32 GMT  
		Size: 52.2 MB (52172516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa853700f1de2e0c582912f1a2175a3c69c30b2cd96cf0db35fb599a9d9bd9c7`  
		Last Modified: Tue, 19 Dec 2023 08:20:25 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:32014d110bbaffe0743bdc54c6c9d439532cf91ad71fbcdbdb7ae00779b18d62
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.8 MB (95781809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66a11569b230dc214d07fcb99a041dcdfe426ea3ca30a6c31410230131217503`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 21:19:16 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Tue, 21 Nov 2023 21:19:16 GMT
ARG VARNISH_VERSION=7.3.1
# Tue, 21 Nov 2023 21:19:16 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Tue, 21 Nov 2023 21:19:16 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 21 Nov 2023 21:19:16 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 21 Nov 2023 21:19:16 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Tue, 21 Nov 2023 21:19:16 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Tue, 21 Nov 2023 21:19:16 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Tue, 21 Nov 2023 21:19:16 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 21 Nov 2023 21:19:16 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 21 Nov 2023 21:19:16 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Nov 2023 21:21:25 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.1.tgz -o $tmpdir/orig.tgz;     echo "57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 21 Nov 2023 21:21:26 GMT
WORKDIR /etc/varnish
# Tue, 21 Nov 2023 21:21:26 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 21 Nov 2023 21:21:26 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Nov 2023 21:21:26 GMT
USER varnish
# Tue, 21 Nov 2023 21:21:26 GMT
EXPOSE 80 8443
# Tue, 21 Nov 2023 21:21:26 GMT
CMD []
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc98e65c086f4b548a2e982f49352b25a0cd9922c2f9a98330b42163385f0d4`  
		Last Modified: Tue, 21 Nov 2023 21:23:59 GMT  
		Size: 65.7 MB (65717192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff1904762c1d07cd5329fe0e393c0598fdbac6a204808c4e326bd44f6f505eb`  
		Last Modified: Tue, 21 Nov 2023 21:23:52 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; 386

```console
$ docker pull varnish@sha256:522eb24b5d28a7295ce65f1086e33d5d85beaf7c9c65b3c60759498baeb3d4e0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.2 MB (103212796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b70fc90e400e9dfbd466ceab45b7e7287a51be25ddbbc35bb9b1668978ffda0d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Nov 2023 04:40:15 GMT
ADD file:7de881b584405a880c4d02778056aaa81bb5dd5d1af65b3086d66aed9ff0ad4b in / 
# Tue, 21 Nov 2023 04:40:16 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 15:15:08 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Tue, 21 Nov 2023 15:15:08 GMT
ARG VARNISH_VERSION=7.3.1
# Tue, 21 Nov 2023 15:15:08 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Tue, 21 Nov 2023 15:15:08 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 21 Nov 2023 15:15:09 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 21 Nov 2023 15:15:09 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Tue, 21 Nov 2023 15:15:09 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Tue, 21 Nov 2023 15:15:09 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Tue, 21 Nov 2023 15:15:09 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 21 Nov 2023 15:15:09 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 21 Nov 2023 15:15:09 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Nov 2023 15:18:32 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.1.tgz -o $tmpdir/orig.tgz;     echo "57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 21 Nov 2023 15:18:33 GMT
WORKDIR /etc/varnish
# Tue, 21 Nov 2023 15:18:33 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 21 Nov 2023 15:18:33 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Nov 2023 15:18:34 GMT
USER varnish
# Tue, 21 Nov 2023 15:18:34 GMT
EXPOSE 80 8443
# Tue, 21 Nov 2023 15:18:34 GMT
CMD []
```

-	Layers:
	-	`sha256:75c11612678b54e79a38118fe66e532c61b3d0798afb741007b4cd3209c0ec4e`  
		Last Modified: Tue, 21 Nov 2023 04:45:24 GMT  
		Size: 32.4 MB (32402632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae3bc414da66bdd2d32a046a233e988a45ad7faaa11b96e0f5e55973fa16073`  
		Last Modified: Tue, 21 Nov 2023 15:22:12 GMT  
		Size: 70.8 MB (70809672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d549858933a493ec89c83cb3fafe3fec83022f9eae66525cdcbdf30fc7e49c92`  
		Last Modified: Tue, 21 Nov 2023 15:21:58 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; ppc64le

```console
$ docker pull varnish@sha256:66a0133569e260a895c68333c0426c77cdaa6c2f4dcb29b8f24906c16932c150
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.9 MB (100887371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc4919272c647cb21a3aee48eb9f1a2e0a70f042c7da2e16ef2463f7cf62433b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Nov 2023 04:24:43 GMT
ADD file:b0d18f2d04821eb50d1faecc1a64916f5c63dd386ae71a3b2cb1d6c4aac6e1c4 in / 
# Tue, 21 Nov 2023 04:24:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 12:54:35 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Tue, 21 Nov 2023 12:54:35 GMT
ARG VARNISH_VERSION=7.3.1
# Tue, 21 Nov 2023 12:54:36 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Tue, 21 Nov 2023 12:54:36 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 21 Nov 2023 12:54:36 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 21 Nov 2023 12:54:37 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Tue, 21 Nov 2023 12:54:37 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Tue, 21 Nov 2023 12:54:37 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Tue, 21 Nov 2023 12:54:37 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 21 Nov 2023 12:54:38 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 21 Nov 2023 12:54:38 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Nov 2023 12:58:17 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.1.tgz -o $tmpdir/orig.tgz;     echo "57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 21 Nov 2023 12:58:19 GMT
WORKDIR /etc/varnish
# Tue, 21 Nov 2023 12:58:19 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 21 Nov 2023 12:58:20 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Nov 2023 12:58:20 GMT
USER varnish
# Tue, 21 Nov 2023 12:58:20 GMT
EXPOSE 80 8443
# Tue, 21 Nov 2023 12:58:20 GMT
CMD []
```

-	Layers:
	-	`sha256:60239a74847cd7e9a928353188f3cf096ca8cf648e2b27c765058e169d568fd9`  
		Last Modified: Tue, 21 Nov 2023 04:29:47 GMT  
		Size: 35.3 MB (35293727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef474112e53d3cd9414bbc58b355c42c87c37b9296900ac553800b9812b43a51`  
		Last Modified: Tue, 21 Nov 2023 13:02:23 GMT  
		Size: 65.6 MB (65593153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72377d237fe1a86489eea9d2d9f72ba19b74303b09593612e4f440d909932fc`  
		Last Modified: Tue, 21 Nov 2023 13:02:12 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; s390x

```console
$ docker pull varnish@sha256:0ab6caa4ba596675fb6506e80cd6416e352dc89123bce57cd6a750c5e9162e99
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.3 MB (82337376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77957464272e0f2a1870b20c4bd51bf9af77a796e6053701d2cc4d533ee2cc88`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Dec 2023 01:43:11 GMT
ADD file:36a070457acddafcd6cdda22a3c41efcbd4e2b1694831eb74c8143520ebf1cf2 in / 
# Tue, 19 Dec 2023 01:43:14 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 09:57:28 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Tue, 19 Dec 2023 09:57:28 GMT
ARG VARNISH_VERSION=7.3.1
# Tue, 19 Dec 2023 09:57:28 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Tue, 19 Dec 2023 09:57:29 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 19 Dec 2023 09:57:29 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 19 Dec 2023 09:57:30 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Tue, 19 Dec 2023 09:57:30 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Tue, 19 Dec 2023 09:57:30 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Tue, 19 Dec 2023 09:57:31 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 19 Dec 2023 09:57:31 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 19 Dec 2023 09:57:31 GMT
ENV VARNISH_SIZE=100M
# Tue, 19 Dec 2023 09:59:40 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.1.tgz -o $tmpdir/orig.tgz;     echo "57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 19 Dec 2023 09:59:43 GMT
WORKDIR /etc/varnish
# Tue, 19 Dec 2023 09:59:43 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 19 Dec 2023 09:59:43 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 19 Dec 2023 09:59:44 GMT
USER varnish
# Tue, 19 Dec 2023 09:59:44 GMT
EXPOSE 80 8443
# Tue, 19 Dec 2023 09:59:44 GMT
CMD []
```

-	Layers:
	-	`sha256:eff2a4367cf88d5103011eba9299da2b4d173b0bde5dc0455020febf72b9b1c4`  
		Last Modified: Tue, 19 Dec 2023 01:48:08 GMT  
		Size: 29.7 MB (29657006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973b42ff7f83f76b123f93bf3b16fc127a7cc9fe1475d16b393a84485a77e625`  
		Last Modified: Tue, 19 Dec 2023 10:02:30 GMT  
		Size: 52.7 MB (52679878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e8e963aca39b2ea7900e6590a2e12624c36457b736760d4d9eb8d5289d9da7`  
		Last Modified: Tue, 19 Dec 2023 10:02:23 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
