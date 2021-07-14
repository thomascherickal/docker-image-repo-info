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
-	Platforms:
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
-	Platforms:
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
-	Platforms:
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
$ docker pull kong@sha256:84d82fdb8c6c70d4f42e429e44c229ceca18de6f687bdf3773fc2c3466c04664
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.4-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:4a65d877bfe21dd9c012c838cb5645cefc38b916aed6d30888ee5618f708c7e9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134751840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c87e8dc8ed7d78be3686e38c65814583d124bb9e1a596a3220f7400271d9d702`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:06 GMT
ADD file:4dd75f16753c9c921fd05b1d0ed5b425d74d87405a76a0b3afcbf9723a50d1ce in / 
# Thu, 17 Jun 2021 23:32:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:32:08 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:32:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:32:09 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 01:30:20 GMT
ARG ASSET=ce
# Fri, 18 Jun 2021 01:30:21 GMT
ENV ASSET=ce
# Fri, 18 Jun 2021 01:30:21 GMT
ARG EE_PORTS
# Fri, 18 Jun 2021 01:30:21 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Fri, 18 Jun 2021 01:30:21 GMT
ARG KONG_VERSION=2.4.1
# Fri, 18 Jun 2021 01:30:22 GMT
ENV KONG_VERSION=2.4.1
# Fri, 18 Jun 2021 01:30:47 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL 		https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-xenial/pool/all/k/kong/kong_${KONG_VERSION}_$(dpkg --print-architecture).deb -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Fri, 18 Jun 2021 01:30:47 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Fri, 18 Jun 2021 01:30:48 GMT
USER kong
# Fri, 18 Jun 2021 01:30:48 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 18 Jun 2021 01:30:48 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 18 Jun 2021 01:30:48 GMT
STOPSIGNAL SIGQUIT
# Fri, 18 Jun 2021 01:30:48 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:61e03ba1d4149ac4eb681c6bf75aef8ac4b3f0d6fbb08e9623c4089889396fc8`  
		Last Modified: Sat, 12 Jun 2021 00:25:16 GMT  
		Size: 46.5 MB (46496785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afb39f216bd4e336f9b78584bae0f6bcb77150107471d8d67d3b8abfbdea46a`  
		Last Modified: Thu, 17 Jun 2021 23:34:09 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e489abdc9f902f737bfef2c0c7ff5c35ca9b3ca11e73405a472f31a25f2dcc69`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999fff7bcc2450fcf1210182802f3907e35cd7cf7569568bd2a179b9144d9c57`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b286e31b43b25089a4c360a36546b5f01a9d41bbe333e3e0f5803d2ff8e602cc`  
		Last Modified: Fri, 18 Jun 2021 01:34:03 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83fbccc03c9787f35d084b8ad9d353aa4b799bca69b145f97705e99081eeea89`  
		Last Modified: Fri, 18 Jun 2021 01:34:12 GMT  
		Size: 63.2 MB (63170866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8dfd1fccb5682b460b959fd63d5df9e4954c217fa617b367dec4632a75b373a`  
		Last Modified: Fri, 18 Jun 2021 01:34:02 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.4-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:c41786dd4f3d369d00518f8d46cc1cf98a5bb659e2f7ccb34054bf2246147624
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125853532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:089c15009cd77c8bdc358200e0cf0d4b08f478d142706a2d620952f6e9434a0c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 17 Jun 2021 23:54:40 GMT
ADD file:2675f90ace0ec88b2cdadc737d15d701b544bf2113480e898d0014a79dca13c7 in / 
# Thu, 17 Jun 2021 23:54:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:54:42 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:54:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:54:43 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 00:54:45 GMT
ARG ASSET=ce
# Fri, 18 Jun 2021 00:54:46 GMT
ENV ASSET=ce
# Fri, 18 Jun 2021 00:54:46 GMT
ARG EE_PORTS
# Fri, 18 Jun 2021 00:54:46 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Fri, 18 Jun 2021 00:54:46 GMT
ARG KONG_VERSION=2.4.1
# Fri, 18 Jun 2021 00:54:47 GMT
ENV KONG_VERSION=2.4.1
# Fri, 18 Jun 2021 00:55:10 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL 		https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-xenial/pool/all/k/kong/kong_${KONG_VERSION}_$(dpkg --print-architecture).deb -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Fri, 18 Jun 2021 00:55:11 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Fri, 18 Jun 2021 00:55:11 GMT
USER kong
# Fri, 18 Jun 2021 00:55:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 18 Jun 2021 00:55:12 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 18 Jun 2021 00:55:12 GMT
STOPSIGNAL SIGQUIT
# Fri, 18 Jun 2021 00:55:12 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:e2a24739a48e2c634f94c2cb69ead6b0ff1c84cedd9624eb29560b83c3eb6e0e`  
		Last Modified: Sat, 12 Jun 2021 00:25:19 GMT  
		Size: 41.2 MB (41239907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6732798425e9389fa6bd92caa59cd7de853b4cf01a7166724e26a430ec7211f`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0af2bd04c3cb9d221318d494c05b29dd4b7c46886de97baee11fbd40723ab8`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835469060484e7130eb258c8dfae8e4b1f8035c63bba23ab6e4f3e9b53a6cf1e`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7302e93943a9631fdef59ad177b0107d5f43c9c973a7d408198c495c3e5e08e0`  
		Last Modified: Fri, 18 Jun 2021 00:58:48 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12dfe8750b0a843228ac7dd5922cb2b28b0fba6b3a94aaec0bedc7d1817c599`  
		Last Modified: Fri, 18 Jun 2021 00:58:58 GMT  
		Size: 59.5 MB (59529495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b84e6de14f4fc064e108b6824bd8057aeb9e3f152a9dfaf28c0d4b779ad0f9`  
		Last Modified: Fri, 18 Jun 2021 00:58:46 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.4.1`

```console
$ docker pull kong@sha256:c9872460e6c9cb05d5ac1f125fff571c00541d4da7438f5eb821e07a56efe752
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
-	Platforms:
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
-	Platforms:
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
$ docker pull kong@sha256:84d82fdb8c6c70d4f42e429e44c229ceca18de6f687bdf3773fc2c3466c04664
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.4.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:4a65d877bfe21dd9c012c838cb5645cefc38b916aed6d30888ee5618f708c7e9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134751840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c87e8dc8ed7d78be3686e38c65814583d124bb9e1a596a3220f7400271d9d702`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:06 GMT
ADD file:4dd75f16753c9c921fd05b1d0ed5b425d74d87405a76a0b3afcbf9723a50d1ce in / 
# Thu, 17 Jun 2021 23:32:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:32:08 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:32:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:32:09 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 01:30:20 GMT
ARG ASSET=ce
# Fri, 18 Jun 2021 01:30:21 GMT
ENV ASSET=ce
# Fri, 18 Jun 2021 01:30:21 GMT
ARG EE_PORTS
# Fri, 18 Jun 2021 01:30:21 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Fri, 18 Jun 2021 01:30:21 GMT
ARG KONG_VERSION=2.4.1
# Fri, 18 Jun 2021 01:30:22 GMT
ENV KONG_VERSION=2.4.1
# Fri, 18 Jun 2021 01:30:47 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL 		https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-xenial/pool/all/k/kong/kong_${KONG_VERSION}_$(dpkg --print-architecture).deb -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Fri, 18 Jun 2021 01:30:47 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Fri, 18 Jun 2021 01:30:48 GMT
USER kong
# Fri, 18 Jun 2021 01:30:48 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 18 Jun 2021 01:30:48 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 18 Jun 2021 01:30:48 GMT
STOPSIGNAL SIGQUIT
# Fri, 18 Jun 2021 01:30:48 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:61e03ba1d4149ac4eb681c6bf75aef8ac4b3f0d6fbb08e9623c4089889396fc8`  
		Last Modified: Sat, 12 Jun 2021 00:25:16 GMT  
		Size: 46.5 MB (46496785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afb39f216bd4e336f9b78584bae0f6bcb77150107471d8d67d3b8abfbdea46a`  
		Last Modified: Thu, 17 Jun 2021 23:34:09 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e489abdc9f902f737bfef2c0c7ff5c35ca9b3ca11e73405a472f31a25f2dcc69`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999fff7bcc2450fcf1210182802f3907e35cd7cf7569568bd2a179b9144d9c57`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b286e31b43b25089a4c360a36546b5f01a9d41bbe333e3e0f5803d2ff8e602cc`  
		Last Modified: Fri, 18 Jun 2021 01:34:03 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83fbccc03c9787f35d084b8ad9d353aa4b799bca69b145f97705e99081eeea89`  
		Last Modified: Fri, 18 Jun 2021 01:34:12 GMT  
		Size: 63.2 MB (63170866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8dfd1fccb5682b460b959fd63d5df9e4954c217fa617b367dec4632a75b373a`  
		Last Modified: Fri, 18 Jun 2021 01:34:02 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.4.1-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:c41786dd4f3d369d00518f8d46cc1cf98a5bb659e2f7ccb34054bf2246147624
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125853532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:089c15009cd77c8bdc358200e0cf0d4b08f478d142706a2d620952f6e9434a0c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 17 Jun 2021 23:54:40 GMT
ADD file:2675f90ace0ec88b2cdadc737d15d701b544bf2113480e898d0014a79dca13c7 in / 
# Thu, 17 Jun 2021 23:54:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:54:42 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:54:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:54:43 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 00:54:45 GMT
ARG ASSET=ce
# Fri, 18 Jun 2021 00:54:46 GMT
ENV ASSET=ce
# Fri, 18 Jun 2021 00:54:46 GMT
ARG EE_PORTS
# Fri, 18 Jun 2021 00:54:46 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Fri, 18 Jun 2021 00:54:46 GMT
ARG KONG_VERSION=2.4.1
# Fri, 18 Jun 2021 00:54:47 GMT
ENV KONG_VERSION=2.4.1
# Fri, 18 Jun 2021 00:55:10 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL 		https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-xenial/pool/all/k/kong/kong_${KONG_VERSION}_$(dpkg --print-architecture).deb -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Fri, 18 Jun 2021 00:55:11 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Fri, 18 Jun 2021 00:55:11 GMT
USER kong
# Fri, 18 Jun 2021 00:55:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 18 Jun 2021 00:55:12 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 18 Jun 2021 00:55:12 GMT
STOPSIGNAL SIGQUIT
# Fri, 18 Jun 2021 00:55:12 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:e2a24739a48e2c634f94c2cb69ead6b0ff1c84cedd9624eb29560b83c3eb6e0e`  
		Last Modified: Sat, 12 Jun 2021 00:25:19 GMT  
		Size: 41.2 MB (41239907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6732798425e9389fa6bd92caa59cd7de853b4cf01a7166724e26a430ec7211f`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0af2bd04c3cb9d221318d494c05b29dd4b7c46886de97baee11fbd40723ab8`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835469060484e7130eb258c8dfae8e4b1f8035c63bba23ab6e4f3e9b53a6cf1e`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7302e93943a9631fdef59ad177b0107d5f43c9c973a7d408198c495c3e5e08e0`  
		Last Modified: Fri, 18 Jun 2021 00:58:48 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12dfe8750b0a843228ac7dd5922cb2b28b0fba6b3a94aaec0bedc7d1817c599`  
		Last Modified: Fri, 18 Jun 2021 00:58:58 GMT  
		Size: 59.5 MB (59529495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b84e6de14f4fc064e108b6824bd8057aeb9e3f152a9dfaf28c0d4b779ad0f9`  
		Last Modified: Fri, 18 Jun 2021 00:58:46 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.5`

```console
$ docker pull kong@sha256:7a33695e8c817dbc8776d5c8d0167457893d151b6c66f10ef52650d06db2334d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

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

## `kong:2.5-centos`

```console
$ docker pull kong@sha256:372f94e60ab235c10d72924ac7fdbee522f142235d9db4077c87376a9a61a85f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
$ docker pull kong@sha256:70c2e29713139f3a4fc04cb8f8f439bd4420035b78fc0622c7a467175294abff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.5-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:f3dce9e6f7d732ff292a7dfb69e3e49f54c9671bbf4ef362452cde57768f333b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134773988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d0c2b45772b0928fe051f937159565a9d4cdd2c38b23d9563388333a79085ef`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:06 GMT
ADD file:4dd75f16753c9c921fd05b1d0ed5b425d74d87405a76a0b3afcbf9723a50d1ce in / 
# Thu, 17 Jun 2021 23:32:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:32:08 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:32:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:32:09 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 01:30:20 GMT
ARG ASSET=ce
# Fri, 18 Jun 2021 01:30:21 GMT
ENV ASSET=ce
# Fri, 18 Jun 2021 01:30:21 GMT
ARG EE_PORTS
# Fri, 18 Jun 2021 01:30:21 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Tue, 13 Jul 2021 21:20:21 GMT
ARG KONG_VERSION=2.5.0
# Tue, 13 Jul 2021 21:20:21 GMT
ENV KONG_VERSION=2.5.0
# Tue, 13 Jul 2021 21:21:24 GMT
RUN set -ex     && apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)/pool/all/k/kong/kong_${KONG_VERSION}_$(dpkg --print-architecture).deb -o /tmp/kong.deb       && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 13 Jul 2021 21:21:25 GMT
COPY file:ae813ec19d3fef1de3793f6717c2aed3a9daa94e583e9e55448084541de3c5ff in /docker-entrypoint.sh 
# Tue, 13 Jul 2021 21:21:25 GMT
USER kong
# Tue, 13 Jul 2021 21:21:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 13 Jul 2021 21:21:25 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 13 Jul 2021 21:21:26 GMT
STOPSIGNAL SIGQUIT
# Tue, 13 Jul 2021 21:21:26 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 13 Jul 2021 21:21:26 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:61e03ba1d4149ac4eb681c6bf75aef8ac4b3f0d6fbb08e9623c4089889396fc8`  
		Last Modified: Sat, 12 Jun 2021 00:25:16 GMT  
		Size: 46.5 MB (46496785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afb39f216bd4e336f9b78584bae0f6bcb77150107471d8d67d3b8abfbdea46a`  
		Last Modified: Thu, 17 Jun 2021 23:34:09 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e489abdc9f902f737bfef2c0c7ff5c35ca9b3ca11e73405a472f31a25f2dcc69`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999fff7bcc2450fcf1210182802f3907e35cd7cf7569568bd2a179b9144d9c57`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b286e31b43b25089a4c360a36546b5f01a9d41bbe333e3e0f5803d2ff8e602cc`  
		Last Modified: Fri, 18 Jun 2021 01:34:03 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0dd9b55b05ae8a9ce66301dfc04a0b2b2fe6810bcc25bb4bb3fdea5c0b3089`  
		Last Modified: Tue, 13 Jul 2021 21:23:19 GMT  
		Size: 63.2 MB (63193012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13cbd93a408a8bffea0f11a600e891756637f2ecea6920be6f2345f2c7b0b276`  
		Last Modified: Tue, 13 Jul 2021 21:23:09 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.5-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:58dc824fdddab726be644c8f32057b76e43f703776cea8d0424b01e689a31403
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125880731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16eda571d3f969713cea3c32a98457ce85d7a4f6a1396d3e93855909921a0b3e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 17 Jun 2021 23:54:40 GMT
ADD file:2675f90ace0ec88b2cdadc737d15d701b544bf2113480e898d0014a79dca13c7 in / 
# Thu, 17 Jun 2021 23:54:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:54:42 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:54:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:54:43 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 00:54:45 GMT
ARG ASSET=ce
# Fri, 18 Jun 2021 00:54:46 GMT
ENV ASSET=ce
# Fri, 18 Jun 2021 00:54:46 GMT
ARG EE_PORTS
# Fri, 18 Jun 2021 00:54:46 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Tue, 13 Jul 2021 21:49:56 GMT
ARG KONG_VERSION=2.5.0
# Tue, 13 Jul 2021 21:49:57 GMT
ENV KONG_VERSION=2.5.0
# Tue, 13 Jul 2021 21:50:21 GMT
RUN set -ex     && apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)/pool/all/k/kong/kong_${KONG_VERSION}_$(dpkg --print-architecture).deb -o /tmp/kong.deb       && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 13 Jul 2021 21:50:22 GMT
COPY file:ae813ec19d3fef1de3793f6717c2aed3a9daa94e583e9e55448084541de3c5ff in /docker-entrypoint.sh 
# Tue, 13 Jul 2021 21:50:22 GMT
USER kong
# Tue, 13 Jul 2021 21:50:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 13 Jul 2021 21:50:22 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 13 Jul 2021 21:50:22 GMT
STOPSIGNAL SIGQUIT
# Tue, 13 Jul 2021 21:50:23 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 13 Jul 2021 21:50:23 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:e2a24739a48e2c634f94c2cb69ead6b0ff1c84cedd9624eb29560b83c3eb6e0e`  
		Last Modified: Sat, 12 Jun 2021 00:25:19 GMT  
		Size: 41.2 MB (41239907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6732798425e9389fa6bd92caa59cd7de853b4cf01a7166724e26a430ec7211f`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0af2bd04c3cb9d221318d494c05b29dd4b7c46886de97baee11fbd40723ab8`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835469060484e7130eb258c8dfae8e4b1f8035c63bba23ab6e4f3e9b53a6cf1e`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7302e93943a9631fdef59ad177b0107d5f43c9c973a7d408198c495c3e5e08e0`  
		Last Modified: Fri, 18 Jun 2021 00:58:48 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c005bece33df94bb23fa7b6060342df594b8fb0f6ecbd345d7b8af860c00ad33`  
		Last Modified: Tue, 13 Jul 2021 21:51:12 GMT  
		Size: 59.6 MB (59556692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5273527be6c52184bf5b03f7f43830dd98fd33a5512f0a39ab4c5a1903dbbec`  
		Last Modified: Tue, 13 Jul 2021 21:51:00 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.5.0`

```console
$ docker pull kong@sha256:7a33695e8c817dbc8776d5c8d0167457893d151b6c66f10ef52650d06db2334d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

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

## `kong:2.5.0-alpine`

```console
$ docker pull kong@sha256:7a33695e8c817dbc8776d5c8d0167457893d151b6c66f10ef52650d06db2334d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

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

## `kong:2.5.0-centos`

```console
$ docker pull kong@sha256:372f94e60ab235c10d72924ac7fdbee522f142235d9db4077c87376a9a61a85f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
$ docker pull kong@sha256:70c2e29713139f3a4fc04cb8f8f439bd4420035b78fc0622c7a467175294abff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.5.0-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:f3dce9e6f7d732ff292a7dfb69e3e49f54c9671bbf4ef362452cde57768f333b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134773988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d0c2b45772b0928fe051f937159565a9d4cdd2c38b23d9563388333a79085ef`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:06 GMT
ADD file:4dd75f16753c9c921fd05b1d0ed5b425d74d87405a76a0b3afcbf9723a50d1ce in / 
# Thu, 17 Jun 2021 23:32:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:32:08 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:32:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:32:09 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 01:30:20 GMT
ARG ASSET=ce
# Fri, 18 Jun 2021 01:30:21 GMT
ENV ASSET=ce
# Fri, 18 Jun 2021 01:30:21 GMT
ARG EE_PORTS
# Fri, 18 Jun 2021 01:30:21 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Tue, 13 Jul 2021 21:20:21 GMT
ARG KONG_VERSION=2.5.0
# Tue, 13 Jul 2021 21:20:21 GMT
ENV KONG_VERSION=2.5.0
# Tue, 13 Jul 2021 21:21:24 GMT
RUN set -ex     && apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)/pool/all/k/kong/kong_${KONG_VERSION}_$(dpkg --print-architecture).deb -o /tmp/kong.deb       && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 13 Jul 2021 21:21:25 GMT
COPY file:ae813ec19d3fef1de3793f6717c2aed3a9daa94e583e9e55448084541de3c5ff in /docker-entrypoint.sh 
# Tue, 13 Jul 2021 21:21:25 GMT
USER kong
# Tue, 13 Jul 2021 21:21:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 13 Jul 2021 21:21:25 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 13 Jul 2021 21:21:26 GMT
STOPSIGNAL SIGQUIT
# Tue, 13 Jul 2021 21:21:26 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 13 Jul 2021 21:21:26 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:61e03ba1d4149ac4eb681c6bf75aef8ac4b3f0d6fbb08e9623c4089889396fc8`  
		Last Modified: Sat, 12 Jun 2021 00:25:16 GMT  
		Size: 46.5 MB (46496785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afb39f216bd4e336f9b78584bae0f6bcb77150107471d8d67d3b8abfbdea46a`  
		Last Modified: Thu, 17 Jun 2021 23:34:09 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e489abdc9f902f737bfef2c0c7ff5c35ca9b3ca11e73405a472f31a25f2dcc69`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999fff7bcc2450fcf1210182802f3907e35cd7cf7569568bd2a179b9144d9c57`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b286e31b43b25089a4c360a36546b5f01a9d41bbe333e3e0f5803d2ff8e602cc`  
		Last Modified: Fri, 18 Jun 2021 01:34:03 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0dd9b55b05ae8a9ce66301dfc04a0b2b2fe6810bcc25bb4bb3fdea5c0b3089`  
		Last Modified: Tue, 13 Jul 2021 21:23:19 GMT  
		Size: 63.2 MB (63193012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13cbd93a408a8bffea0f11a600e891756637f2ecea6920be6f2345f2c7b0b276`  
		Last Modified: Tue, 13 Jul 2021 21:23:09 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.5.0-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:58dc824fdddab726be644c8f32057b76e43f703776cea8d0424b01e689a31403
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125880731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16eda571d3f969713cea3c32a98457ce85d7a4f6a1396d3e93855909921a0b3e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 17 Jun 2021 23:54:40 GMT
ADD file:2675f90ace0ec88b2cdadc737d15d701b544bf2113480e898d0014a79dca13c7 in / 
# Thu, 17 Jun 2021 23:54:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:54:42 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:54:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:54:43 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 00:54:45 GMT
ARG ASSET=ce
# Fri, 18 Jun 2021 00:54:46 GMT
ENV ASSET=ce
# Fri, 18 Jun 2021 00:54:46 GMT
ARG EE_PORTS
# Fri, 18 Jun 2021 00:54:46 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Tue, 13 Jul 2021 21:49:56 GMT
ARG KONG_VERSION=2.5.0
# Tue, 13 Jul 2021 21:49:57 GMT
ENV KONG_VERSION=2.5.0
# Tue, 13 Jul 2021 21:50:21 GMT
RUN set -ex     && apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)/pool/all/k/kong/kong_${KONG_VERSION}_$(dpkg --print-architecture).deb -o /tmp/kong.deb       && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 13 Jul 2021 21:50:22 GMT
COPY file:ae813ec19d3fef1de3793f6717c2aed3a9daa94e583e9e55448084541de3c5ff in /docker-entrypoint.sh 
# Tue, 13 Jul 2021 21:50:22 GMT
USER kong
# Tue, 13 Jul 2021 21:50:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 13 Jul 2021 21:50:22 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 13 Jul 2021 21:50:22 GMT
STOPSIGNAL SIGQUIT
# Tue, 13 Jul 2021 21:50:23 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 13 Jul 2021 21:50:23 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:e2a24739a48e2c634f94c2cb69ead6b0ff1c84cedd9624eb29560b83c3eb6e0e`  
		Last Modified: Sat, 12 Jun 2021 00:25:19 GMT  
		Size: 41.2 MB (41239907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6732798425e9389fa6bd92caa59cd7de853b4cf01a7166724e26a430ec7211f`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0af2bd04c3cb9d221318d494c05b29dd4b7c46886de97baee11fbd40723ab8`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835469060484e7130eb258c8dfae8e4b1f8035c63bba23ab6e4f3e9b53a6cf1e`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7302e93943a9631fdef59ad177b0107d5f43c9c973a7d408198c495c3e5e08e0`  
		Last Modified: Fri, 18 Jun 2021 00:58:48 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c005bece33df94bb23fa7b6060342df594b8fb0f6ecbd345d7b8af860c00ad33`  
		Last Modified: Tue, 13 Jul 2021 21:51:12 GMT  
		Size: 59.6 MB (59556692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5273527be6c52184bf5b03f7f43830dd98fd33a5512f0a39ab4c5a1903dbbec`  
		Last Modified: Tue, 13 Jul 2021 21:51:00 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:alpine`

```console
$ docker pull kong@sha256:7a33695e8c817dbc8776d5c8d0167457893d151b6c66f10ef52650d06db2334d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

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

## `kong:centos`

```console
$ docker pull kong@sha256:372f94e60ab235c10d72924ac7fdbee522f142235d9db4077c87376a9a61a85f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
$ docker pull kong@sha256:7a33695e8c817dbc8776d5c8d0167457893d151b6c66f10ef52650d06db2334d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

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

## `kong:ubuntu`

```console
$ docker pull kong@sha256:70c2e29713139f3a4fc04cb8f8f439bd4420035b78fc0622c7a467175294abff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:f3dce9e6f7d732ff292a7dfb69e3e49f54c9671bbf4ef362452cde57768f333b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134773988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d0c2b45772b0928fe051f937159565a9d4cdd2c38b23d9563388333a79085ef`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:06 GMT
ADD file:4dd75f16753c9c921fd05b1d0ed5b425d74d87405a76a0b3afcbf9723a50d1ce in / 
# Thu, 17 Jun 2021 23:32:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:32:08 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:32:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:32:09 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 01:30:20 GMT
ARG ASSET=ce
# Fri, 18 Jun 2021 01:30:21 GMT
ENV ASSET=ce
# Fri, 18 Jun 2021 01:30:21 GMT
ARG EE_PORTS
# Fri, 18 Jun 2021 01:30:21 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Tue, 13 Jul 2021 21:20:21 GMT
ARG KONG_VERSION=2.5.0
# Tue, 13 Jul 2021 21:20:21 GMT
ENV KONG_VERSION=2.5.0
# Tue, 13 Jul 2021 21:21:24 GMT
RUN set -ex     && apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)/pool/all/k/kong/kong_${KONG_VERSION}_$(dpkg --print-architecture).deb -o /tmp/kong.deb       && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 13 Jul 2021 21:21:25 GMT
COPY file:ae813ec19d3fef1de3793f6717c2aed3a9daa94e583e9e55448084541de3c5ff in /docker-entrypoint.sh 
# Tue, 13 Jul 2021 21:21:25 GMT
USER kong
# Tue, 13 Jul 2021 21:21:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 13 Jul 2021 21:21:25 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 13 Jul 2021 21:21:26 GMT
STOPSIGNAL SIGQUIT
# Tue, 13 Jul 2021 21:21:26 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 13 Jul 2021 21:21:26 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:61e03ba1d4149ac4eb681c6bf75aef8ac4b3f0d6fbb08e9623c4089889396fc8`  
		Last Modified: Sat, 12 Jun 2021 00:25:16 GMT  
		Size: 46.5 MB (46496785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afb39f216bd4e336f9b78584bae0f6bcb77150107471d8d67d3b8abfbdea46a`  
		Last Modified: Thu, 17 Jun 2021 23:34:09 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e489abdc9f902f737bfef2c0c7ff5c35ca9b3ca11e73405a472f31a25f2dcc69`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999fff7bcc2450fcf1210182802f3907e35cd7cf7569568bd2a179b9144d9c57`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b286e31b43b25089a4c360a36546b5f01a9d41bbe333e3e0f5803d2ff8e602cc`  
		Last Modified: Fri, 18 Jun 2021 01:34:03 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0dd9b55b05ae8a9ce66301dfc04a0b2b2fe6810bcc25bb4bb3fdea5c0b3089`  
		Last Modified: Tue, 13 Jul 2021 21:23:19 GMT  
		Size: 63.2 MB (63193012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13cbd93a408a8bffea0f11a600e891756637f2ecea6920be6f2345f2c7b0b276`  
		Last Modified: Tue, 13 Jul 2021 21:23:09 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:58dc824fdddab726be644c8f32057b76e43f703776cea8d0424b01e689a31403
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125880731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16eda571d3f969713cea3c32a98457ce85d7a4f6a1396d3e93855909921a0b3e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 17 Jun 2021 23:54:40 GMT
ADD file:2675f90ace0ec88b2cdadc737d15d701b544bf2113480e898d0014a79dca13c7 in / 
# Thu, 17 Jun 2021 23:54:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:54:42 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:54:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:54:43 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 00:54:45 GMT
ARG ASSET=ce
# Fri, 18 Jun 2021 00:54:46 GMT
ENV ASSET=ce
# Fri, 18 Jun 2021 00:54:46 GMT
ARG EE_PORTS
# Fri, 18 Jun 2021 00:54:46 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Tue, 13 Jul 2021 21:49:56 GMT
ARG KONG_VERSION=2.5.0
# Tue, 13 Jul 2021 21:49:57 GMT
ENV KONG_VERSION=2.5.0
# Tue, 13 Jul 2021 21:50:21 GMT
RUN set -ex     && apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)/pool/all/k/kong/kong_${KONG_VERSION}_$(dpkg --print-architecture).deb -o /tmp/kong.deb       && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 13 Jul 2021 21:50:22 GMT
COPY file:ae813ec19d3fef1de3793f6717c2aed3a9daa94e583e9e55448084541de3c5ff in /docker-entrypoint.sh 
# Tue, 13 Jul 2021 21:50:22 GMT
USER kong
# Tue, 13 Jul 2021 21:50:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 13 Jul 2021 21:50:22 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 13 Jul 2021 21:50:22 GMT
STOPSIGNAL SIGQUIT
# Tue, 13 Jul 2021 21:50:23 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 13 Jul 2021 21:50:23 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:e2a24739a48e2c634f94c2cb69ead6b0ff1c84cedd9624eb29560b83c3eb6e0e`  
		Last Modified: Sat, 12 Jun 2021 00:25:19 GMT  
		Size: 41.2 MB (41239907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6732798425e9389fa6bd92caa59cd7de853b4cf01a7166724e26a430ec7211f`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0af2bd04c3cb9d221318d494c05b29dd4b7c46886de97baee11fbd40723ab8`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835469060484e7130eb258c8dfae8e4b1f8035c63bba23ab6e4f3e9b53a6cf1e`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7302e93943a9631fdef59ad177b0107d5f43c9c973a7d408198c495c3e5e08e0`  
		Last Modified: Fri, 18 Jun 2021 00:58:48 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c005bece33df94bb23fa7b6060342df594b8fb0f6ecbd345d7b8af860c00ad33`  
		Last Modified: Tue, 13 Jul 2021 21:51:12 GMT  
		Size: 59.6 MB (59556692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5273527be6c52184bf5b03f7f43830dd98fd33a5512f0a39ab4c5a1903dbbec`  
		Last Modified: Tue, 13 Jul 2021 21:51:00 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
