## `swift:amazonlinux2-slim`

```console
$ docker pull swift@sha256:0c61608827244cad4c3f1e475ceccce482adc70bc9be8a16f05942ed60571297
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swift:amazonlinux2-slim` - linux; amd64

```console
$ docker pull swift@sha256:9297c1dd86b91499e8831985f5dad4943d4656244c00b637b4fad7092c17d137
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.8 MB (193816329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a3a20419c02fc5c98901ced4c2f72fab094ac28e17fcf9dd55d49cd22c7faed`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 18 Dec 2020 07:04:34 GMT
ADD file:63bb1089f29109498e6000d9884216288b7b1b9093e0c247b99df2a8ba64d601 in / 
# Fri, 18 Dec 2020 07:04:35 GMT
CMD ["/bin/bash"]
# Fri, 18 Dec 2020 09:30:35 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@swift.org>
# Fri, 18 Dec 2020 09:30:36 GMT
LABEL description=Docker Container for the Swift programming language
# Fri, 18 Dec 2020 09:32:39 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Fri, 18 Dec 2020 09:32:39 GMT
ARG SWIFT_PLATFORM=amazonlinux2
# Fri, 18 Dec 2020 09:32:39 GMT
ARG SWIFT_BRANCH=swift-5.3.2-release
# Fri, 18 Dec 2020 09:32:39 GMT
ARG SWIFT_VERSION=swift-5.3.2-RELEASE
# Fri, 18 Dec 2020 09:32:39 GMT
ARG SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 18 Dec 2020 09:32:40 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=amazonlinux2 SWIFT_BRANCH=swift-5.3.2-release SWIFT_VERSION=swift-5.3.2-RELEASE SWIFT_WEBROOT=https://swift.org/builds/
# Fri, 18 Dec 2020 09:33:50 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)/"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver ha.pool.sks-keyservers.net --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && yum -y install tar gzip     && tar -xzf swift.tar.gz --directory / --strip-components=1 $SWIFT_VERSION-$SWIFT_PLATFORM/usr/lib/swift/linux     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && yum autoremove -y tar gzip
```

-	Layers:
	-	`sha256:b6f03d5d6f5a93eede753139822eca5ce4a921a8c35922b9969996cfc31deb60`  
		Last Modified: Wed, 09 Dec 2020 16:33:37 GMT  
		Size: 62.0 MB (62008519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b9c22ad3e152ba42550706d9c91b9be7548dbdf45dd982b301e2de995b4be5`  
		Last Modified: Fri, 18 Dec 2020 09:41:19 GMT  
		Size: 131.8 MB (131807810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
