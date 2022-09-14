## `swift:bionic`

```console
$ docker pull swift@sha256:06379bfd936b2980746e20a71a3923ae09aa820972c228d51deb2eadc9c5038f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `swift:bionic` - linux; amd64

```console
$ docker pull swift@sha256:08c92a96de4e29ee2f940d7b9fd5baeda2ba89346a405f95bba09303991a46b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **724.8 MB (724841945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:317cbf21f70c41765ea641369782d10757a329492cf36b48295e0a8651a1dc74`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 19:38:36 GMT
ADD file:8733c7e8faf03d53cb2143ff6ac405362944cfa07422fccd21a3066cc2f42c83 in / 
# Tue, 06 Sep 2022 19:38:37 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 20:55:44 GMT
LABEL maintainer=Swift Infrastructure <swift-infrastructure@forums.swift.org>
# Tue, 06 Sep 2022 20:55:44 GMT
LABEL Description=Docker Container for the Swift programming language
# Mon, 12 Sep 2022 18:21:43 GMT
RUN export DEBIAN_FRONTEND=noninteractive DEBCONF_NONINTERACTIVE_SEEN=true && apt-get -q update &&     apt-get -q install -y     libatomic1     libcurl4-openssl-dev     libxml2-dev     libedit2     libsqlite3-0     libc6-dev     binutils     libgcc-5-dev     libstdc++-5-dev     zlib1g-dev     libpython3.6     tzdata     git     unzip     pkg-config     && rm -r /var/lib/apt/lists/*
# Mon, 12 Sep 2022 18:21:44 GMT
ARG SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561
# Mon, 12 Sep 2022 18:21:44 GMT
ARG SWIFT_PLATFORM=ubuntu18.04
# Wed, 14 Sep 2022 00:30:47 GMT
ARG SWIFT_BRANCH=swift-5.7-release
# Wed, 14 Sep 2022 00:30:47 GMT
ARG SWIFT_VERSION=swift-5.7-RELEASE
# Wed, 14 Sep 2022 00:30:47 GMT
ARG SWIFT_WEBROOT=https://download.swift.org
# Wed, 14 Sep 2022 00:30:47 GMT
ENV SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561 SWIFT_PLATFORM=ubuntu18.04 SWIFT_BRANCH=swift-5.7-release SWIFT_VERSION=swift-5.7-RELEASE SWIFT_WEBROOT=https://download.swift.org
# Wed, 14 Sep 2022 00:31:42 GMT
RUN set -e;     SWIFT_WEBDIR="$SWIFT_WEBROOT/$SWIFT_BRANCH/$(echo $SWIFT_PLATFORM | tr -d .)"     && SWIFT_BIN_URL="$SWIFT_WEBDIR/$SWIFT_VERSION/$SWIFT_VERSION-$SWIFT_PLATFORM.tar.gz"     && SWIFT_SIG_URL="$SWIFT_BIN_URL.sig"     && export DEBIAN_FRONTEND=noninteractive     && apt-get -q update && apt-get -q install -y curl && rm -rf /var/lib/apt/lists/*     && export GNUPGHOME="$(mktemp -d)"     && curl -fsSL "$SWIFT_BIN_URL" -o swift.tar.gz "$SWIFT_SIG_URL" -o swift.tar.gz.sig     && gpg --batch --quiet --keyserver keyserver.ubuntu.com --recv-keys "$SWIFT_SIGNING_KEY"     && gpg --batch --verify swift.tar.gz.sig swift.tar.gz     && tar -xzf swift.tar.gz --directory / --strip-components=1     && chmod -R o+r /usr/lib/swift     && rm -rf "$GNUPGHOME" swift.tar.gz.sig swift.tar.gz     && apt-get purge --auto-remove -y curl
# Wed, 14 Sep 2022 00:31:48 GMT
RUN swift --version
```

-	Layers:
	-	`sha256:726b8a513d66e3585eb57389171d97fcd348e4914a415891e1da135b85ffa6c3`  
		Last Modified: Fri, 02 Sep 2022 15:41:13 GMT  
		Size: 26.7 MB (26710833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20d3ae3c18ad8a1f9eb086adc2a1dc7f831b940168720f62306b751ae5ae8e17`  
		Last Modified: Mon, 12 Sep 2022 18:38:15 GMT  
		Size: 151.9 MB (151860997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abea7052ad25adf2d53b01c2989c0bdb634c30e555528b6b2b748c8c83ec923`  
		Last Modified: Wed, 14 Sep 2022 00:50:37 GMT  
		Size: 546.3 MB (546269886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:304df6e78882a342ed464c678d406b6664164147f782fd12c827d5081e88f387`  
		Last Modified: Wed, 14 Sep 2022 00:49:20 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
