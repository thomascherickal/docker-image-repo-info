## `swift:amazonlinux2-slim`

```console
$ docker pull swift@sha256:97507f92ce49439f05f9040eb0f556272728ae58a876b509dfc58117fe728116
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:amazonlinux2-slim` - linux; amd64

```console
$ docker pull swift@sha256:0ef3c19f6e61a6884ab5d3aee5661189fec642feb8ba68fd739a50c4222914e3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.1 MB (187062427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e40e4688c47d088762e711326359d5e1823282c2175d3187e485f3dcf221a92`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:19:45 GMT
ADD file:92220f428664788288d5cda805c94b48f6a5e957d4c7724085f3278d0a864f6d in / 
# Fri, 31 Jul 2020 22:19:46 GMT
CMD ["/bin/bash"]
# Fri, 31 Jul 2020 22:36:52 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 31 Jul 2020 22:36:52 GMT
LABEL description=Docker Container for the Swift programming language
# Tue, 11 Aug 2020 19:32:36 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Tue, 11 Aug 2020 19:32:37 GMT
ARG SWIFT_PLATFORM=amazonlinux2
# Thu, 17 Sep 2020 22:31:39 GMT
ARG SWIFT_BRANCH=swift-5.3-release
# Thu, 17 Sep 2020 22:31:42 GMT
ARG SWIFT_VERSION=swift-5.3-RELEASE
# Thu, 17 Sep 2020 22:31:46 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Thu, 17 Sep 2020 22:31:46 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=amazonlinux2 SWIFT_BRANCH=swift-5.3-release SWIFT_VERSION=swift-5.3-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Thu, 17 Sep 2020 22:33:07 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && yum -y install tar gzip     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && yum autoremove -y tar gzip
```

-	Layers:
	-	`sha256:37373184fe69e0fc20370c26317bf4c5b9b843c60b375563d4ee1c7766a89782`  
		Last Modified: Fri, 31 Jul 2020 22:20:37 GMT  
		Size: 61.7 MB (61716540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f6bd6d2ee27f134b2a3a53e91e46de3c714201d0bee663bc5f838ce39cb024`  
		Last Modified: Thu, 17 Sep 2020 22:48:18 GMT  
		Size: 125.3 MB (125345887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
