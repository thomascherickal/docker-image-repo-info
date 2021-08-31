<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kong`

-	[`kong:2.4`](#kong24)
-	[`kong:2.4-alpine`](#kong24-alpine)
-	[`kong:2.4-centos`](#kong24-centos)
-	[`kong:2.4-ubuntu`](#kong24-ubuntu)
-	[`kong:2.4.1`](#kong241)
-	[`kong:2.4.1-alpine`](#kong241-alpine)
-	[`kong:2.4.1-centos`](#kong241-centos)
-	[`kong:2.4.1-ubuntu`](#kong241-ubuntu)
-	[`kong:2.5`](#kong25)
-	[`kong:2.5-centos`](#kong25-centos)
-	[`kong:2.5-ubuntu`](#kong25-ubuntu)
-	[`kong:2.5.0`](#kong250)
-	[`kong:2.5.0-alpine`](#kong250-alpine)
-	[`kong:2.5.0-centos`](#kong250-centos)
-	[`kong:2.5.0-ubuntu`](#kong250-ubuntu)
-	[`kong:alpine`](#kongalpine)
-	[`kong:centos`](#kongcentos)
-	[`kong:latest`](#konglatest)
-	[`kong:ubuntu`](#kongubuntu)

## `kong:2.4`

```console
$ docker pull kong@sha256:c9872460e6c9cb05d5ac1f125fff571c00541d4da7438f5eb821e07a56efe752
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.4` - linux; amd64

```console
$ docker pull kong@sha256:31e0abee64747a4a31159b4d41538a03d9cbf7bfbe9708e00d5703aa9ce5f2b5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51160610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b022e820b9b2bb6de4b8d0a3f8d50702612ef93ab70a2a108c020bac31b4f02a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:56 GMT
ADD file:282b9d56236cae29600bf8b698cb0a865ab17db7beea0be6870f9de63e7d4f80 in / 
# Wed, 14 Apr 2021 19:19:56 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:23:21 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 14 Apr 2021 19:23:21 GMT
ARG ASSET=ce
# Wed, 14 Apr 2021 19:23:21 GMT
ENV ASSET=ce
# Wed, 14 Apr 2021 19:23:22 GMT
ARG EE_PORTS
# Wed, 14 Apr 2021 19:23:22 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 11 May 2021 22:29:40 GMT
ARG KONG_VERSION=2.4.1
# Tue, 11 May 2021 22:29:40 GMT
ENV KONG_VERSION=2.4.1
# Tue, 11 May 2021 22:29:40 GMT
ARG KONG_AMD64_SHA=582cbcf23eb4dcdf9873105ac7d8428a4022ec61bcc68642ad9dd8a5c03e2a57
# Tue, 11 May 2021 22:29:40 GMT
ENV KONG_AMD64_SHA=582cbcf23eb4dcdf9873105ac7d8428a4022ec61bcc68642ad9dd8a5c03e2a57
# Tue, 11 May 2021 22:29:40 GMT
ARG KONG_ARM64_SHA=5ec35d1b19dd4e6592ad2c6586e68bfd1549c6a22840ce7d5654677b94e5028a
# Tue, 11 May 2021 22:29:40 GMT
ENV KONG_ARM64_SHA=5ec35d1b19dd4e6592ad2c6586e68bfd1549c6a22840ce7d5654677b94e5028a
# Tue, 11 May 2021 22:29:48 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;; 		aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Tue, 11 May 2021 22:29:49 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Tue, 11 May 2021 22:29:49 GMT
USER kong
# Tue, 11 May 2021 22:29:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 11 May 2021 22:29:49 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 11 May 2021 22:29:49 GMT
STOPSIGNAL SIGQUIT
# Tue, 11 May 2021 22:29:50 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ddad3d7c1e96adf9153f8921a7c9790f880a390163df453be1566e9ef0d546e0`  
		Last Modified: Wed, 14 Apr 2021 19:21:03 GMT  
		Size: 2.8 MB (2816246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2472b23dfb901e3b9a325bd2956bf0a230c603b44b559b671f46090712feaa25`  
		Last Modified: Wed, 14 Apr 2021 19:29:06 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04308f3534771e4911ece45118ea51db7d9a992c72336fb9c1165a8fe3ca894e`  
		Last Modified: Tue, 11 May 2021 22:33:23 GMT  
		Size: 48.3 MB (48343499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af5626bb095a631ee85ddaae2c1bc71dd4085dfd56e149ba5f34fbe3a71cd05`  
		Last Modified: Tue, 11 May 2021 22:33:15 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.4` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:a350bd912a622a02b61e9c5b6b20c5e3365f5544407ee1b8b4c63e9a8f0bdec0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50694302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58e44d048d3428713b1443578b223a2833de190e4e9adcd22a618d1fba72fd1e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:15 GMT
ADD file:62109d08b751b6f41eb8dc5dcb3ea6b553619ef0a58a40685faa749a20c3b051 in / 
# Tue, 15 Jun 2021 21:45:15 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 01:03:52 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 16 Jun 2021 01:03:52 GMT
ARG ASSET=ce
# Wed, 16 Jun 2021 01:03:52 GMT
ENV ASSET=ce
# Wed, 16 Jun 2021 01:03:52 GMT
ARG EE_PORTS
# Wed, 16 Jun 2021 01:03:52 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 16 Jun 2021 01:03:52 GMT
ARG KONG_VERSION=2.4.1
# Wed, 16 Jun 2021 01:03:53 GMT
ENV KONG_VERSION=2.4.1
# Wed, 16 Jun 2021 01:03:53 GMT
ARG KONG_AMD64_SHA=582cbcf23eb4dcdf9873105ac7d8428a4022ec61bcc68642ad9dd8a5c03e2a57
# Wed, 16 Jun 2021 01:03:53 GMT
ENV KONG_AMD64_SHA=582cbcf23eb4dcdf9873105ac7d8428a4022ec61bcc68642ad9dd8a5c03e2a57
# Wed, 16 Jun 2021 01:03:53 GMT
ARG KONG_ARM64_SHA=5ec35d1b19dd4e6592ad2c6586e68bfd1549c6a22840ce7d5654677b94e5028a
# Wed, 16 Jun 2021 01:03:53 GMT
ENV KONG_ARM64_SHA=5ec35d1b19dd4e6592ad2c6586e68bfd1549c6a22840ce7d5654677b94e5028a
# Wed, 16 Jun 2021 01:04:00 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;; 		aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Wed, 16 Jun 2021 01:04:01 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 16 Jun 2021 01:04:01 GMT
USER kong
# Wed, 16 Jun 2021 01:04:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 16 Jun 2021 01:04:01 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 16 Jun 2021 01:04:02 GMT
STOPSIGNAL SIGQUIT
# Wed, 16 Jun 2021 01:04:02 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:535256e01bcb9590f56b9b2a053648a1d98fbe4dc0fd34c1fc3f32afec8c6e7b`  
		Last Modified: Wed, 14 Apr 2021 18:44:02 GMT  
		Size: 2.7 MB (2726928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68089cee6c0f6ef8dd053c9f3b7d70c11dda2c426bf38daac971441a912c9bf0`  
		Last Modified: Wed, 16 Jun 2021 01:06:17 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc4661998cf20ee5e8dc00d8c36cc7bac6fb43f2c86ea1c68d7ed96e3698b15`  
		Last Modified: Wed, 16 Jun 2021 01:06:27 GMT  
		Size: 48.0 MB (47966509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4afbf6dc6d0b33bda49d4eeb05932798f55369bdb1969730abc0ac73fd9f0e4`  
		Last Modified: Wed, 16 Jun 2021 01:06:17 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.4-alpine`

```console
$ docker pull kong@sha256:c9872460e6c9cb05d5ac1f125fff571c00541d4da7438f5eb821e07a56efe752
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.4-alpine` - linux; amd64

```console
$ docker pull kong@sha256:31e0abee64747a4a31159b4d41538a03d9cbf7bfbe9708e00d5703aa9ce5f2b5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51160610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b022e820b9b2bb6de4b8d0a3f8d50702612ef93ab70a2a108c020bac31b4f02a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:56 GMT
ADD file:282b9d56236cae29600bf8b698cb0a865ab17db7beea0be6870f9de63e7d4f80 in / 
# Wed, 14 Apr 2021 19:19:56 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:23:21 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 14 Apr 2021 19:23:21 GMT
ARG ASSET=ce
# Wed, 14 Apr 2021 19:23:21 GMT
ENV ASSET=ce
# Wed, 14 Apr 2021 19:23:22 GMT
ARG EE_PORTS
# Wed, 14 Apr 2021 19:23:22 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 11 May 2021 22:29:40 GMT
ARG KONG_VERSION=2.4.1
# Tue, 11 May 2021 22:29:40 GMT
ENV KONG_VERSION=2.4.1
# Tue, 11 May 2021 22:29:40 GMT
ARG KONG_AMD64_SHA=582cbcf23eb4dcdf9873105ac7d8428a4022ec61bcc68642ad9dd8a5c03e2a57
# Tue, 11 May 2021 22:29:40 GMT
ENV KONG_AMD64_SHA=582cbcf23eb4dcdf9873105ac7d8428a4022ec61bcc68642ad9dd8a5c03e2a57
# Tue, 11 May 2021 22:29:40 GMT
ARG KONG_ARM64_SHA=5ec35d1b19dd4e6592ad2c6586e68bfd1549c6a22840ce7d5654677b94e5028a
# Tue, 11 May 2021 22:29:40 GMT
ENV KONG_ARM64_SHA=5ec35d1b19dd4e6592ad2c6586e68bfd1549c6a22840ce7d5654677b94e5028a
# Tue, 11 May 2021 22:29:48 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;; 		aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Tue, 11 May 2021 22:29:49 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Tue, 11 May 2021 22:29:49 GMT
USER kong
# Tue, 11 May 2021 22:29:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 11 May 2021 22:29:49 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 11 May 2021 22:29:49 GMT
STOPSIGNAL SIGQUIT
# Tue, 11 May 2021 22:29:50 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ddad3d7c1e96adf9153f8921a7c9790f880a390163df453be1566e9ef0d546e0`  
		Last Modified: Wed, 14 Apr 2021 19:21:03 GMT  
		Size: 2.8 MB (2816246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2472b23dfb901e3b9a325bd2956bf0a230c603b44b559b671f46090712feaa25`  
		Last Modified: Wed, 14 Apr 2021 19:29:06 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04308f3534771e4911ece45118ea51db7d9a992c72336fb9c1165a8fe3ca894e`  
		Last Modified: Tue, 11 May 2021 22:33:23 GMT  
		Size: 48.3 MB (48343499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af5626bb095a631ee85ddaae2c1bc71dd4085dfd56e149ba5f34fbe3a71cd05`  
		Last Modified: Tue, 11 May 2021 22:33:15 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.4-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:a350bd912a622a02b61e9c5b6b20c5e3365f5544407ee1b8b4c63e9a8f0bdec0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50694302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58e44d048d3428713b1443578b223a2833de190e4e9adcd22a618d1fba72fd1e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:15 GMT
ADD file:62109d08b751b6f41eb8dc5dcb3ea6b553619ef0a58a40685faa749a20c3b051 in / 
# Tue, 15 Jun 2021 21:45:15 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 01:03:52 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 16 Jun 2021 01:03:52 GMT
ARG ASSET=ce
# Wed, 16 Jun 2021 01:03:52 GMT
ENV ASSET=ce
# Wed, 16 Jun 2021 01:03:52 GMT
ARG EE_PORTS
# Wed, 16 Jun 2021 01:03:52 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 16 Jun 2021 01:03:52 GMT
ARG KONG_VERSION=2.4.1
# Wed, 16 Jun 2021 01:03:53 GMT
ENV KONG_VERSION=2.4.1
# Wed, 16 Jun 2021 01:03:53 GMT
ARG KONG_AMD64_SHA=582cbcf23eb4dcdf9873105ac7d8428a4022ec61bcc68642ad9dd8a5c03e2a57
# Wed, 16 Jun 2021 01:03:53 GMT
ENV KONG_AMD64_SHA=582cbcf23eb4dcdf9873105ac7d8428a4022ec61bcc68642ad9dd8a5c03e2a57
# Wed, 16 Jun 2021 01:03:53 GMT
ARG KONG_ARM64_SHA=5ec35d1b19dd4e6592ad2c6586e68bfd1549c6a22840ce7d5654677b94e5028a
# Wed, 16 Jun 2021 01:03:53 GMT
ENV KONG_ARM64_SHA=5ec35d1b19dd4e6592ad2c6586e68bfd1549c6a22840ce7d5654677b94e5028a
# Wed, 16 Jun 2021 01:04:00 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;; 		aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Wed, 16 Jun 2021 01:04:01 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 16 Jun 2021 01:04:01 GMT
USER kong
# Wed, 16 Jun 2021 01:04:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 16 Jun 2021 01:04:01 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 16 Jun 2021 01:04:02 GMT
STOPSIGNAL SIGQUIT
# Wed, 16 Jun 2021 01:04:02 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:535256e01bcb9590f56b9b2a053648a1d98fbe4dc0fd34c1fc3f32afec8c6e7b`  
		Last Modified: Wed, 14 Apr 2021 18:44:02 GMT  
		Size: 2.7 MB (2726928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68089cee6c0f6ef8dd053c9f3b7d70c11dda2c426bf38daac971441a912c9bf0`  
		Last Modified: Wed, 16 Jun 2021 01:06:17 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc4661998cf20ee5e8dc00d8c36cc7bac6fb43f2c86ea1c68d7ed96e3698b15`  
		Last Modified: Wed, 16 Jun 2021 01:06:27 GMT  
		Size: 48.0 MB (47966509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4afbf6dc6d0b33bda49d4eeb05932798f55369bdb1969730abc0ac73fd9f0e4`  
		Last Modified: Wed, 16 Jun 2021 01:06:17 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.4-centos`

```console
$ docker pull kong@sha256:af3b555aafa9057bf0cb66f7257fa5748e328a92cc8324ad5b9de004745bbfbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:2.4-centos` - linux; amd64

```console
$ docker pull kong@sha256:f67758723288bacee4b1a20c4afdad985bd6b338e5d5325a3adf77808c85a593
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.6 MB (127648547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c24b1346db87f019dfe4a9929b3e4cde9a8d943f5b7976063dd21e6b3124787a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 14 Nov 2020 00:20:04 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Sat, 14 Nov 2020 00:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:20:04 GMT
CMD ["/bin/bash"]
# Sat, 06 Mar 2021 07:32:08 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 06 Mar 2021 07:32:08 GMT
ARG ASSET=ce
# Sat, 06 Mar 2021 07:32:08 GMT
ENV ASSET=ce
# Sat, 06 Mar 2021 07:32:08 GMT
ARG EE_PORTS
# Sat, 06 Mar 2021 07:32:08 GMT
COPY file:ff02c070e4c89f043b176279a7e41464b5fab8cb98cfcd6332fad2d2741fc41d in /tmp/kong.rpm 
# Tue, 11 May 2021 22:31:19 GMT
ARG KONG_VERSION=2.4.1
# Tue, 11 May 2021 22:31:19 GMT
ENV KONG_VERSION=2.4.1
# Tue, 11 May 2021 22:31:19 GMT
ARG KONG_SHA256=b8083a6c268f69865e66a8d504fcdacab49ba36a4194ccfc9737d65e6863c30a
# Tue, 11 May 2021 22:31:51 GMT
# ARGS: KONG_SHA256=b8083a6c268f69865e66a8d504fcdacab49ba36a4194ccfc9737d65e6863c30a
RUN set -ex;   if [ "$ASSET" = "ce" ] ; then   curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-centos-7/Packages/k/kong-$KONG_VERSION.el7.amd64.rpm -o /tmp/kong.rpm     && echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -;   fi;   yum install -y -q unzip shadow-utils git   && yum clean all -q   && rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki   && yum install -y /tmp/kong.rpm   && yum clean all   && rm /tmp/kong.rpm   && chown kong:0 /usr/local/bin/kong   && chown -R kong:0 /usr/local/kong &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Tue, 11 May 2021 22:31:52 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Tue, 11 May 2021 22:31:52 GMT
USER kong
# Tue, 11 May 2021 22:31:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 11 May 2021 22:31:52 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 11 May 2021 22:31:53 GMT
STOPSIGNAL SIGQUIT
# Tue, 11 May 2021 22:31:53 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c237ce1272ffe51f7f4a890afaca88db75cb107611ffb1833c9dbd5161df8157`  
		Last Modified: Sat, 06 Mar 2021 07:39:18 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab966ea217fbab8c5192165645951c189bf30a8e7646590426a6d246564c324`  
		Last Modified: Tue, 11 May 2021 22:34:20 GMT  
		Size: 51.6 MB (51550529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4193596ed9cb1305f2d4c3fee914eee8727f30d3a96e36fe7f182bd5166de03b`  
		Last Modified: Tue, 11 May 2021 22:34:11 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.4-ubuntu`

```console
$ docker pull kong@sha256:e780257aead37ebeb18419dd7fe02d62e1a1085b7c734b2f77883ed6ac3fd257
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.4-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:859587738484e5cbb63685ba93d9226430fa28c79acc21a0eff6cfbc725f2dd6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134752322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dcc1c5996a9c5705bc02ee55ce61b4874e7ee7c9636966844d064e484499084`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 26 Jul 2021 21:22:15 GMT
ADD file:a94a87e268e99c78143fae5148bd1200bf0da90c0e7f42bd8c168bb205ccb105 in / 
# Mon, 26 Jul 2021 21:22:16 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 26 Jul 2021 21:22:17 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:22:17 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 26 Jul 2021 21:22:18 GMT
CMD ["/bin/bash"]
# Mon, 26 Jul 2021 23:28:42 GMT
ARG ASSET=ce
# Mon, 26 Jul 2021 23:28:43 GMT
ENV ASSET=ce
# Mon, 26 Jul 2021 23:28:43 GMT
ARG EE_PORTS
# Mon, 26 Jul 2021 23:28:43 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Mon, 26 Jul 2021 23:29:38 GMT
ARG KONG_VERSION=2.4.1
# Mon, 26 Jul 2021 23:29:38 GMT
ENV KONG_VERSION=2.4.1
# Mon, 26 Jul 2021 23:30:00 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL 		https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-xenial/pool/all/k/kong/kong_${KONG_VERSION}_$(dpkg --print-architecture).deb -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Mon, 26 Jul 2021 23:30:01 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Mon, 26 Jul 2021 23:30:01 GMT
USER kong
# Mon, 26 Jul 2021 23:30:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 26 Jul 2021 23:30:01 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 26 Jul 2021 23:30:02 GMT
STOPSIGNAL SIGQUIT
# Mon, 26 Jul 2021 23:30:02 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:52818491084148fa3469964bbcc3576686018a3b16b2e29be0407565c4c80b44`  
		Last Modified: Thu, 22 Jul 2021 16:25:00 GMT  
		Size: 46.5 MB (46497362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9df81d603d28f2a294b2f11b4f60d07b5b833b2ad7d6659a3f59b10cff2696`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636d9303bf663657be8e6796d720913bb985b5343da7949749ae1e72b54a88d8`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672b5bdcef61237567b311ad3d349f5eae18ba839ce2b204858a3083437a0a59`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdd2955c511e0c6bedd8d0fb726625f0608e6fa14d9361ab3e51b208d892ac8`  
		Last Modified: Mon, 26 Jul 2021 23:30:37 GMT  
		Size: 25.1 MB (25081965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:934e9635160ae04ed10d7ba3ac4dbefa4f2a7b7e3c1dc80786c0487a03359f8b`  
		Last Modified: Mon, 26 Jul 2021 23:31:14 GMT  
		Size: 63.2 MB (63170755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8694d3fc91dbd92576fdb17a9b7c87fec7cc944c0b33f813d7bac6953f188dae`  
		Last Modified: Mon, 26 Jul 2021 23:31:04 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.4-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:27fd09b0cec48bec925771a4413a410006f13d22f5751753725ba65eac7eaefb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125852785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ccd495383d16434f96c90ca9ac18aff97e8f9606eab8439a36fca2d77a4af70`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 31 Aug 2021 01:41:19 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Tue, 31 Aug 2021 01:41:20 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:41:20 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:41:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:41:21 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 03:13:00 GMT
ARG ASSET=ce
# Tue, 31 Aug 2021 03:13:00 GMT
ENV ASSET=ce
# Tue, 31 Aug 2021 03:13:00 GMT
ARG EE_PORTS
# Tue, 31 Aug 2021 03:13:00 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Tue, 31 Aug 2021 03:13:37 GMT
ARG KONG_VERSION=2.4.1
# Tue, 31 Aug 2021 03:13:37 GMT
ENV KONG_VERSION=2.4.1
# Tue, 31 Aug 2021 03:14:01 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL 		https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-xenial/pool/all/k/kong/kong_${KONG_VERSION}_$(dpkg --print-architecture).deb -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Tue, 31 Aug 2021 03:14:01 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Tue, 31 Aug 2021 03:14:02 GMT
USER kong
# Tue, 31 Aug 2021 03:14:02 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:14:02 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 31 Aug 2021 03:14:02 GMT
STOPSIGNAL SIGQUIT
# Tue, 31 Aug 2021 03:14:02 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85569e0c17003d9cf46a8b94076418863e0abfc5474bb830403acf246947fea7`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32ca509d28808ab7c61361835292ee8eddecd0c0949d658bde0ab1a77ecbf6e`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 469.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8168af71f81f1ffa234c301e9cc2ee87b560ad8b74ef4100f8ab4a6abf3a8ad3`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eee59a359925630cd377c9610b18f7d7797349cdbabeda7b8c8685852a5ff83`  
		Last Modified: Tue, 31 Aug 2021 03:14:48 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f85fcbb4d194d453d51be130f08022aaf7f6c3dff823e0c9028f5f03f24efd6`  
		Last Modified: Tue, 31 Aug 2021 03:15:31 GMT  
		Size: 59.5 MB (59529393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d06546a51b8a187a27923ca3d77c983e48224cfe02a2f6d4c909073482c24e`  
		Last Modified: Tue, 31 Aug 2021 03:15:20 GMT  
		Size: 688.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.4.1`

```console
$ docker pull kong@sha256:c9872460e6c9cb05d5ac1f125fff571c00541d4da7438f5eb821e07a56efe752
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.4.1` - linux; amd64

```console
$ docker pull kong@sha256:31e0abee64747a4a31159b4d41538a03d9cbf7bfbe9708e00d5703aa9ce5f2b5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51160610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b022e820b9b2bb6de4b8d0a3f8d50702612ef93ab70a2a108c020bac31b4f02a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:56 GMT
ADD file:282b9d56236cae29600bf8b698cb0a865ab17db7beea0be6870f9de63e7d4f80 in / 
# Wed, 14 Apr 2021 19:19:56 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:23:21 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 14 Apr 2021 19:23:21 GMT
ARG ASSET=ce
# Wed, 14 Apr 2021 19:23:21 GMT
ENV ASSET=ce
# Wed, 14 Apr 2021 19:23:22 GMT
ARG EE_PORTS
# Wed, 14 Apr 2021 19:23:22 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 11 May 2021 22:29:40 GMT
ARG KONG_VERSION=2.4.1
# Tue, 11 May 2021 22:29:40 GMT
ENV KONG_VERSION=2.4.1
# Tue, 11 May 2021 22:29:40 GMT
ARG KONG_AMD64_SHA=582cbcf23eb4dcdf9873105ac7d8428a4022ec61bcc68642ad9dd8a5c03e2a57
# Tue, 11 May 2021 22:29:40 GMT
ENV KONG_AMD64_SHA=582cbcf23eb4dcdf9873105ac7d8428a4022ec61bcc68642ad9dd8a5c03e2a57
# Tue, 11 May 2021 22:29:40 GMT
ARG KONG_ARM64_SHA=5ec35d1b19dd4e6592ad2c6586e68bfd1549c6a22840ce7d5654677b94e5028a
# Tue, 11 May 2021 22:29:40 GMT
ENV KONG_ARM64_SHA=5ec35d1b19dd4e6592ad2c6586e68bfd1549c6a22840ce7d5654677b94e5028a
# Tue, 11 May 2021 22:29:48 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;; 		aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Tue, 11 May 2021 22:29:49 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Tue, 11 May 2021 22:29:49 GMT
USER kong
# Tue, 11 May 2021 22:29:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 11 May 2021 22:29:49 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 11 May 2021 22:29:49 GMT
STOPSIGNAL SIGQUIT
# Tue, 11 May 2021 22:29:50 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ddad3d7c1e96adf9153f8921a7c9790f880a390163df453be1566e9ef0d546e0`  
		Last Modified: Wed, 14 Apr 2021 19:21:03 GMT  
		Size: 2.8 MB (2816246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2472b23dfb901e3b9a325bd2956bf0a230c603b44b559b671f46090712feaa25`  
		Last Modified: Wed, 14 Apr 2021 19:29:06 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04308f3534771e4911ece45118ea51db7d9a992c72336fb9c1165a8fe3ca894e`  
		Last Modified: Tue, 11 May 2021 22:33:23 GMT  
		Size: 48.3 MB (48343499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af5626bb095a631ee85ddaae2c1bc71dd4085dfd56e149ba5f34fbe3a71cd05`  
		Last Modified: Tue, 11 May 2021 22:33:15 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.4.1` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:a350bd912a622a02b61e9c5b6b20c5e3365f5544407ee1b8b4c63e9a8f0bdec0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50694302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58e44d048d3428713b1443578b223a2833de190e4e9adcd22a618d1fba72fd1e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:15 GMT
ADD file:62109d08b751b6f41eb8dc5dcb3ea6b553619ef0a58a40685faa749a20c3b051 in / 
# Tue, 15 Jun 2021 21:45:15 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 01:03:52 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 16 Jun 2021 01:03:52 GMT
ARG ASSET=ce
# Wed, 16 Jun 2021 01:03:52 GMT
ENV ASSET=ce
# Wed, 16 Jun 2021 01:03:52 GMT
ARG EE_PORTS
# Wed, 16 Jun 2021 01:03:52 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 16 Jun 2021 01:03:52 GMT
ARG KONG_VERSION=2.4.1
# Wed, 16 Jun 2021 01:03:53 GMT
ENV KONG_VERSION=2.4.1
# Wed, 16 Jun 2021 01:03:53 GMT
ARG KONG_AMD64_SHA=582cbcf23eb4dcdf9873105ac7d8428a4022ec61bcc68642ad9dd8a5c03e2a57
# Wed, 16 Jun 2021 01:03:53 GMT
ENV KONG_AMD64_SHA=582cbcf23eb4dcdf9873105ac7d8428a4022ec61bcc68642ad9dd8a5c03e2a57
# Wed, 16 Jun 2021 01:03:53 GMT
ARG KONG_ARM64_SHA=5ec35d1b19dd4e6592ad2c6586e68bfd1549c6a22840ce7d5654677b94e5028a
# Wed, 16 Jun 2021 01:03:53 GMT
ENV KONG_ARM64_SHA=5ec35d1b19dd4e6592ad2c6586e68bfd1549c6a22840ce7d5654677b94e5028a
# Wed, 16 Jun 2021 01:04:00 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;; 		aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Wed, 16 Jun 2021 01:04:01 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 16 Jun 2021 01:04:01 GMT
USER kong
# Wed, 16 Jun 2021 01:04:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 16 Jun 2021 01:04:01 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 16 Jun 2021 01:04:02 GMT
STOPSIGNAL SIGQUIT
# Wed, 16 Jun 2021 01:04:02 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:535256e01bcb9590f56b9b2a053648a1d98fbe4dc0fd34c1fc3f32afec8c6e7b`  
		Last Modified: Wed, 14 Apr 2021 18:44:02 GMT  
		Size: 2.7 MB (2726928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68089cee6c0f6ef8dd053c9f3b7d70c11dda2c426bf38daac971441a912c9bf0`  
		Last Modified: Wed, 16 Jun 2021 01:06:17 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc4661998cf20ee5e8dc00d8c36cc7bac6fb43f2c86ea1c68d7ed96e3698b15`  
		Last Modified: Wed, 16 Jun 2021 01:06:27 GMT  
		Size: 48.0 MB (47966509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4afbf6dc6d0b33bda49d4eeb05932798f55369bdb1969730abc0ac73fd9f0e4`  
		Last Modified: Wed, 16 Jun 2021 01:06:17 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.4.1-alpine`

```console
$ docker pull kong@sha256:c9872460e6c9cb05d5ac1f125fff571c00541d4da7438f5eb821e07a56efe752
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.4.1-alpine` - linux; amd64

```console
$ docker pull kong@sha256:31e0abee64747a4a31159b4d41538a03d9cbf7bfbe9708e00d5703aa9ce5f2b5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51160610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b022e820b9b2bb6de4b8d0a3f8d50702612ef93ab70a2a108c020bac31b4f02a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:56 GMT
ADD file:282b9d56236cae29600bf8b698cb0a865ab17db7beea0be6870f9de63e7d4f80 in / 
# Wed, 14 Apr 2021 19:19:56 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:23:21 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 14 Apr 2021 19:23:21 GMT
ARG ASSET=ce
# Wed, 14 Apr 2021 19:23:21 GMT
ENV ASSET=ce
# Wed, 14 Apr 2021 19:23:22 GMT
ARG EE_PORTS
# Wed, 14 Apr 2021 19:23:22 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 11 May 2021 22:29:40 GMT
ARG KONG_VERSION=2.4.1
# Tue, 11 May 2021 22:29:40 GMT
ENV KONG_VERSION=2.4.1
# Tue, 11 May 2021 22:29:40 GMT
ARG KONG_AMD64_SHA=582cbcf23eb4dcdf9873105ac7d8428a4022ec61bcc68642ad9dd8a5c03e2a57
# Tue, 11 May 2021 22:29:40 GMT
ENV KONG_AMD64_SHA=582cbcf23eb4dcdf9873105ac7d8428a4022ec61bcc68642ad9dd8a5c03e2a57
# Tue, 11 May 2021 22:29:40 GMT
ARG KONG_ARM64_SHA=5ec35d1b19dd4e6592ad2c6586e68bfd1549c6a22840ce7d5654677b94e5028a
# Tue, 11 May 2021 22:29:40 GMT
ENV KONG_ARM64_SHA=5ec35d1b19dd4e6592ad2c6586e68bfd1549c6a22840ce7d5654677b94e5028a
# Tue, 11 May 2021 22:29:48 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;; 		aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Tue, 11 May 2021 22:29:49 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Tue, 11 May 2021 22:29:49 GMT
USER kong
# Tue, 11 May 2021 22:29:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 11 May 2021 22:29:49 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 11 May 2021 22:29:49 GMT
STOPSIGNAL SIGQUIT
# Tue, 11 May 2021 22:29:50 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ddad3d7c1e96adf9153f8921a7c9790f880a390163df453be1566e9ef0d546e0`  
		Last Modified: Wed, 14 Apr 2021 19:21:03 GMT  
		Size: 2.8 MB (2816246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2472b23dfb901e3b9a325bd2956bf0a230c603b44b559b671f46090712feaa25`  
		Last Modified: Wed, 14 Apr 2021 19:29:06 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04308f3534771e4911ece45118ea51db7d9a992c72336fb9c1165a8fe3ca894e`  
		Last Modified: Tue, 11 May 2021 22:33:23 GMT  
		Size: 48.3 MB (48343499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af5626bb095a631ee85ddaae2c1bc71dd4085dfd56e149ba5f34fbe3a71cd05`  
		Last Modified: Tue, 11 May 2021 22:33:15 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.4.1-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:a350bd912a622a02b61e9c5b6b20c5e3365f5544407ee1b8b4c63e9a8f0bdec0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50694302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58e44d048d3428713b1443578b223a2833de190e4e9adcd22a618d1fba72fd1e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:15 GMT
ADD file:62109d08b751b6f41eb8dc5dcb3ea6b553619ef0a58a40685faa749a20c3b051 in / 
# Tue, 15 Jun 2021 21:45:15 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 01:03:52 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 16 Jun 2021 01:03:52 GMT
ARG ASSET=ce
# Wed, 16 Jun 2021 01:03:52 GMT
ENV ASSET=ce
# Wed, 16 Jun 2021 01:03:52 GMT
ARG EE_PORTS
# Wed, 16 Jun 2021 01:03:52 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 16 Jun 2021 01:03:52 GMT
ARG KONG_VERSION=2.4.1
# Wed, 16 Jun 2021 01:03:53 GMT
ENV KONG_VERSION=2.4.1
# Wed, 16 Jun 2021 01:03:53 GMT
ARG KONG_AMD64_SHA=582cbcf23eb4dcdf9873105ac7d8428a4022ec61bcc68642ad9dd8a5c03e2a57
# Wed, 16 Jun 2021 01:03:53 GMT
ENV KONG_AMD64_SHA=582cbcf23eb4dcdf9873105ac7d8428a4022ec61bcc68642ad9dd8a5c03e2a57
# Wed, 16 Jun 2021 01:03:53 GMT
ARG KONG_ARM64_SHA=5ec35d1b19dd4e6592ad2c6586e68bfd1549c6a22840ce7d5654677b94e5028a
# Wed, 16 Jun 2021 01:03:53 GMT
ENV KONG_ARM64_SHA=5ec35d1b19dd4e6592ad2c6586e68bfd1549c6a22840ce7d5654677b94e5028a
# Wed, 16 Jun 2021 01:04:00 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;; 		aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Wed, 16 Jun 2021 01:04:01 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 16 Jun 2021 01:04:01 GMT
USER kong
# Wed, 16 Jun 2021 01:04:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 16 Jun 2021 01:04:01 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 16 Jun 2021 01:04:02 GMT
STOPSIGNAL SIGQUIT
# Wed, 16 Jun 2021 01:04:02 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:535256e01bcb9590f56b9b2a053648a1d98fbe4dc0fd34c1fc3f32afec8c6e7b`  
		Last Modified: Wed, 14 Apr 2021 18:44:02 GMT  
		Size: 2.7 MB (2726928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68089cee6c0f6ef8dd053c9f3b7d70c11dda2c426bf38daac971441a912c9bf0`  
		Last Modified: Wed, 16 Jun 2021 01:06:17 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc4661998cf20ee5e8dc00d8c36cc7bac6fb43f2c86ea1c68d7ed96e3698b15`  
		Last Modified: Wed, 16 Jun 2021 01:06:27 GMT  
		Size: 48.0 MB (47966509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4afbf6dc6d0b33bda49d4eeb05932798f55369bdb1969730abc0ac73fd9f0e4`  
		Last Modified: Wed, 16 Jun 2021 01:06:17 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.4.1-centos`

```console
$ docker pull kong@sha256:af3b555aafa9057bf0cb66f7257fa5748e328a92cc8324ad5b9de004745bbfbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:2.4.1-centos` - linux; amd64

```console
$ docker pull kong@sha256:f67758723288bacee4b1a20c4afdad985bd6b338e5d5325a3adf77808c85a593
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.6 MB (127648547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c24b1346db87f019dfe4a9929b3e4cde9a8d943f5b7976063dd21e6b3124787a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 14 Nov 2020 00:20:04 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Sat, 14 Nov 2020 00:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:20:04 GMT
CMD ["/bin/bash"]
# Sat, 06 Mar 2021 07:32:08 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 06 Mar 2021 07:32:08 GMT
ARG ASSET=ce
# Sat, 06 Mar 2021 07:32:08 GMT
ENV ASSET=ce
# Sat, 06 Mar 2021 07:32:08 GMT
ARG EE_PORTS
# Sat, 06 Mar 2021 07:32:08 GMT
COPY file:ff02c070e4c89f043b176279a7e41464b5fab8cb98cfcd6332fad2d2741fc41d in /tmp/kong.rpm 
# Tue, 11 May 2021 22:31:19 GMT
ARG KONG_VERSION=2.4.1
# Tue, 11 May 2021 22:31:19 GMT
ENV KONG_VERSION=2.4.1
# Tue, 11 May 2021 22:31:19 GMT
ARG KONG_SHA256=b8083a6c268f69865e66a8d504fcdacab49ba36a4194ccfc9737d65e6863c30a
# Tue, 11 May 2021 22:31:51 GMT
# ARGS: KONG_SHA256=b8083a6c268f69865e66a8d504fcdacab49ba36a4194ccfc9737d65e6863c30a
RUN set -ex;   if [ "$ASSET" = "ce" ] ; then   curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-centos-7/Packages/k/kong-$KONG_VERSION.el7.amd64.rpm -o /tmp/kong.rpm     && echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -;   fi;   yum install -y -q unzip shadow-utils git   && yum clean all -q   && rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki   && yum install -y /tmp/kong.rpm   && yum clean all   && rm /tmp/kong.rpm   && chown kong:0 /usr/local/bin/kong   && chown -R kong:0 /usr/local/kong &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Tue, 11 May 2021 22:31:52 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Tue, 11 May 2021 22:31:52 GMT
USER kong
# Tue, 11 May 2021 22:31:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 11 May 2021 22:31:52 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 11 May 2021 22:31:53 GMT
STOPSIGNAL SIGQUIT
# Tue, 11 May 2021 22:31:53 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c237ce1272ffe51f7f4a890afaca88db75cb107611ffb1833c9dbd5161df8157`  
		Last Modified: Sat, 06 Mar 2021 07:39:18 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab966ea217fbab8c5192165645951c189bf30a8e7646590426a6d246564c324`  
		Last Modified: Tue, 11 May 2021 22:34:20 GMT  
		Size: 51.6 MB (51550529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4193596ed9cb1305f2d4c3fee914eee8727f30d3a96e36fe7f182bd5166de03b`  
		Last Modified: Tue, 11 May 2021 22:34:11 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.4.1-ubuntu`

```console
$ docker pull kong@sha256:e780257aead37ebeb18419dd7fe02d62e1a1085b7c734b2f77883ed6ac3fd257
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.4.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:859587738484e5cbb63685ba93d9226430fa28c79acc21a0eff6cfbc725f2dd6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134752322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dcc1c5996a9c5705bc02ee55ce61b4874e7ee7c9636966844d064e484499084`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 26 Jul 2021 21:22:15 GMT
ADD file:a94a87e268e99c78143fae5148bd1200bf0da90c0e7f42bd8c168bb205ccb105 in / 
# Mon, 26 Jul 2021 21:22:16 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 26 Jul 2021 21:22:17 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:22:17 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 26 Jul 2021 21:22:18 GMT
CMD ["/bin/bash"]
# Mon, 26 Jul 2021 23:28:42 GMT
ARG ASSET=ce
# Mon, 26 Jul 2021 23:28:43 GMT
ENV ASSET=ce
# Mon, 26 Jul 2021 23:28:43 GMT
ARG EE_PORTS
# Mon, 26 Jul 2021 23:28:43 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Mon, 26 Jul 2021 23:29:38 GMT
ARG KONG_VERSION=2.4.1
# Mon, 26 Jul 2021 23:29:38 GMT
ENV KONG_VERSION=2.4.1
# Mon, 26 Jul 2021 23:30:00 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL 		https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-xenial/pool/all/k/kong/kong_${KONG_VERSION}_$(dpkg --print-architecture).deb -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Mon, 26 Jul 2021 23:30:01 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Mon, 26 Jul 2021 23:30:01 GMT
USER kong
# Mon, 26 Jul 2021 23:30:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 26 Jul 2021 23:30:01 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 26 Jul 2021 23:30:02 GMT
STOPSIGNAL SIGQUIT
# Mon, 26 Jul 2021 23:30:02 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:52818491084148fa3469964bbcc3576686018a3b16b2e29be0407565c4c80b44`  
		Last Modified: Thu, 22 Jul 2021 16:25:00 GMT  
		Size: 46.5 MB (46497362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9df81d603d28f2a294b2f11b4f60d07b5b833b2ad7d6659a3f59b10cff2696`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636d9303bf663657be8e6796d720913bb985b5343da7949749ae1e72b54a88d8`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672b5bdcef61237567b311ad3d349f5eae18ba839ce2b204858a3083437a0a59`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdd2955c511e0c6bedd8d0fb726625f0608e6fa14d9361ab3e51b208d892ac8`  
		Last Modified: Mon, 26 Jul 2021 23:30:37 GMT  
		Size: 25.1 MB (25081965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:934e9635160ae04ed10d7ba3ac4dbefa4f2a7b7e3c1dc80786c0487a03359f8b`  
		Last Modified: Mon, 26 Jul 2021 23:31:14 GMT  
		Size: 63.2 MB (63170755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8694d3fc91dbd92576fdb17a9b7c87fec7cc944c0b33f813d7bac6953f188dae`  
		Last Modified: Mon, 26 Jul 2021 23:31:04 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.4.1-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:27fd09b0cec48bec925771a4413a410006f13d22f5751753725ba65eac7eaefb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125852785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ccd495383d16434f96c90ca9ac18aff97e8f9606eab8439a36fca2d77a4af70`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 31 Aug 2021 01:41:19 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Tue, 31 Aug 2021 01:41:20 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:41:20 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:41:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:41:21 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 03:13:00 GMT
ARG ASSET=ce
# Tue, 31 Aug 2021 03:13:00 GMT
ENV ASSET=ce
# Tue, 31 Aug 2021 03:13:00 GMT
ARG EE_PORTS
# Tue, 31 Aug 2021 03:13:00 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Tue, 31 Aug 2021 03:13:37 GMT
ARG KONG_VERSION=2.4.1
# Tue, 31 Aug 2021 03:13:37 GMT
ENV KONG_VERSION=2.4.1
# Tue, 31 Aug 2021 03:14:01 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL 		https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-xenial/pool/all/k/kong/kong_${KONG_VERSION}_$(dpkg --print-architecture).deb -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Tue, 31 Aug 2021 03:14:01 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Tue, 31 Aug 2021 03:14:02 GMT
USER kong
# Tue, 31 Aug 2021 03:14:02 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:14:02 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 31 Aug 2021 03:14:02 GMT
STOPSIGNAL SIGQUIT
# Tue, 31 Aug 2021 03:14:02 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85569e0c17003d9cf46a8b94076418863e0abfc5474bb830403acf246947fea7`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32ca509d28808ab7c61361835292ee8eddecd0c0949d658bde0ab1a77ecbf6e`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 469.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8168af71f81f1ffa234c301e9cc2ee87b560ad8b74ef4100f8ab4a6abf3a8ad3`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eee59a359925630cd377c9610b18f7d7797349cdbabeda7b8c8685852a5ff83`  
		Last Modified: Tue, 31 Aug 2021 03:14:48 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f85fcbb4d194d453d51be130f08022aaf7f6c3dff823e0c9028f5f03f24efd6`  
		Last Modified: Tue, 31 Aug 2021 03:15:31 GMT  
		Size: 59.5 MB (59529393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d06546a51b8a187a27923ca3d77c983e48224cfe02a2f6d4c909073482c24e`  
		Last Modified: Tue, 31 Aug 2021 03:15:20 GMT  
		Size: 688.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.5`

```console
$ docker pull kong@sha256:eab7328f53373a47f04e1466eeee07cde8e0808c6f36067a068e554f436d1757
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.5` - linux; amd64

```console
$ docker pull kong@sha256:40d7a2eac255f47e1af9c30a5525230573aa9e120cf25cc6dcb7d6eb61cff38b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49536515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6ccc21c00cef6852bbf840402c7c92cd19d23882e66880b3c4b74fa7c48c6a7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Tue, 13 Jul 2021 21:20:05 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 13 Jul 2021 21:20:06 GMT
ARG ASSET=ce
# Tue, 13 Jul 2021 21:20:06 GMT
ENV ASSET=ce
# Tue, 13 Jul 2021 21:20:06 GMT
ARG EE_PORTS
# Tue, 13 Jul 2021 21:20:06 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 13 Jul 2021 21:20:06 GMT
ARG KONG_VERSION=2.5.0
# Tue, 13 Jul 2021 21:20:07 GMT
ENV KONG_VERSION=2.5.0
# Tue, 13 Jul 2021 21:20:07 GMT
ARG KONG_AMD64_SHA=ebe0cf3a3e71d202774ede5083c98e2ae39fae0459d11140f53401a66527e1b7
# Tue, 13 Jul 2021 21:20:07 GMT
ENV KONG_AMD64_SHA=ebe0cf3a3e71d202774ede5083c98e2ae39fae0459d11140f53401a66527e1b7
# Tue, 13 Jul 2021 21:20:07 GMT
ARG KONG_ARM64_SHA=131964ce443f2d08dc98191fcc442867f2dee2f741ccee9cc519bb99c765f3cf
# Tue, 13 Jul 2021 21:20:07 GMT
ENV KONG_ARM64_SHA=131964ce443f2d08dc98191fcc442867f2dee2f741ccee9cc519bb99c765f3cf
# Tue, 13 Jul 2021 21:20:15 GMT
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Tue, 13 Jul 2021 21:20:15 GMT
COPY file:a9828df20ead648b4c991bfb67a40d0065e248e50a2ae98fad0104e78f32d234 in /docker-entrypoint.sh 
# Tue, 13 Jul 2021 21:20:16 GMT
USER kong
# Tue, 13 Jul 2021 21:20:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 13 Jul 2021 21:20:16 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 13 Jul 2021 21:20:16 GMT
STOPSIGNAL SIGQUIT
# Tue, 13 Jul 2021 21:20:16 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 13 Jul 2021 21:20:17 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dcb869933b18a40e5829078fafe0a2045da1deafddf08550c6346d15353e9b`  
		Last Modified: Tue, 13 Jul 2021 21:22:43 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae5d676504a7ba5bcd7a66c7882841aa52368badcb077e8e97d40bb184cc27f`  
		Last Modified: Tue, 13 Jul 2021 21:22:51 GMT  
		Size: 46.7 MB (46723678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ab8837b0f778269986d4d09b2595189cd801706ebade92f33ca9260d77bffc`  
		Last Modified: Tue, 13 Jul 2021 21:22:44 GMT  
		Size: 736.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.5` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:9b1bc0857322e9d543d1ad0c2b7d1e060cd19db7ce2e553b5f9585cf8412eaf6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48936614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:695a7dc469f00769a8aa48b491a4541a37d820aa2967382749a1418d11d69558`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Mon, 16 Aug 2021 23:40:03 GMT
LABEL maintainer=Kong <support@konghq.com>
# Mon, 16 Aug 2021 23:40:03 GMT
ARG ASSET=ce
# Mon, 16 Aug 2021 23:40:03 GMT
ENV ASSET=ce
# Mon, 16 Aug 2021 23:40:04 GMT
ARG EE_PORTS
# Mon, 16 Aug 2021 23:40:04 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Mon, 16 Aug 2021 23:40:04 GMT
ARG KONG_VERSION=2.5.0
# Mon, 16 Aug 2021 23:40:04 GMT
ENV KONG_VERSION=2.5.0
# Mon, 16 Aug 2021 23:40:04 GMT
ARG KONG_AMD64_SHA=ebe0cf3a3e71d202774ede5083c98e2ae39fae0459d11140f53401a66527e1b7
# Mon, 16 Aug 2021 23:40:05 GMT
ENV KONG_AMD64_SHA=ebe0cf3a3e71d202774ede5083c98e2ae39fae0459d11140f53401a66527e1b7
# Mon, 16 Aug 2021 23:40:05 GMT
ARG KONG_ARM64_SHA=131964ce443f2d08dc98191fcc442867f2dee2f741ccee9cc519bb99c765f3cf
# Mon, 16 Aug 2021 23:40:05 GMT
ENV KONG_ARM64_SHA=131964ce443f2d08dc98191fcc442867f2dee2f741ccee9cc519bb99c765f3cf
# Mon, 16 Aug 2021 23:40:12 GMT
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Mon, 16 Aug 2021 23:40:13 GMT
COPY file:a9828df20ead648b4c991bfb67a40d0065e248e50a2ae98fad0104e78f32d234 in /docker-entrypoint.sh 
# Mon, 16 Aug 2021 23:40:13 GMT
USER kong
# Mon, 16 Aug 2021 23:40:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 16 Aug 2021 23:40:13 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 16 Aug 2021 23:40:13 GMT
STOPSIGNAL SIGQUIT
# Mon, 16 Aug 2021 23:40:14 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Mon, 16 Aug 2021 23:40:14 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16dfa7b57c17ad30d2ca84e453a222cceba322ba4e63c5f0236b1f657fd3ad09`  
		Last Modified: Mon, 16 Aug 2021 23:41:07 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef997f1b8b589b68d6ad13302768170cb1fdfbe0a4d50c40be58929b2b3cb22`  
		Last Modified: Mon, 16 Aug 2021 23:41:17 GMT  
		Size: 46.2 MB (46223721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01c1aa162f5e7767b889221779fe88330588720d3ddb3345752f8c08c70f849`  
		Last Modified: Mon, 16 Aug 2021 23:41:07 GMT  
		Size: 737.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.5-centos`

```console
$ docker pull kong@sha256:372f94e60ab235c10d72924ac7fdbee522f142235d9db4077c87376a9a61a85f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:2.5-centos` - linux; amd64

```console
$ docker pull kong@sha256:618987dc3e009862ed56756b9d519e89bf71695be2785956137d5a1371c7bb9c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127675275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7994889dce8690c91360f21c5404b0c5f69d6ddbacd17f8d396a62b95b3e3e7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 14 Nov 2020 00:20:04 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Sat, 14 Nov 2020 00:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:20:04 GMT
CMD ["/bin/bash"]
# Sat, 06 Mar 2021 07:32:08 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 06 Mar 2021 07:32:08 GMT
ARG ASSET=ce
# Sat, 06 Mar 2021 07:32:08 GMT
ENV ASSET=ce
# Sat, 06 Mar 2021 07:32:08 GMT
ARG EE_PORTS
# Sat, 06 Mar 2021 07:32:08 GMT
COPY file:ff02c070e4c89f043b176279a7e41464b5fab8cb98cfcd6332fad2d2741fc41d in /tmp/kong.rpm 
# Tue, 13 Jul 2021 21:21:32 GMT
ARG KONG_VERSION=2.5.0
# Tue, 13 Jul 2021 21:21:32 GMT
ENV KONG_VERSION=2.5.0
# Tue, 13 Jul 2021 21:21:33 GMT
ARG KONG_SHA256=87b789aed871991b92d264b02ceca3c66246c825c28dd71e73faac7293e43fa2
# Tue, 13 Jul 2021 21:22:06 GMT
# ARGS: KONG_SHA256=87b789aed871991b92d264b02ceca3c66246c825c28dd71e73faac7293e43fa2
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then       curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-centos-7/Packages/k/kong-$KONG_VERSION.el7.amd64.rpm -o /tmp/kong.rpm       && echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -;     fi;     yum install -y -q unzip shadow-utils git     && yum clean all -q     && rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki     && yum install -y /tmp/kong.rpm     && yum clean all     && rm /tmp/kong.rpm     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 13 Jul 2021 21:22:06 GMT
COPY file:a9828df20ead648b4c991bfb67a40d0065e248e50a2ae98fad0104e78f32d234 in /docker-entrypoint.sh 
# Tue, 13 Jul 2021 21:22:06 GMT
USER kong
# Tue, 13 Jul 2021 21:22:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 13 Jul 2021 21:22:07 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 13 Jul 2021 21:22:07 GMT
STOPSIGNAL SIGQUIT
# Tue, 13 Jul 2021 21:22:07 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 13 Jul 2021 21:22:07 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c237ce1272ffe51f7f4a890afaca88db75cb107611ffb1833c9dbd5161df8157`  
		Last Modified: Sat, 06 Mar 2021 07:39:18 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb6400158dfebf8d4f40060b5c19c9601601efc21b95b2ad987d96c8f7df150`  
		Last Modified: Tue, 13 Jul 2021 21:23:42 GMT  
		Size: 51.6 MB (51577255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c34fa922eb9655e29b08007b015e41025f72561d76196163819a303d86b125d`  
		Last Modified: Tue, 13 Jul 2021 21:23:32 GMT  
		Size: 735.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.5-ubuntu`

```console
$ docker pull kong@sha256:4f1b4ceceeb572651241f05b2e7b3f3555eb26dda5a8e826e22d970184614e99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.5-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:28a36065352062d1206113edd6fb0912a441af26517a7fa7a68d5d43f44a14b0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134774453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39c03fd01122d4fdc3c13f128aadfe3e605ccbf2fdee58cac4c3f12deb6ec2b5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 26 Jul 2021 21:22:15 GMT
ADD file:a94a87e268e99c78143fae5148bd1200bf0da90c0e7f42bd8c168bb205ccb105 in / 
# Mon, 26 Jul 2021 21:22:16 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 26 Jul 2021 21:22:17 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:22:17 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 26 Jul 2021 21:22:18 GMT
CMD ["/bin/bash"]
# Mon, 26 Jul 2021 23:28:42 GMT
ARG ASSET=ce
# Mon, 26 Jul 2021 23:28:43 GMT
ENV ASSET=ce
# Mon, 26 Jul 2021 23:28:43 GMT
ARG EE_PORTS
# Mon, 26 Jul 2021 23:28:43 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Mon, 26 Jul 2021 23:28:43 GMT
ARG KONG_VERSION=2.5.0
# Mon, 26 Jul 2021 23:28:44 GMT
ENV KONG_VERSION=2.5.0
# Mon, 26 Jul 2021 23:29:21 GMT
RUN set -ex     && apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)/pool/all/k/kong/kong_${KONG_VERSION}_$(dpkg --print-architecture).deb -o /tmp/kong.deb       && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Mon, 26 Jul 2021 23:29:22 GMT
COPY file:ae813ec19d3fef1de3793f6717c2aed3a9daa94e583e9e55448084541de3c5ff in /docker-entrypoint.sh 
# Mon, 26 Jul 2021 23:29:22 GMT
USER kong
# Mon, 26 Jul 2021 23:29:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 26 Jul 2021 23:29:22 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 26 Jul 2021 23:29:23 GMT
STOPSIGNAL SIGQUIT
# Mon, 26 Jul 2021 23:29:23 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Mon, 26 Jul 2021 23:29:23 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:52818491084148fa3469964bbcc3576686018a3b16b2e29be0407565c4c80b44`  
		Last Modified: Thu, 22 Jul 2021 16:25:00 GMT  
		Size: 46.5 MB (46497362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9df81d603d28f2a294b2f11b4f60d07b5b833b2ad7d6659a3f59b10cff2696`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636d9303bf663657be8e6796d720913bb985b5343da7949749ae1e72b54a88d8`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672b5bdcef61237567b311ad3d349f5eae18ba839ce2b204858a3083437a0a59`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdd2955c511e0c6bedd8d0fb726625f0608e6fa14d9361ab3e51b208d892ac8`  
		Last Modified: Mon, 26 Jul 2021 23:30:37 GMT  
		Size: 25.1 MB (25081965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc0be693280e7051fbb71d03c81d05245f8a69949feedbb9c4662d075ed577d`  
		Last Modified: Mon, 26 Jul 2021 23:30:46 GMT  
		Size: 63.2 MB (63192884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44bc8ec94b7019e19e92ec972623d439956fcdf9ae8e426fd6b2944440808fef`  
		Last Modified: Mon, 26 Jul 2021 23:30:35 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.5-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:7fb163125ba0769471c7adccc2609abcd37c3e58afcfb159ab99aa30f5ba58f2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125879708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8100ea3c312d55c4a34fcf3706f2584737cc61f1662715a6dd709d77d3f79138`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 31 Aug 2021 01:41:19 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Tue, 31 Aug 2021 01:41:20 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:41:20 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:41:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:41:21 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 03:13:00 GMT
ARG ASSET=ce
# Tue, 31 Aug 2021 03:13:00 GMT
ENV ASSET=ce
# Tue, 31 Aug 2021 03:13:00 GMT
ARG EE_PORTS
# Tue, 31 Aug 2021 03:13:00 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Tue, 31 Aug 2021 03:13:01 GMT
ARG KONG_VERSION=2.5.0
# Tue, 31 Aug 2021 03:13:01 GMT
ENV KONG_VERSION=2.5.0
# Tue, 31 Aug 2021 03:13:24 GMT
RUN set -ex     && apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)/pool/all/k/kong/kong_${KONG_VERSION}_$(dpkg --print-architecture).deb -o /tmp/kong.deb       && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 31 Aug 2021 03:13:25 GMT
COPY file:ae813ec19d3fef1de3793f6717c2aed3a9daa94e583e9e55448084541de3c5ff in /docker-entrypoint.sh 
# Tue, 31 Aug 2021 03:13:25 GMT
USER kong
# Tue, 31 Aug 2021 03:13:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:13:25 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 31 Aug 2021 03:13:26 GMT
STOPSIGNAL SIGQUIT
# Tue, 31 Aug 2021 03:13:26 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 31 Aug 2021 03:13:26 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85569e0c17003d9cf46a8b94076418863e0abfc5474bb830403acf246947fea7`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32ca509d28808ab7c61361835292ee8eddecd0c0949d658bde0ab1a77ecbf6e`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 469.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8168af71f81f1ffa234c301e9cc2ee87b560ad8b74ef4100f8ab4a6abf3a8ad3`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eee59a359925630cd377c9610b18f7d7797349cdbabeda7b8c8685852a5ff83`  
		Last Modified: Tue, 31 Aug 2021 03:14:48 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbbe71eb414d43ff3fbf75c0de9133ebafceaf672848c6e2c17e4ab47780e97b`  
		Last Modified: Tue, 31 Aug 2021 03:15:00 GMT  
		Size: 59.6 MB (59556314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a45ed64e5c35d56c7aafb050d22218142de8f6d3142eba9294d41638844747`  
		Last Modified: Tue, 31 Aug 2021 03:14:46 GMT  
		Size: 690.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.5.0`

```console
$ docker pull kong@sha256:eab7328f53373a47f04e1466eeee07cde8e0808c6f36067a068e554f436d1757
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.5.0` - linux; amd64

```console
$ docker pull kong@sha256:40d7a2eac255f47e1af9c30a5525230573aa9e120cf25cc6dcb7d6eb61cff38b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49536515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6ccc21c00cef6852bbf840402c7c92cd19d23882e66880b3c4b74fa7c48c6a7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Tue, 13 Jul 2021 21:20:05 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 13 Jul 2021 21:20:06 GMT
ARG ASSET=ce
# Tue, 13 Jul 2021 21:20:06 GMT
ENV ASSET=ce
# Tue, 13 Jul 2021 21:20:06 GMT
ARG EE_PORTS
# Tue, 13 Jul 2021 21:20:06 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 13 Jul 2021 21:20:06 GMT
ARG KONG_VERSION=2.5.0
# Tue, 13 Jul 2021 21:20:07 GMT
ENV KONG_VERSION=2.5.0
# Tue, 13 Jul 2021 21:20:07 GMT
ARG KONG_AMD64_SHA=ebe0cf3a3e71d202774ede5083c98e2ae39fae0459d11140f53401a66527e1b7
# Tue, 13 Jul 2021 21:20:07 GMT
ENV KONG_AMD64_SHA=ebe0cf3a3e71d202774ede5083c98e2ae39fae0459d11140f53401a66527e1b7
# Tue, 13 Jul 2021 21:20:07 GMT
ARG KONG_ARM64_SHA=131964ce443f2d08dc98191fcc442867f2dee2f741ccee9cc519bb99c765f3cf
# Tue, 13 Jul 2021 21:20:07 GMT
ENV KONG_ARM64_SHA=131964ce443f2d08dc98191fcc442867f2dee2f741ccee9cc519bb99c765f3cf
# Tue, 13 Jul 2021 21:20:15 GMT
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Tue, 13 Jul 2021 21:20:15 GMT
COPY file:a9828df20ead648b4c991bfb67a40d0065e248e50a2ae98fad0104e78f32d234 in /docker-entrypoint.sh 
# Tue, 13 Jul 2021 21:20:16 GMT
USER kong
# Tue, 13 Jul 2021 21:20:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 13 Jul 2021 21:20:16 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 13 Jul 2021 21:20:16 GMT
STOPSIGNAL SIGQUIT
# Tue, 13 Jul 2021 21:20:16 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 13 Jul 2021 21:20:17 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dcb869933b18a40e5829078fafe0a2045da1deafddf08550c6346d15353e9b`  
		Last Modified: Tue, 13 Jul 2021 21:22:43 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae5d676504a7ba5bcd7a66c7882841aa52368badcb077e8e97d40bb184cc27f`  
		Last Modified: Tue, 13 Jul 2021 21:22:51 GMT  
		Size: 46.7 MB (46723678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ab8837b0f778269986d4d09b2595189cd801706ebade92f33ca9260d77bffc`  
		Last Modified: Tue, 13 Jul 2021 21:22:44 GMT  
		Size: 736.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.5.0` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:9b1bc0857322e9d543d1ad0c2b7d1e060cd19db7ce2e553b5f9585cf8412eaf6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48936614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:695a7dc469f00769a8aa48b491a4541a37d820aa2967382749a1418d11d69558`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Mon, 16 Aug 2021 23:40:03 GMT
LABEL maintainer=Kong <support@konghq.com>
# Mon, 16 Aug 2021 23:40:03 GMT
ARG ASSET=ce
# Mon, 16 Aug 2021 23:40:03 GMT
ENV ASSET=ce
# Mon, 16 Aug 2021 23:40:04 GMT
ARG EE_PORTS
# Mon, 16 Aug 2021 23:40:04 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Mon, 16 Aug 2021 23:40:04 GMT
ARG KONG_VERSION=2.5.0
# Mon, 16 Aug 2021 23:40:04 GMT
ENV KONG_VERSION=2.5.0
# Mon, 16 Aug 2021 23:40:04 GMT
ARG KONG_AMD64_SHA=ebe0cf3a3e71d202774ede5083c98e2ae39fae0459d11140f53401a66527e1b7
# Mon, 16 Aug 2021 23:40:05 GMT
ENV KONG_AMD64_SHA=ebe0cf3a3e71d202774ede5083c98e2ae39fae0459d11140f53401a66527e1b7
# Mon, 16 Aug 2021 23:40:05 GMT
ARG KONG_ARM64_SHA=131964ce443f2d08dc98191fcc442867f2dee2f741ccee9cc519bb99c765f3cf
# Mon, 16 Aug 2021 23:40:05 GMT
ENV KONG_ARM64_SHA=131964ce443f2d08dc98191fcc442867f2dee2f741ccee9cc519bb99c765f3cf
# Mon, 16 Aug 2021 23:40:12 GMT
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Mon, 16 Aug 2021 23:40:13 GMT
COPY file:a9828df20ead648b4c991bfb67a40d0065e248e50a2ae98fad0104e78f32d234 in /docker-entrypoint.sh 
# Mon, 16 Aug 2021 23:40:13 GMT
USER kong
# Mon, 16 Aug 2021 23:40:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 16 Aug 2021 23:40:13 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 16 Aug 2021 23:40:13 GMT
STOPSIGNAL SIGQUIT
# Mon, 16 Aug 2021 23:40:14 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Mon, 16 Aug 2021 23:40:14 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16dfa7b57c17ad30d2ca84e453a222cceba322ba4e63c5f0236b1f657fd3ad09`  
		Last Modified: Mon, 16 Aug 2021 23:41:07 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef997f1b8b589b68d6ad13302768170cb1fdfbe0a4d50c40be58929b2b3cb22`  
		Last Modified: Mon, 16 Aug 2021 23:41:17 GMT  
		Size: 46.2 MB (46223721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01c1aa162f5e7767b889221779fe88330588720d3ddb3345752f8c08c70f849`  
		Last Modified: Mon, 16 Aug 2021 23:41:07 GMT  
		Size: 737.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.5.0-alpine`

```console
$ docker pull kong@sha256:eab7328f53373a47f04e1466eeee07cde8e0808c6f36067a068e554f436d1757
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.5.0-alpine` - linux; amd64

```console
$ docker pull kong@sha256:40d7a2eac255f47e1af9c30a5525230573aa9e120cf25cc6dcb7d6eb61cff38b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49536515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6ccc21c00cef6852bbf840402c7c92cd19d23882e66880b3c4b74fa7c48c6a7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Tue, 13 Jul 2021 21:20:05 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 13 Jul 2021 21:20:06 GMT
ARG ASSET=ce
# Tue, 13 Jul 2021 21:20:06 GMT
ENV ASSET=ce
# Tue, 13 Jul 2021 21:20:06 GMT
ARG EE_PORTS
# Tue, 13 Jul 2021 21:20:06 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 13 Jul 2021 21:20:06 GMT
ARG KONG_VERSION=2.5.0
# Tue, 13 Jul 2021 21:20:07 GMT
ENV KONG_VERSION=2.5.0
# Tue, 13 Jul 2021 21:20:07 GMT
ARG KONG_AMD64_SHA=ebe0cf3a3e71d202774ede5083c98e2ae39fae0459d11140f53401a66527e1b7
# Tue, 13 Jul 2021 21:20:07 GMT
ENV KONG_AMD64_SHA=ebe0cf3a3e71d202774ede5083c98e2ae39fae0459d11140f53401a66527e1b7
# Tue, 13 Jul 2021 21:20:07 GMT
ARG KONG_ARM64_SHA=131964ce443f2d08dc98191fcc442867f2dee2f741ccee9cc519bb99c765f3cf
# Tue, 13 Jul 2021 21:20:07 GMT
ENV KONG_ARM64_SHA=131964ce443f2d08dc98191fcc442867f2dee2f741ccee9cc519bb99c765f3cf
# Tue, 13 Jul 2021 21:20:15 GMT
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Tue, 13 Jul 2021 21:20:15 GMT
COPY file:a9828df20ead648b4c991bfb67a40d0065e248e50a2ae98fad0104e78f32d234 in /docker-entrypoint.sh 
# Tue, 13 Jul 2021 21:20:16 GMT
USER kong
# Tue, 13 Jul 2021 21:20:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 13 Jul 2021 21:20:16 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 13 Jul 2021 21:20:16 GMT
STOPSIGNAL SIGQUIT
# Tue, 13 Jul 2021 21:20:16 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 13 Jul 2021 21:20:17 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dcb869933b18a40e5829078fafe0a2045da1deafddf08550c6346d15353e9b`  
		Last Modified: Tue, 13 Jul 2021 21:22:43 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae5d676504a7ba5bcd7a66c7882841aa52368badcb077e8e97d40bb184cc27f`  
		Last Modified: Tue, 13 Jul 2021 21:22:51 GMT  
		Size: 46.7 MB (46723678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ab8837b0f778269986d4d09b2595189cd801706ebade92f33ca9260d77bffc`  
		Last Modified: Tue, 13 Jul 2021 21:22:44 GMT  
		Size: 736.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.5.0-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:9b1bc0857322e9d543d1ad0c2b7d1e060cd19db7ce2e553b5f9585cf8412eaf6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48936614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:695a7dc469f00769a8aa48b491a4541a37d820aa2967382749a1418d11d69558`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Mon, 16 Aug 2021 23:40:03 GMT
LABEL maintainer=Kong <support@konghq.com>
# Mon, 16 Aug 2021 23:40:03 GMT
ARG ASSET=ce
# Mon, 16 Aug 2021 23:40:03 GMT
ENV ASSET=ce
# Mon, 16 Aug 2021 23:40:04 GMT
ARG EE_PORTS
# Mon, 16 Aug 2021 23:40:04 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Mon, 16 Aug 2021 23:40:04 GMT
ARG KONG_VERSION=2.5.0
# Mon, 16 Aug 2021 23:40:04 GMT
ENV KONG_VERSION=2.5.0
# Mon, 16 Aug 2021 23:40:04 GMT
ARG KONG_AMD64_SHA=ebe0cf3a3e71d202774ede5083c98e2ae39fae0459d11140f53401a66527e1b7
# Mon, 16 Aug 2021 23:40:05 GMT
ENV KONG_AMD64_SHA=ebe0cf3a3e71d202774ede5083c98e2ae39fae0459d11140f53401a66527e1b7
# Mon, 16 Aug 2021 23:40:05 GMT
ARG KONG_ARM64_SHA=131964ce443f2d08dc98191fcc442867f2dee2f741ccee9cc519bb99c765f3cf
# Mon, 16 Aug 2021 23:40:05 GMT
ENV KONG_ARM64_SHA=131964ce443f2d08dc98191fcc442867f2dee2f741ccee9cc519bb99c765f3cf
# Mon, 16 Aug 2021 23:40:12 GMT
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Mon, 16 Aug 2021 23:40:13 GMT
COPY file:a9828df20ead648b4c991bfb67a40d0065e248e50a2ae98fad0104e78f32d234 in /docker-entrypoint.sh 
# Mon, 16 Aug 2021 23:40:13 GMT
USER kong
# Mon, 16 Aug 2021 23:40:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 16 Aug 2021 23:40:13 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 16 Aug 2021 23:40:13 GMT
STOPSIGNAL SIGQUIT
# Mon, 16 Aug 2021 23:40:14 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Mon, 16 Aug 2021 23:40:14 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16dfa7b57c17ad30d2ca84e453a222cceba322ba4e63c5f0236b1f657fd3ad09`  
		Last Modified: Mon, 16 Aug 2021 23:41:07 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef997f1b8b589b68d6ad13302768170cb1fdfbe0a4d50c40be58929b2b3cb22`  
		Last Modified: Mon, 16 Aug 2021 23:41:17 GMT  
		Size: 46.2 MB (46223721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01c1aa162f5e7767b889221779fe88330588720d3ddb3345752f8c08c70f849`  
		Last Modified: Mon, 16 Aug 2021 23:41:07 GMT  
		Size: 737.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.5.0-centos`

```console
$ docker pull kong@sha256:372f94e60ab235c10d72924ac7fdbee522f142235d9db4077c87376a9a61a85f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:2.5.0-centos` - linux; amd64

```console
$ docker pull kong@sha256:618987dc3e009862ed56756b9d519e89bf71695be2785956137d5a1371c7bb9c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127675275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7994889dce8690c91360f21c5404b0c5f69d6ddbacd17f8d396a62b95b3e3e7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 14 Nov 2020 00:20:04 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Sat, 14 Nov 2020 00:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:20:04 GMT
CMD ["/bin/bash"]
# Sat, 06 Mar 2021 07:32:08 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 06 Mar 2021 07:32:08 GMT
ARG ASSET=ce
# Sat, 06 Mar 2021 07:32:08 GMT
ENV ASSET=ce
# Sat, 06 Mar 2021 07:32:08 GMT
ARG EE_PORTS
# Sat, 06 Mar 2021 07:32:08 GMT
COPY file:ff02c070e4c89f043b176279a7e41464b5fab8cb98cfcd6332fad2d2741fc41d in /tmp/kong.rpm 
# Tue, 13 Jul 2021 21:21:32 GMT
ARG KONG_VERSION=2.5.0
# Tue, 13 Jul 2021 21:21:32 GMT
ENV KONG_VERSION=2.5.0
# Tue, 13 Jul 2021 21:21:33 GMT
ARG KONG_SHA256=87b789aed871991b92d264b02ceca3c66246c825c28dd71e73faac7293e43fa2
# Tue, 13 Jul 2021 21:22:06 GMT
# ARGS: KONG_SHA256=87b789aed871991b92d264b02ceca3c66246c825c28dd71e73faac7293e43fa2
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then       curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-centos-7/Packages/k/kong-$KONG_VERSION.el7.amd64.rpm -o /tmp/kong.rpm       && echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -;     fi;     yum install -y -q unzip shadow-utils git     && yum clean all -q     && rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki     && yum install -y /tmp/kong.rpm     && yum clean all     && rm /tmp/kong.rpm     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 13 Jul 2021 21:22:06 GMT
COPY file:a9828df20ead648b4c991bfb67a40d0065e248e50a2ae98fad0104e78f32d234 in /docker-entrypoint.sh 
# Tue, 13 Jul 2021 21:22:06 GMT
USER kong
# Tue, 13 Jul 2021 21:22:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 13 Jul 2021 21:22:07 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 13 Jul 2021 21:22:07 GMT
STOPSIGNAL SIGQUIT
# Tue, 13 Jul 2021 21:22:07 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 13 Jul 2021 21:22:07 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c237ce1272ffe51f7f4a890afaca88db75cb107611ffb1833c9dbd5161df8157`  
		Last Modified: Sat, 06 Mar 2021 07:39:18 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb6400158dfebf8d4f40060b5c19c9601601efc21b95b2ad987d96c8f7df150`  
		Last Modified: Tue, 13 Jul 2021 21:23:42 GMT  
		Size: 51.6 MB (51577255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c34fa922eb9655e29b08007b015e41025f72561d76196163819a303d86b125d`  
		Last Modified: Tue, 13 Jul 2021 21:23:32 GMT  
		Size: 735.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.5.0-ubuntu`

```console
$ docker pull kong@sha256:4f1b4ceceeb572651241f05b2e7b3f3555eb26dda5a8e826e22d970184614e99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.5.0-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:28a36065352062d1206113edd6fb0912a441af26517a7fa7a68d5d43f44a14b0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134774453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39c03fd01122d4fdc3c13f128aadfe3e605ccbf2fdee58cac4c3f12deb6ec2b5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 26 Jul 2021 21:22:15 GMT
ADD file:a94a87e268e99c78143fae5148bd1200bf0da90c0e7f42bd8c168bb205ccb105 in / 
# Mon, 26 Jul 2021 21:22:16 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 26 Jul 2021 21:22:17 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:22:17 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 26 Jul 2021 21:22:18 GMT
CMD ["/bin/bash"]
# Mon, 26 Jul 2021 23:28:42 GMT
ARG ASSET=ce
# Mon, 26 Jul 2021 23:28:43 GMT
ENV ASSET=ce
# Mon, 26 Jul 2021 23:28:43 GMT
ARG EE_PORTS
# Mon, 26 Jul 2021 23:28:43 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Mon, 26 Jul 2021 23:28:43 GMT
ARG KONG_VERSION=2.5.0
# Mon, 26 Jul 2021 23:28:44 GMT
ENV KONG_VERSION=2.5.0
# Mon, 26 Jul 2021 23:29:21 GMT
RUN set -ex     && apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)/pool/all/k/kong/kong_${KONG_VERSION}_$(dpkg --print-architecture).deb -o /tmp/kong.deb       && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Mon, 26 Jul 2021 23:29:22 GMT
COPY file:ae813ec19d3fef1de3793f6717c2aed3a9daa94e583e9e55448084541de3c5ff in /docker-entrypoint.sh 
# Mon, 26 Jul 2021 23:29:22 GMT
USER kong
# Mon, 26 Jul 2021 23:29:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 26 Jul 2021 23:29:22 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 26 Jul 2021 23:29:23 GMT
STOPSIGNAL SIGQUIT
# Mon, 26 Jul 2021 23:29:23 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Mon, 26 Jul 2021 23:29:23 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:52818491084148fa3469964bbcc3576686018a3b16b2e29be0407565c4c80b44`  
		Last Modified: Thu, 22 Jul 2021 16:25:00 GMT  
		Size: 46.5 MB (46497362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9df81d603d28f2a294b2f11b4f60d07b5b833b2ad7d6659a3f59b10cff2696`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636d9303bf663657be8e6796d720913bb985b5343da7949749ae1e72b54a88d8`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672b5bdcef61237567b311ad3d349f5eae18ba839ce2b204858a3083437a0a59`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdd2955c511e0c6bedd8d0fb726625f0608e6fa14d9361ab3e51b208d892ac8`  
		Last Modified: Mon, 26 Jul 2021 23:30:37 GMT  
		Size: 25.1 MB (25081965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc0be693280e7051fbb71d03c81d05245f8a69949feedbb9c4662d075ed577d`  
		Last Modified: Mon, 26 Jul 2021 23:30:46 GMT  
		Size: 63.2 MB (63192884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44bc8ec94b7019e19e92ec972623d439956fcdf9ae8e426fd6b2944440808fef`  
		Last Modified: Mon, 26 Jul 2021 23:30:35 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.5.0-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:7fb163125ba0769471c7adccc2609abcd37c3e58afcfb159ab99aa30f5ba58f2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125879708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8100ea3c312d55c4a34fcf3706f2584737cc61f1662715a6dd709d77d3f79138`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 31 Aug 2021 01:41:19 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Tue, 31 Aug 2021 01:41:20 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:41:20 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:41:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:41:21 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 03:13:00 GMT
ARG ASSET=ce
# Tue, 31 Aug 2021 03:13:00 GMT
ENV ASSET=ce
# Tue, 31 Aug 2021 03:13:00 GMT
ARG EE_PORTS
# Tue, 31 Aug 2021 03:13:00 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Tue, 31 Aug 2021 03:13:01 GMT
ARG KONG_VERSION=2.5.0
# Tue, 31 Aug 2021 03:13:01 GMT
ENV KONG_VERSION=2.5.0
# Tue, 31 Aug 2021 03:13:24 GMT
RUN set -ex     && apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)/pool/all/k/kong/kong_${KONG_VERSION}_$(dpkg --print-architecture).deb -o /tmp/kong.deb       && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 31 Aug 2021 03:13:25 GMT
COPY file:ae813ec19d3fef1de3793f6717c2aed3a9daa94e583e9e55448084541de3c5ff in /docker-entrypoint.sh 
# Tue, 31 Aug 2021 03:13:25 GMT
USER kong
# Tue, 31 Aug 2021 03:13:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:13:25 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 31 Aug 2021 03:13:26 GMT
STOPSIGNAL SIGQUIT
# Tue, 31 Aug 2021 03:13:26 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 31 Aug 2021 03:13:26 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85569e0c17003d9cf46a8b94076418863e0abfc5474bb830403acf246947fea7`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32ca509d28808ab7c61361835292ee8eddecd0c0949d658bde0ab1a77ecbf6e`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 469.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8168af71f81f1ffa234c301e9cc2ee87b560ad8b74ef4100f8ab4a6abf3a8ad3`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eee59a359925630cd377c9610b18f7d7797349cdbabeda7b8c8685852a5ff83`  
		Last Modified: Tue, 31 Aug 2021 03:14:48 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbbe71eb414d43ff3fbf75c0de9133ebafceaf672848c6e2c17e4ab47780e97b`  
		Last Modified: Tue, 31 Aug 2021 03:15:00 GMT  
		Size: 59.6 MB (59556314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a45ed64e5c35d56c7aafb050d22218142de8f6d3142eba9294d41638844747`  
		Last Modified: Tue, 31 Aug 2021 03:14:46 GMT  
		Size: 690.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:alpine`

```console
$ docker pull kong@sha256:eab7328f53373a47f04e1466eeee07cde8e0808c6f36067a068e554f436d1757
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:alpine` - linux; amd64

```console
$ docker pull kong@sha256:40d7a2eac255f47e1af9c30a5525230573aa9e120cf25cc6dcb7d6eb61cff38b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49536515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6ccc21c00cef6852bbf840402c7c92cd19d23882e66880b3c4b74fa7c48c6a7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Tue, 13 Jul 2021 21:20:05 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 13 Jul 2021 21:20:06 GMT
ARG ASSET=ce
# Tue, 13 Jul 2021 21:20:06 GMT
ENV ASSET=ce
# Tue, 13 Jul 2021 21:20:06 GMT
ARG EE_PORTS
# Tue, 13 Jul 2021 21:20:06 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 13 Jul 2021 21:20:06 GMT
ARG KONG_VERSION=2.5.0
# Tue, 13 Jul 2021 21:20:07 GMT
ENV KONG_VERSION=2.5.0
# Tue, 13 Jul 2021 21:20:07 GMT
ARG KONG_AMD64_SHA=ebe0cf3a3e71d202774ede5083c98e2ae39fae0459d11140f53401a66527e1b7
# Tue, 13 Jul 2021 21:20:07 GMT
ENV KONG_AMD64_SHA=ebe0cf3a3e71d202774ede5083c98e2ae39fae0459d11140f53401a66527e1b7
# Tue, 13 Jul 2021 21:20:07 GMT
ARG KONG_ARM64_SHA=131964ce443f2d08dc98191fcc442867f2dee2f741ccee9cc519bb99c765f3cf
# Tue, 13 Jul 2021 21:20:07 GMT
ENV KONG_ARM64_SHA=131964ce443f2d08dc98191fcc442867f2dee2f741ccee9cc519bb99c765f3cf
# Tue, 13 Jul 2021 21:20:15 GMT
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Tue, 13 Jul 2021 21:20:15 GMT
COPY file:a9828df20ead648b4c991bfb67a40d0065e248e50a2ae98fad0104e78f32d234 in /docker-entrypoint.sh 
# Tue, 13 Jul 2021 21:20:16 GMT
USER kong
# Tue, 13 Jul 2021 21:20:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 13 Jul 2021 21:20:16 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 13 Jul 2021 21:20:16 GMT
STOPSIGNAL SIGQUIT
# Tue, 13 Jul 2021 21:20:16 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 13 Jul 2021 21:20:17 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dcb869933b18a40e5829078fafe0a2045da1deafddf08550c6346d15353e9b`  
		Last Modified: Tue, 13 Jul 2021 21:22:43 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae5d676504a7ba5bcd7a66c7882841aa52368badcb077e8e97d40bb184cc27f`  
		Last Modified: Tue, 13 Jul 2021 21:22:51 GMT  
		Size: 46.7 MB (46723678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ab8837b0f778269986d4d09b2595189cd801706ebade92f33ca9260d77bffc`  
		Last Modified: Tue, 13 Jul 2021 21:22:44 GMT  
		Size: 736.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:9b1bc0857322e9d543d1ad0c2b7d1e060cd19db7ce2e553b5f9585cf8412eaf6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48936614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:695a7dc469f00769a8aa48b491a4541a37d820aa2967382749a1418d11d69558`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Mon, 16 Aug 2021 23:40:03 GMT
LABEL maintainer=Kong <support@konghq.com>
# Mon, 16 Aug 2021 23:40:03 GMT
ARG ASSET=ce
# Mon, 16 Aug 2021 23:40:03 GMT
ENV ASSET=ce
# Mon, 16 Aug 2021 23:40:04 GMT
ARG EE_PORTS
# Mon, 16 Aug 2021 23:40:04 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Mon, 16 Aug 2021 23:40:04 GMT
ARG KONG_VERSION=2.5.0
# Mon, 16 Aug 2021 23:40:04 GMT
ENV KONG_VERSION=2.5.0
# Mon, 16 Aug 2021 23:40:04 GMT
ARG KONG_AMD64_SHA=ebe0cf3a3e71d202774ede5083c98e2ae39fae0459d11140f53401a66527e1b7
# Mon, 16 Aug 2021 23:40:05 GMT
ENV KONG_AMD64_SHA=ebe0cf3a3e71d202774ede5083c98e2ae39fae0459d11140f53401a66527e1b7
# Mon, 16 Aug 2021 23:40:05 GMT
ARG KONG_ARM64_SHA=131964ce443f2d08dc98191fcc442867f2dee2f741ccee9cc519bb99c765f3cf
# Mon, 16 Aug 2021 23:40:05 GMT
ENV KONG_ARM64_SHA=131964ce443f2d08dc98191fcc442867f2dee2f741ccee9cc519bb99c765f3cf
# Mon, 16 Aug 2021 23:40:12 GMT
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Mon, 16 Aug 2021 23:40:13 GMT
COPY file:a9828df20ead648b4c991bfb67a40d0065e248e50a2ae98fad0104e78f32d234 in /docker-entrypoint.sh 
# Mon, 16 Aug 2021 23:40:13 GMT
USER kong
# Mon, 16 Aug 2021 23:40:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 16 Aug 2021 23:40:13 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 16 Aug 2021 23:40:13 GMT
STOPSIGNAL SIGQUIT
# Mon, 16 Aug 2021 23:40:14 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Mon, 16 Aug 2021 23:40:14 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16dfa7b57c17ad30d2ca84e453a222cceba322ba4e63c5f0236b1f657fd3ad09`  
		Last Modified: Mon, 16 Aug 2021 23:41:07 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef997f1b8b589b68d6ad13302768170cb1fdfbe0a4d50c40be58929b2b3cb22`  
		Last Modified: Mon, 16 Aug 2021 23:41:17 GMT  
		Size: 46.2 MB (46223721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01c1aa162f5e7767b889221779fe88330588720d3ddb3345752f8c08c70f849`  
		Last Modified: Mon, 16 Aug 2021 23:41:07 GMT  
		Size: 737.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:centos`

```console
$ docker pull kong@sha256:372f94e60ab235c10d72924ac7fdbee522f142235d9db4077c87376a9a61a85f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:centos` - linux; amd64

```console
$ docker pull kong@sha256:618987dc3e009862ed56756b9d519e89bf71695be2785956137d5a1371c7bb9c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127675275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7994889dce8690c91360f21c5404b0c5f69d6ddbacd17f8d396a62b95b3e3e7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 14 Nov 2020 00:20:04 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Sat, 14 Nov 2020 00:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:20:04 GMT
CMD ["/bin/bash"]
# Sat, 06 Mar 2021 07:32:08 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 06 Mar 2021 07:32:08 GMT
ARG ASSET=ce
# Sat, 06 Mar 2021 07:32:08 GMT
ENV ASSET=ce
# Sat, 06 Mar 2021 07:32:08 GMT
ARG EE_PORTS
# Sat, 06 Mar 2021 07:32:08 GMT
COPY file:ff02c070e4c89f043b176279a7e41464b5fab8cb98cfcd6332fad2d2741fc41d in /tmp/kong.rpm 
# Tue, 13 Jul 2021 21:21:32 GMT
ARG KONG_VERSION=2.5.0
# Tue, 13 Jul 2021 21:21:32 GMT
ENV KONG_VERSION=2.5.0
# Tue, 13 Jul 2021 21:21:33 GMT
ARG KONG_SHA256=87b789aed871991b92d264b02ceca3c66246c825c28dd71e73faac7293e43fa2
# Tue, 13 Jul 2021 21:22:06 GMT
# ARGS: KONG_SHA256=87b789aed871991b92d264b02ceca3c66246c825c28dd71e73faac7293e43fa2
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then       curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-centos-7/Packages/k/kong-$KONG_VERSION.el7.amd64.rpm -o /tmp/kong.rpm       && echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -;     fi;     yum install -y -q unzip shadow-utils git     && yum clean all -q     && rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki     && yum install -y /tmp/kong.rpm     && yum clean all     && rm /tmp/kong.rpm     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 13 Jul 2021 21:22:06 GMT
COPY file:a9828df20ead648b4c991bfb67a40d0065e248e50a2ae98fad0104e78f32d234 in /docker-entrypoint.sh 
# Tue, 13 Jul 2021 21:22:06 GMT
USER kong
# Tue, 13 Jul 2021 21:22:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 13 Jul 2021 21:22:07 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 13 Jul 2021 21:22:07 GMT
STOPSIGNAL SIGQUIT
# Tue, 13 Jul 2021 21:22:07 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 13 Jul 2021 21:22:07 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c237ce1272ffe51f7f4a890afaca88db75cb107611ffb1833c9dbd5161df8157`  
		Last Modified: Sat, 06 Mar 2021 07:39:18 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb6400158dfebf8d4f40060b5c19c9601601efc21b95b2ad987d96c8f7df150`  
		Last Modified: Tue, 13 Jul 2021 21:23:42 GMT  
		Size: 51.6 MB (51577255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c34fa922eb9655e29b08007b015e41025f72561d76196163819a303d86b125d`  
		Last Modified: Tue, 13 Jul 2021 21:23:32 GMT  
		Size: 735.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:latest`

```console
$ docker pull kong@sha256:eab7328f53373a47f04e1466eeee07cde8e0808c6f36067a068e554f436d1757
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:latest` - linux; amd64

```console
$ docker pull kong@sha256:40d7a2eac255f47e1af9c30a5525230573aa9e120cf25cc6dcb7d6eb61cff38b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49536515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6ccc21c00cef6852bbf840402c7c92cd19d23882e66880b3c4b74fa7c48c6a7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Tue, 13 Jul 2021 21:20:05 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 13 Jul 2021 21:20:06 GMT
ARG ASSET=ce
# Tue, 13 Jul 2021 21:20:06 GMT
ENV ASSET=ce
# Tue, 13 Jul 2021 21:20:06 GMT
ARG EE_PORTS
# Tue, 13 Jul 2021 21:20:06 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 13 Jul 2021 21:20:06 GMT
ARG KONG_VERSION=2.5.0
# Tue, 13 Jul 2021 21:20:07 GMT
ENV KONG_VERSION=2.5.0
# Tue, 13 Jul 2021 21:20:07 GMT
ARG KONG_AMD64_SHA=ebe0cf3a3e71d202774ede5083c98e2ae39fae0459d11140f53401a66527e1b7
# Tue, 13 Jul 2021 21:20:07 GMT
ENV KONG_AMD64_SHA=ebe0cf3a3e71d202774ede5083c98e2ae39fae0459d11140f53401a66527e1b7
# Tue, 13 Jul 2021 21:20:07 GMT
ARG KONG_ARM64_SHA=131964ce443f2d08dc98191fcc442867f2dee2f741ccee9cc519bb99c765f3cf
# Tue, 13 Jul 2021 21:20:07 GMT
ENV KONG_ARM64_SHA=131964ce443f2d08dc98191fcc442867f2dee2f741ccee9cc519bb99c765f3cf
# Tue, 13 Jul 2021 21:20:15 GMT
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Tue, 13 Jul 2021 21:20:15 GMT
COPY file:a9828df20ead648b4c991bfb67a40d0065e248e50a2ae98fad0104e78f32d234 in /docker-entrypoint.sh 
# Tue, 13 Jul 2021 21:20:16 GMT
USER kong
# Tue, 13 Jul 2021 21:20:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 13 Jul 2021 21:20:16 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 13 Jul 2021 21:20:16 GMT
STOPSIGNAL SIGQUIT
# Tue, 13 Jul 2021 21:20:16 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 13 Jul 2021 21:20:17 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dcb869933b18a40e5829078fafe0a2045da1deafddf08550c6346d15353e9b`  
		Last Modified: Tue, 13 Jul 2021 21:22:43 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae5d676504a7ba5bcd7a66c7882841aa52368badcb077e8e97d40bb184cc27f`  
		Last Modified: Tue, 13 Jul 2021 21:22:51 GMT  
		Size: 46.7 MB (46723678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ab8837b0f778269986d4d09b2595189cd801706ebade92f33ca9260d77bffc`  
		Last Modified: Tue, 13 Jul 2021 21:22:44 GMT  
		Size: 736.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:latest` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:9b1bc0857322e9d543d1ad0c2b7d1e060cd19db7ce2e553b5f9585cf8412eaf6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48936614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:695a7dc469f00769a8aa48b491a4541a37d820aa2967382749a1418d11d69558`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Mon, 16 Aug 2021 23:40:03 GMT
LABEL maintainer=Kong <support@konghq.com>
# Mon, 16 Aug 2021 23:40:03 GMT
ARG ASSET=ce
# Mon, 16 Aug 2021 23:40:03 GMT
ENV ASSET=ce
# Mon, 16 Aug 2021 23:40:04 GMT
ARG EE_PORTS
# Mon, 16 Aug 2021 23:40:04 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Mon, 16 Aug 2021 23:40:04 GMT
ARG KONG_VERSION=2.5.0
# Mon, 16 Aug 2021 23:40:04 GMT
ENV KONG_VERSION=2.5.0
# Mon, 16 Aug 2021 23:40:04 GMT
ARG KONG_AMD64_SHA=ebe0cf3a3e71d202774ede5083c98e2ae39fae0459d11140f53401a66527e1b7
# Mon, 16 Aug 2021 23:40:05 GMT
ENV KONG_AMD64_SHA=ebe0cf3a3e71d202774ede5083c98e2ae39fae0459d11140f53401a66527e1b7
# Mon, 16 Aug 2021 23:40:05 GMT
ARG KONG_ARM64_SHA=131964ce443f2d08dc98191fcc442867f2dee2f741ccee9cc519bb99c765f3cf
# Mon, 16 Aug 2021 23:40:05 GMT
ENV KONG_ARM64_SHA=131964ce443f2d08dc98191fcc442867f2dee2f741ccee9cc519bb99c765f3cf
# Mon, 16 Aug 2021 23:40:12 GMT
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Mon, 16 Aug 2021 23:40:13 GMT
COPY file:a9828df20ead648b4c991bfb67a40d0065e248e50a2ae98fad0104e78f32d234 in /docker-entrypoint.sh 
# Mon, 16 Aug 2021 23:40:13 GMT
USER kong
# Mon, 16 Aug 2021 23:40:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 16 Aug 2021 23:40:13 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 16 Aug 2021 23:40:13 GMT
STOPSIGNAL SIGQUIT
# Mon, 16 Aug 2021 23:40:14 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Mon, 16 Aug 2021 23:40:14 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16dfa7b57c17ad30d2ca84e453a222cceba322ba4e63c5f0236b1f657fd3ad09`  
		Last Modified: Mon, 16 Aug 2021 23:41:07 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef997f1b8b589b68d6ad13302768170cb1fdfbe0a4d50c40be58929b2b3cb22`  
		Last Modified: Mon, 16 Aug 2021 23:41:17 GMT  
		Size: 46.2 MB (46223721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01c1aa162f5e7767b889221779fe88330588720d3ddb3345752f8c08c70f849`  
		Last Modified: Mon, 16 Aug 2021 23:41:07 GMT  
		Size: 737.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:ubuntu`

```console
$ docker pull kong@sha256:4f1b4ceceeb572651241f05b2e7b3f3555eb26dda5a8e826e22d970184614e99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:28a36065352062d1206113edd6fb0912a441af26517a7fa7a68d5d43f44a14b0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134774453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39c03fd01122d4fdc3c13f128aadfe3e605ccbf2fdee58cac4c3f12deb6ec2b5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 26 Jul 2021 21:22:15 GMT
ADD file:a94a87e268e99c78143fae5148bd1200bf0da90c0e7f42bd8c168bb205ccb105 in / 
# Mon, 26 Jul 2021 21:22:16 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 26 Jul 2021 21:22:17 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:22:17 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 26 Jul 2021 21:22:18 GMT
CMD ["/bin/bash"]
# Mon, 26 Jul 2021 23:28:42 GMT
ARG ASSET=ce
# Mon, 26 Jul 2021 23:28:43 GMT
ENV ASSET=ce
# Mon, 26 Jul 2021 23:28:43 GMT
ARG EE_PORTS
# Mon, 26 Jul 2021 23:28:43 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Mon, 26 Jul 2021 23:28:43 GMT
ARG KONG_VERSION=2.5.0
# Mon, 26 Jul 2021 23:28:44 GMT
ENV KONG_VERSION=2.5.0
# Mon, 26 Jul 2021 23:29:21 GMT
RUN set -ex     && apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)/pool/all/k/kong/kong_${KONG_VERSION}_$(dpkg --print-architecture).deb -o /tmp/kong.deb       && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Mon, 26 Jul 2021 23:29:22 GMT
COPY file:ae813ec19d3fef1de3793f6717c2aed3a9daa94e583e9e55448084541de3c5ff in /docker-entrypoint.sh 
# Mon, 26 Jul 2021 23:29:22 GMT
USER kong
# Mon, 26 Jul 2021 23:29:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 26 Jul 2021 23:29:22 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 26 Jul 2021 23:29:23 GMT
STOPSIGNAL SIGQUIT
# Mon, 26 Jul 2021 23:29:23 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Mon, 26 Jul 2021 23:29:23 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:52818491084148fa3469964bbcc3576686018a3b16b2e29be0407565c4c80b44`  
		Last Modified: Thu, 22 Jul 2021 16:25:00 GMT  
		Size: 46.5 MB (46497362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9df81d603d28f2a294b2f11b4f60d07b5b833b2ad7d6659a3f59b10cff2696`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636d9303bf663657be8e6796d720913bb985b5343da7949749ae1e72b54a88d8`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672b5bdcef61237567b311ad3d349f5eae18ba839ce2b204858a3083437a0a59`  
		Last Modified: Mon, 26 Jul 2021 21:24:20 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdd2955c511e0c6bedd8d0fb726625f0608e6fa14d9361ab3e51b208d892ac8`  
		Last Modified: Mon, 26 Jul 2021 23:30:37 GMT  
		Size: 25.1 MB (25081965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc0be693280e7051fbb71d03c81d05245f8a69949feedbb9c4662d075ed577d`  
		Last Modified: Mon, 26 Jul 2021 23:30:46 GMT  
		Size: 63.2 MB (63192884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44bc8ec94b7019e19e92ec972623d439956fcdf9ae8e426fd6b2944440808fef`  
		Last Modified: Mon, 26 Jul 2021 23:30:35 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:7fb163125ba0769471c7adccc2609abcd37c3e58afcfb159ab99aa30f5ba58f2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125879708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8100ea3c312d55c4a34fcf3706f2584737cc61f1662715a6dd709d77d3f79138`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 31 Aug 2021 01:41:19 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Tue, 31 Aug 2021 01:41:20 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:41:20 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:41:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:41:21 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 03:13:00 GMT
ARG ASSET=ce
# Tue, 31 Aug 2021 03:13:00 GMT
ENV ASSET=ce
# Tue, 31 Aug 2021 03:13:00 GMT
ARG EE_PORTS
# Tue, 31 Aug 2021 03:13:00 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Tue, 31 Aug 2021 03:13:01 GMT
ARG KONG_VERSION=2.5.0
# Tue, 31 Aug 2021 03:13:01 GMT
ENV KONG_VERSION=2.5.0
# Tue, 31 Aug 2021 03:13:24 GMT
RUN set -ex     && apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)/pool/all/k/kong/kong_${KONG_VERSION}_$(dpkg --print-architecture).deb -o /tmp/kong.deb       && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 31 Aug 2021 03:13:25 GMT
COPY file:ae813ec19d3fef1de3793f6717c2aed3a9daa94e583e9e55448084541de3c5ff in /docker-entrypoint.sh 
# Tue, 31 Aug 2021 03:13:25 GMT
USER kong
# Tue, 31 Aug 2021 03:13:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:13:25 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 31 Aug 2021 03:13:26 GMT
STOPSIGNAL SIGQUIT
# Tue, 31 Aug 2021 03:13:26 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 31 Aug 2021 03:13:26 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85569e0c17003d9cf46a8b94076418863e0abfc5474bb830403acf246947fea7`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32ca509d28808ab7c61361835292ee8eddecd0c0949d658bde0ab1a77ecbf6e`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 469.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8168af71f81f1ffa234c301e9cc2ee87b560ad8b74ef4100f8ab4a6abf3a8ad3`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eee59a359925630cd377c9610b18f7d7797349cdbabeda7b8c8685852a5ff83`  
		Last Modified: Tue, 31 Aug 2021 03:14:48 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbbe71eb414d43ff3fbf75c0de9133ebafceaf672848c6e2c17e4ab47780e97b`  
		Last Modified: Tue, 31 Aug 2021 03:15:00 GMT  
		Size: 59.6 MB (59556314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a45ed64e5c35d56c7aafb050d22218142de8f6d3142eba9294d41638844747`  
		Last Modified: Tue, 31 Aug 2021 03:14:46 GMT  
		Size: 690.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
