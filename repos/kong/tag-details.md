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
-	[`kong:2.5.1`](#kong251)
-	[`kong:2.5.1-alpine`](#kong251-alpine)
-	[`kong:2.5.1-centos`](#kong251-centos)
-	[`kong:2.5.1-ubuntu`](#kong251-ubuntu)
-	[`kong:alpine`](#kongalpine)
-	[`kong:centos`](#kongcentos)
-	[`kong:latest`](#konglatest)
-	[`kong:ubuntu`](#kongubuntu)

## `kong:2.4`

```console
$ docker pull kong@sha256:e296a94b044f02cedc1f4ead5f3643fd346abfa3af65b8e1e22829568fee6c19
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.4` - linux; amd64

```console
$ docker pull kong@sha256:045e697e3ef3ea4cd43f936de41ddd088a2f3890bf7006cb4826e73a764a6f9d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51161550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7cf1525dfb883b0ba6a6a34740124f69b9c300aea711c255acb20f35dab1668`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:31 GMT
ADD file:9d14b11183983923090d9e6d15cc51ee210466296e913bfefbfd580b3de59c95 in / 
# Tue, 31 Aug 2021 23:18:31 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 03:09:02 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 01 Sep 2021 03:09:02 GMT
ARG ASSET=ce
# Wed, 01 Sep 2021 03:09:03 GMT
ENV ASSET=ce
# Wed, 01 Sep 2021 03:09:03 GMT
ARG EE_PORTS
# Wed, 01 Sep 2021 03:09:03 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 01 Sep 2021 03:09:03 GMT
ARG KONG_VERSION=2.4.1
# Wed, 01 Sep 2021 03:09:03 GMT
ENV KONG_VERSION=2.4.1
# Wed, 01 Sep 2021 03:09:04 GMT
ARG KONG_AMD64_SHA=582cbcf23eb4dcdf9873105ac7d8428a4022ec61bcc68642ad9dd8a5c03e2a57
# Wed, 01 Sep 2021 03:09:04 GMT
ENV KONG_AMD64_SHA=582cbcf23eb4dcdf9873105ac7d8428a4022ec61bcc68642ad9dd8a5c03e2a57
# Wed, 01 Sep 2021 03:09:04 GMT
ARG KONG_ARM64_SHA=5ec35d1b19dd4e6592ad2c6586e68bfd1549c6a22840ce7d5654677b94e5028a
# Wed, 01 Sep 2021 03:09:04 GMT
ENV KONG_ARM64_SHA=5ec35d1b19dd4e6592ad2c6586e68bfd1549c6a22840ce7d5654677b94e5028a
# Wed, 01 Sep 2021 03:09:11 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;; 		aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Wed, 01 Sep 2021 03:09:12 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 01 Sep 2021 03:09:12 GMT
USER kong
# Wed, 01 Sep 2021 03:09:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Sep 2021 03:09:13 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Sep 2021 03:09:13 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Sep 2021 03:09:13 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:6a428f9f83b0a29f1fdd2ccccca19a9bab805a925b8eddf432a5a3d3da04afbc`  
		Last Modified: Tue, 31 Aug 2021 23:19:15 GMT  
		Size: 2.8 MB (2817307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b2fdf8677e885d36654660d3b6787d4570360ec039166e107595faaed80df3`  
		Last Modified: Wed, 01 Sep 2021 03:10:12 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50035c712e4bbc88d24c5cc6dd271fb8f509a325c23c14b9be15ff03ce198c7f`  
		Last Modified: Wed, 01 Sep 2021 03:10:21 GMT  
		Size: 48.3 MB (48343378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ec93853d683ef00af85c5c921ff9de5e67f5acffa56856887a112829b9eb025`  
		Last Modified: Wed, 01 Sep 2021 03:10:12 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.4` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:34216898be0687201185259c0eb9279548d473c129a9a76d1caf62002c02bda7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50695357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa2b21df398c3d75f121ce472776a3b244d69586bbbd4ce5dfa03eb16387552d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:59 GMT
ADD file:da6c0ac7cb9f819998546d88fb489b746004eb2ad6da64a39210696ef0e66e54 in / 
# Wed, 01 Sep 2021 02:50:59 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 13:09:51 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 01 Sep 2021 13:09:51 GMT
ARG ASSET=ce
# Wed, 01 Sep 2021 13:09:51 GMT
ENV ASSET=ce
# Wed, 01 Sep 2021 13:09:51 GMT
ARG EE_PORTS
# Wed, 01 Sep 2021 13:09:52 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 01 Sep 2021 13:09:52 GMT
ARG KONG_VERSION=2.4.1
# Wed, 01 Sep 2021 13:09:52 GMT
ENV KONG_VERSION=2.4.1
# Wed, 01 Sep 2021 13:09:52 GMT
ARG KONG_AMD64_SHA=582cbcf23eb4dcdf9873105ac7d8428a4022ec61bcc68642ad9dd8a5c03e2a57
# Wed, 01 Sep 2021 13:09:52 GMT
ENV KONG_AMD64_SHA=582cbcf23eb4dcdf9873105ac7d8428a4022ec61bcc68642ad9dd8a5c03e2a57
# Wed, 01 Sep 2021 13:09:52 GMT
ARG KONG_ARM64_SHA=5ec35d1b19dd4e6592ad2c6586e68bfd1549c6a22840ce7d5654677b94e5028a
# Wed, 01 Sep 2021 13:09:53 GMT
ENV KONG_ARM64_SHA=5ec35d1b19dd4e6592ad2c6586e68bfd1549c6a22840ce7d5654677b94e5028a
# Wed, 01 Sep 2021 13:09:59 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;; 		aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Wed, 01 Sep 2021 13:10:00 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 01 Sep 2021 13:10:00 GMT
USER kong
# Wed, 01 Sep 2021 13:10:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Sep 2021 13:10:00 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Sep 2021 13:10:00 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Sep 2021 13:10:01 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:07d756952c5cd45726cf9e8a292a3e05ca67eee5da176df7d632be8c5bb0ad04`  
		Last Modified: Wed, 01 Sep 2021 02:52:00 GMT  
		Size: 2.7 MB (2728407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7cfd3733cda112df2193eabae749ae36791f899a817f21dcd11feadf9762ec7`  
		Last Modified: Wed, 01 Sep 2021 13:11:21 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56e1e3837467fad535d7b6ba33a44e3ef67db1b53cb8b02a70ae697d29f89e5`  
		Last Modified: Wed, 01 Sep 2021 13:11:30 GMT  
		Size: 48.0 MB (47966084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7985ba6b51e181c2f4c78127f33685ddb1a9fa7309e1dfb3192dd25447005c2a`  
		Last Modified: Wed, 01 Sep 2021 13:11:21 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.4-alpine`

```console
$ docker pull kong@sha256:e296a94b044f02cedc1f4ead5f3643fd346abfa3af65b8e1e22829568fee6c19
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.4-alpine` - linux; amd64

```console
$ docker pull kong@sha256:045e697e3ef3ea4cd43f936de41ddd088a2f3890bf7006cb4826e73a764a6f9d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51161550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7cf1525dfb883b0ba6a6a34740124f69b9c300aea711c255acb20f35dab1668`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:31 GMT
ADD file:9d14b11183983923090d9e6d15cc51ee210466296e913bfefbfd580b3de59c95 in / 
# Tue, 31 Aug 2021 23:18:31 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 03:09:02 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 01 Sep 2021 03:09:02 GMT
ARG ASSET=ce
# Wed, 01 Sep 2021 03:09:03 GMT
ENV ASSET=ce
# Wed, 01 Sep 2021 03:09:03 GMT
ARG EE_PORTS
# Wed, 01 Sep 2021 03:09:03 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 01 Sep 2021 03:09:03 GMT
ARG KONG_VERSION=2.4.1
# Wed, 01 Sep 2021 03:09:03 GMT
ENV KONG_VERSION=2.4.1
# Wed, 01 Sep 2021 03:09:04 GMT
ARG KONG_AMD64_SHA=582cbcf23eb4dcdf9873105ac7d8428a4022ec61bcc68642ad9dd8a5c03e2a57
# Wed, 01 Sep 2021 03:09:04 GMT
ENV KONG_AMD64_SHA=582cbcf23eb4dcdf9873105ac7d8428a4022ec61bcc68642ad9dd8a5c03e2a57
# Wed, 01 Sep 2021 03:09:04 GMT
ARG KONG_ARM64_SHA=5ec35d1b19dd4e6592ad2c6586e68bfd1549c6a22840ce7d5654677b94e5028a
# Wed, 01 Sep 2021 03:09:04 GMT
ENV KONG_ARM64_SHA=5ec35d1b19dd4e6592ad2c6586e68bfd1549c6a22840ce7d5654677b94e5028a
# Wed, 01 Sep 2021 03:09:11 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;; 		aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Wed, 01 Sep 2021 03:09:12 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 01 Sep 2021 03:09:12 GMT
USER kong
# Wed, 01 Sep 2021 03:09:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Sep 2021 03:09:13 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Sep 2021 03:09:13 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Sep 2021 03:09:13 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:6a428f9f83b0a29f1fdd2ccccca19a9bab805a925b8eddf432a5a3d3da04afbc`  
		Last Modified: Tue, 31 Aug 2021 23:19:15 GMT  
		Size: 2.8 MB (2817307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b2fdf8677e885d36654660d3b6787d4570360ec039166e107595faaed80df3`  
		Last Modified: Wed, 01 Sep 2021 03:10:12 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50035c712e4bbc88d24c5cc6dd271fb8f509a325c23c14b9be15ff03ce198c7f`  
		Last Modified: Wed, 01 Sep 2021 03:10:21 GMT  
		Size: 48.3 MB (48343378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ec93853d683ef00af85c5c921ff9de5e67f5acffa56856887a112829b9eb025`  
		Last Modified: Wed, 01 Sep 2021 03:10:12 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.4-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:34216898be0687201185259c0eb9279548d473c129a9a76d1caf62002c02bda7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50695357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa2b21df398c3d75f121ce472776a3b244d69586bbbd4ce5dfa03eb16387552d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:59 GMT
ADD file:da6c0ac7cb9f819998546d88fb489b746004eb2ad6da64a39210696ef0e66e54 in / 
# Wed, 01 Sep 2021 02:50:59 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 13:09:51 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 01 Sep 2021 13:09:51 GMT
ARG ASSET=ce
# Wed, 01 Sep 2021 13:09:51 GMT
ENV ASSET=ce
# Wed, 01 Sep 2021 13:09:51 GMT
ARG EE_PORTS
# Wed, 01 Sep 2021 13:09:52 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 01 Sep 2021 13:09:52 GMT
ARG KONG_VERSION=2.4.1
# Wed, 01 Sep 2021 13:09:52 GMT
ENV KONG_VERSION=2.4.1
# Wed, 01 Sep 2021 13:09:52 GMT
ARG KONG_AMD64_SHA=582cbcf23eb4dcdf9873105ac7d8428a4022ec61bcc68642ad9dd8a5c03e2a57
# Wed, 01 Sep 2021 13:09:52 GMT
ENV KONG_AMD64_SHA=582cbcf23eb4dcdf9873105ac7d8428a4022ec61bcc68642ad9dd8a5c03e2a57
# Wed, 01 Sep 2021 13:09:52 GMT
ARG KONG_ARM64_SHA=5ec35d1b19dd4e6592ad2c6586e68bfd1549c6a22840ce7d5654677b94e5028a
# Wed, 01 Sep 2021 13:09:53 GMT
ENV KONG_ARM64_SHA=5ec35d1b19dd4e6592ad2c6586e68bfd1549c6a22840ce7d5654677b94e5028a
# Wed, 01 Sep 2021 13:09:59 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;; 		aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Wed, 01 Sep 2021 13:10:00 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 01 Sep 2021 13:10:00 GMT
USER kong
# Wed, 01 Sep 2021 13:10:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Sep 2021 13:10:00 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Sep 2021 13:10:00 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Sep 2021 13:10:01 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:07d756952c5cd45726cf9e8a292a3e05ca67eee5da176df7d632be8c5bb0ad04`  
		Last Modified: Wed, 01 Sep 2021 02:52:00 GMT  
		Size: 2.7 MB (2728407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7cfd3733cda112df2193eabae749ae36791f899a817f21dcd11feadf9762ec7`  
		Last Modified: Wed, 01 Sep 2021 13:11:21 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56e1e3837467fad535d7b6ba33a44e3ef67db1b53cb8b02a70ae697d29f89e5`  
		Last Modified: Wed, 01 Sep 2021 13:11:30 GMT  
		Size: 48.0 MB (47966084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7985ba6b51e181c2f4c78127f33685ddb1a9fa7309e1dfb3192dd25447005c2a`  
		Last Modified: Wed, 01 Sep 2021 13:11:21 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.4-centos`

```console
$ docker pull kong@sha256:49dddad34751502c9aee35caeae45b24fc0ac296357711b9de1f8fceb4fd7895
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:2.4-centos` - linux; amd64

```console
$ docker pull kong@sha256:feb4461a2a085b2042c075e2d1744d3ff6b207e775b291cc3675b80461db8029
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.6 MB (127646569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82cc1bb25437f8a5dbed0102a4231f576e55f5d303012939db68a9bc52785fca`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:23 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Wed, 15 Sep 2021 18:20:23 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 18:20:23 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 19:51:18 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 15 Sep 2021 19:51:18 GMT
ARG ASSET=ce
# Wed, 15 Sep 2021 19:51:18 GMT
ENV ASSET=ce
# Wed, 15 Sep 2021 19:51:19 GMT
ARG EE_PORTS
# Wed, 15 Sep 2021 19:51:19 GMT
COPY file:ff02c070e4c89f043b176279a7e41464b5fab8cb98cfcd6332fad2d2741fc41d in /tmp/kong.rpm 
# Wed, 15 Sep 2021 19:52:07 GMT
ARG KONG_VERSION=2.4.1
# Wed, 15 Sep 2021 19:52:07 GMT
ENV KONG_VERSION=2.4.1
# Wed, 15 Sep 2021 19:52:07 GMT
ARG KONG_SHA256=b8083a6c268f69865e66a8d504fcdacab49ba36a4194ccfc9737d65e6863c30a
# Wed, 15 Sep 2021 19:52:42 GMT
# ARGS: KONG_SHA256=b8083a6c268f69865e66a8d504fcdacab49ba36a4194ccfc9737d65e6863c30a
RUN set -ex;   if [ "$ASSET" = "ce" ] ; then   curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-centos-7/Packages/k/kong-$KONG_VERSION.el7.amd64.rpm -o /tmp/kong.rpm     && echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -;   fi;   yum install -y -q unzip shadow-utils git   && yum clean all -q   && rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki   && yum install -y /tmp/kong.rpm   && yum clean all   && rm /tmp/kong.rpm   && chown kong:0 /usr/local/bin/kong   && chown -R kong:0 /usr/local/kong &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Wed, 15 Sep 2021 19:52:43 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 15 Sep 2021 19:52:43 GMT
USER kong
# Wed, 15 Sep 2021 19:52:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 15 Sep 2021 19:52:44 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 15 Sep 2021 19:52:44 GMT
STOPSIGNAL SIGQUIT
# Wed, 15 Sep 2021 19:52:44 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf5a22c33293d0d5fc35b813a8f71d89abcd8398213f41285640177d7580dac`  
		Last Modified: Wed, 15 Sep 2021 19:53:15 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7bbc591d91f6a82fd63289e983b1baa055494e373060828ea98a396e7860bdc`  
		Last Modified: Wed, 15 Sep 2021 19:53:48 GMT  
		Size: 51.5 MB (51548551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fcc045327ddc9eda05feb281dcbf8434f27be814258455a2b415a6f13544d03`  
		Last Modified: Wed, 15 Sep 2021 19:53:39 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.4-ubuntu`

```console
$ docker pull kong@sha256:cceeace7bd46399b90a013088b614aa253c540620c6c4a32d8f07ee836c4c22d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.4-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:1b238a9ef17d623392714e7a5a498a16874b87ae19d56c6f85cb0f937289a079
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134752818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ee52b964888ac2d31cac4c35679b93f316cde405b3d62620dfdfd6d466ac6c8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:27 GMT
ADD file:11b425d4c08e81a3e0cb2e0345d27cd5fc844dd83f1096af4cc05f635824ff5d in / 
# Tue, 31 Aug 2021 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:21:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:21:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:21:30 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 03:40:30 GMT
ARG ASSET=ce
# Tue, 31 Aug 2021 03:40:31 GMT
ENV ASSET=ce
# Tue, 31 Aug 2021 03:40:31 GMT
ARG EE_PORTS
# Tue, 31 Aug 2021 03:40:31 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Tue, 31 Aug 2021 03:41:06 GMT
ARG KONG_VERSION=2.4.1
# Tue, 31 Aug 2021 03:41:06 GMT
ENV KONG_VERSION=2.4.1
# Tue, 31 Aug 2021 03:41:28 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL 		https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-xenial/pool/all/k/kong/kong_${KONG_VERSION}_$(dpkg --print-architecture).deb -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Tue, 31 Aug 2021 03:41:29 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Tue, 31 Aug 2021 03:41:29 GMT
USER kong
# Tue, 31 Aug 2021 03:41:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:41:30 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 31 Aug 2021 03:41:30 GMT
STOPSIGNAL SIGQUIT
# Tue, 31 Aug 2021 03:41:30 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:58690f9b18fca6469a14da4e212c96849469f9b1be6661d2342a4bf01774aa50`  
		Last Modified: Thu, 05 Aug 2021 00:25:05 GMT  
		Size: 46.5 MB (46497548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51569e7c50720acf6860327847fe342a1afbe148d24c529fb81df105e3eed01`  
		Last Modified: Tue, 31 Aug 2021 01:23:09 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ef40b9ecabc2679fe2419957220c0272a965c5cf7e0269fa1aeeb8c56f2e1`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb15d46c38dcd1ea0b1990006c3366ecd10c79d374f341687eb2cb23a2c8672e`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f9bf842551a4304b6e9bb37db25ba1932a186b178e50b94d7ba879d235b8ef`  
		Last Modified: Tue, 31 Aug 2021 03:42:03 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2b40add1d10ca76f9333f9a91f0c033556d4058acbcbb216d98d522fd9d6d1`  
		Last Modified: Tue, 31 Aug 2021 03:42:37 GMT  
		Size: 63.2 MB (63171073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a244e218996bdeaf548d3d178afa2a7f14e419f5a6359218e3983fab9f08b71`  
		Last Modified: Tue, 31 Aug 2021 03:42:26 GMT  
		Size: 688.0 B  
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
$ docker pull kong@sha256:e296a94b044f02cedc1f4ead5f3643fd346abfa3af65b8e1e22829568fee6c19
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.4.1` - linux; amd64

```console
$ docker pull kong@sha256:045e697e3ef3ea4cd43f936de41ddd088a2f3890bf7006cb4826e73a764a6f9d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51161550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7cf1525dfb883b0ba6a6a34740124f69b9c300aea711c255acb20f35dab1668`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:31 GMT
ADD file:9d14b11183983923090d9e6d15cc51ee210466296e913bfefbfd580b3de59c95 in / 
# Tue, 31 Aug 2021 23:18:31 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 03:09:02 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 01 Sep 2021 03:09:02 GMT
ARG ASSET=ce
# Wed, 01 Sep 2021 03:09:03 GMT
ENV ASSET=ce
# Wed, 01 Sep 2021 03:09:03 GMT
ARG EE_PORTS
# Wed, 01 Sep 2021 03:09:03 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 01 Sep 2021 03:09:03 GMT
ARG KONG_VERSION=2.4.1
# Wed, 01 Sep 2021 03:09:03 GMT
ENV KONG_VERSION=2.4.1
# Wed, 01 Sep 2021 03:09:04 GMT
ARG KONG_AMD64_SHA=582cbcf23eb4dcdf9873105ac7d8428a4022ec61bcc68642ad9dd8a5c03e2a57
# Wed, 01 Sep 2021 03:09:04 GMT
ENV KONG_AMD64_SHA=582cbcf23eb4dcdf9873105ac7d8428a4022ec61bcc68642ad9dd8a5c03e2a57
# Wed, 01 Sep 2021 03:09:04 GMT
ARG KONG_ARM64_SHA=5ec35d1b19dd4e6592ad2c6586e68bfd1549c6a22840ce7d5654677b94e5028a
# Wed, 01 Sep 2021 03:09:04 GMT
ENV KONG_ARM64_SHA=5ec35d1b19dd4e6592ad2c6586e68bfd1549c6a22840ce7d5654677b94e5028a
# Wed, 01 Sep 2021 03:09:11 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;; 		aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Wed, 01 Sep 2021 03:09:12 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 01 Sep 2021 03:09:12 GMT
USER kong
# Wed, 01 Sep 2021 03:09:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Sep 2021 03:09:13 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Sep 2021 03:09:13 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Sep 2021 03:09:13 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:6a428f9f83b0a29f1fdd2ccccca19a9bab805a925b8eddf432a5a3d3da04afbc`  
		Last Modified: Tue, 31 Aug 2021 23:19:15 GMT  
		Size: 2.8 MB (2817307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b2fdf8677e885d36654660d3b6787d4570360ec039166e107595faaed80df3`  
		Last Modified: Wed, 01 Sep 2021 03:10:12 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50035c712e4bbc88d24c5cc6dd271fb8f509a325c23c14b9be15ff03ce198c7f`  
		Last Modified: Wed, 01 Sep 2021 03:10:21 GMT  
		Size: 48.3 MB (48343378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ec93853d683ef00af85c5c921ff9de5e67f5acffa56856887a112829b9eb025`  
		Last Modified: Wed, 01 Sep 2021 03:10:12 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.4.1` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:34216898be0687201185259c0eb9279548d473c129a9a76d1caf62002c02bda7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50695357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa2b21df398c3d75f121ce472776a3b244d69586bbbd4ce5dfa03eb16387552d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:59 GMT
ADD file:da6c0ac7cb9f819998546d88fb489b746004eb2ad6da64a39210696ef0e66e54 in / 
# Wed, 01 Sep 2021 02:50:59 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 13:09:51 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 01 Sep 2021 13:09:51 GMT
ARG ASSET=ce
# Wed, 01 Sep 2021 13:09:51 GMT
ENV ASSET=ce
# Wed, 01 Sep 2021 13:09:51 GMT
ARG EE_PORTS
# Wed, 01 Sep 2021 13:09:52 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 01 Sep 2021 13:09:52 GMT
ARG KONG_VERSION=2.4.1
# Wed, 01 Sep 2021 13:09:52 GMT
ENV KONG_VERSION=2.4.1
# Wed, 01 Sep 2021 13:09:52 GMT
ARG KONG_AMD64_SHA=582cbcf23eb4dcdf9873105ac7d8428a4022ec61bcc68642ad9dd8a5c03e2a57
# Wed, 01 Sep 2021 13:09:52 GMT
ENV KONG_AMD64_SHA=582cbcf23eb4dcdf9873105ac7d8428a4022ec61bcc68642ad9dd8a5c03e2a57
# Wed, 01 Sep 2021 13:09:52 GMT
ARG KONG_ARM64_SHA=5ec35d1b19dd4e6592ad2c6586e68bfd1549c6a22840ce7d5654677b94e5028a
# Wed, 01 Sep 2021 13:09:53 GMT
ENV KONG_ARM64_SHA=5ec35d1b19dd4e6592ad2c6586e68bfd1549c6a22840ce7d5654677b94e5028a
# Wed, 01 Sep 2021 13:09:59 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;; 		aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Wed, 01 Sep 2021 13:10:00 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 01 Sep 2021 13:10:00 GMT
USER kong
# Wed, 01 Sep 2021 13:10:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Sep 2021 13:10:00 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Sep 2021 13:10:00 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Sep 2021 13:10:01 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:07d756952c5cd45726cf9e8a292a3e05ca67eee5da176df7d632be8c5bb0ad04`  
		Last Modified: Wed, 01 Sep 2021 02:52:00 GMT  
		Size: 2.7 MB (2728407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7cfd3733cda112df2193eabae749ae36791f899a817f21dcd11feadf9762ec7`  
		Last Modified: Wed, 01 Sep 2021 13:11:21 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56e1e3837467fad535d7b6ba33a44e3ef67db1b53cb8b02a70ae697d29f89e5`  
		Last Modified: Wed, 01 Sep 2021 13:11:30 GMT  
		Size: 48.0 MB (47966084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7985ba6b51e181c2f4c78127f33685ddb1a9fa7309e1dfb3192dd25447005c2a`  
		Last Modified: Wed, 01 Sep 2021 13:11:21 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.4.1-alpine`

```console
$ docker pull kong@sha256:e296a94b044f02cedc1f4ead5f3643fd346abfa3af65b8e1e22829568fee6c19
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.4.1-alpine` - linux; amd64

```console
$ docker pull kong@sha256:045e697e3ef3ea4cd43f936de41ddd088a2f3890bf7006cb4826e73a764a6f9d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51161550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7cf1525dfb883b0ba6a6a34740124f69b9c300aea711c255acb20f35dab1668`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:31 GMT
ADD file:9d14b11183983923090d9e6d15cc51ee210466296e913bfefbfd580b3de59c95 in / 
# Tue, 31 Aug 2021 23:18:31 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 03:09:02 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 01 Sep 2021 03:09:02 GMT
ARG ASSET=ce
# Wed, 01 Sep 2021 03:09:03 GMT
ENV ASSET=ce
# Wed, 01 Sep 2021 03:09:03 GMT
ARG EE_PORTS
# Wed, 01 Sep 2021 03:09:03 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 01 Sep 2021 03:09:03 GMT
ARG KONG_VERSION=2.4.1
# Wed, 01 Sep 2021 03:09:03 GMT
ENV KONG_VERSION=2.4.1
# Wed, 01 Sep 2021 03:09:04 GMT
ARG KONG_AMD64_SHA=582cbcf23eb4dcdf9873105ac7d8428a4022ec61bcc68642ad9dd8a5c03e2a57
# Wed, 01 Sep 2021 03:09:04 GMT
ENV KONG_AMD64_SHA=582cbcf23eb4dcdf9873105ac7d8428a4022ec61bcc68642ad9dd8a5c03e2a57
# Wed, 01 Sep 2021 03:09:04 GMT
ARG KONG_ARM64_SHA=5ec35d1b19dd4e6592ad2c6586e68bfd1549c6a22840ce7d5654677b94e5028a
# Wed, 01 Sep 2021 03:09:04 GMT
ENV KONG_ARM64_SHA=5ec35d1b19dd4e6592ad2c6586e68bfd1549c6a22840ce7d5654677b94e5028a
# Wed, 01 Sep 2021 03:09:11 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;; 		aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Wed, 01 Sep 2021 03:09:12 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 01 Sep 2021 03:09:12 GMT
USER kong
# Wed, 01 Sep 2021 03:09:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Sep 2021 03:09:13 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Sep 2021 03:09:13 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Sep 2021 03:09:13 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:6a428f9f83b0a29f1fdd2ccccca19a9bab805a925b8eddf432a5a3d3da04afbc`  
		Last Modified: Tue, 31 Aug 2021 23:19:15 GMT  
		Size: 2.8 MB (2817307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b2fdf8677e885d36654660d3b6787d4570360ec039166e107595faaed80df3`  
		Last Modified: Wed, 01 Sep 2021 03:10:12 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50035c712e4bbc88d24c5cc6dd271fb8f509a325c23c14b9be15ff03ce198c7f`  
		Last Modified: Wed, 01 Sep 2021 03:10:21 GMT  
		Size: 48.3 MB (48343378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ec93853d683ef00af85c5c921ff9de5e67f5acffa56856887a112829b9eb025`  
		Last Modified: Wed, 01 Sep 2021 03:10:12 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.4.1-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:34216898be0687201185259c0eb9279548d473c129a9a76d1caf62002c02bda7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50695357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa2b21df398c3d75f121ce472776a3b244d69586bbbd4ce5dfa03eb16387552d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:59 GMT
ADD file:da6c0ac7cb9f819998546d88fb489b746004eb2ad6da64a39210696ef0e66e54 in / 
# Wed, 01 Sep 2021 02:50:59 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 13:09:51 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 01 Sep 2021 13:09:51 GMT
ARG ASSET=ce
# Wed, 01 Sep 2021 13:09:51 GMT
ENV ASSET=ce
# Wed, 01 Sep 2021 13:09:51 GMT
ARG EE_PORTS
# Wed, 01 Sep 2021 13:09:52 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 01 Sep 2021 13:09:52 GMT
ARG KONG_VERSION=2.4.1
# Wed, 01 Sep 2021 13:09:52 GMT
ENV KONG_VERSION=2.4.1
# Wed, 01 Sep 2021 13:09:52 GMT
ARG KONG_AMD64_SHA=582cbcf23eb4dcdf9873105ac7d8428a4022ec61bcc68642ad9dd8a5c03e2a57
# Wed, 01 Sep 2021 13:09:52 GMT
ENV KONG_AMD64_SHA=582cbcf23eb4dcdf9873105ac7d8428a4022ec61bcc68642ad9dd8a5c03e2a57
# Wed, 01 Sep 2021 13:09:52 GMT
ARG KONG_ARM64_SHA=5ec35d1b19dd4e6592ad2c6586e68bfd1549c6a22840ce7d5654677b94e5028a
# Wed, 01 Sep 2021 13:09:53 GMT
ENV KONG_ARM64_SHA=5ec35d1b19dd4e6592ad2c6586e68bfd1549c6a22840ce7d5654677b94e5028a
# Wed, 01 Sep 2021 13:09:59 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;; 		aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Wed, 01 Sep 2021 13:10:00 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 01 Sep 2021 13:10:00 GMT
USER kong
# Wed, 01 Sep 2021 13:10:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Sep 2021 13:10:00 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Sep 2021 13:10:00 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Sep 2021 13:10:01 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:07d756952c5cd45726cf9e8a292a3e05ca67eee5da176df7d632be8c5bb0ad04`  
		Last Modified: Wed, 01 Sep 2021 02:52:00 GMT  
		Size: 2.7 MB (2728407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7cfd3733cda112df2193eabae749ae36791f899a817f21dcd11feadf9762ec7`  
		Last Modified: Wed, 01 Sep 2021 13:11:21 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56e1e3837467fad535d7b6ba33a44e3ef67db1b53cb8b02a70ae697d29f89e5`  
		Last Modified: Wed, 01 Sep 2021 13:11:30 GMT  
		Size: 48.0 MB (47966084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7985ba6b51e181c2f4c78127f33685ddb1a9fa7309e1dfb3192dd25447005c2a`  
		Last Modified: Wed, 01 Sep 2021 13:11:21 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.4.1-centos`

```console
$ docker pull kong@sha256:49dddad34751502c9aee35caeae45b24fc0ac296357711b9de1f8fceb4fd7895
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:2.4.1-centos` - linux; amd64

```console
$ docker pull kong@sha256:feb4461a2a085b2042c075e2d1744d3ff6b207e775b291cc3675b80461db8029
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.6 MB (127646569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82cc1bb25437f8a5dbed0102a4231f576e55f5d303012939db68a9bc52785fca`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:23 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Wed, 15 Sep 2021 18:20:23 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 18:20:23 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 19:51:18 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 15 Sep 2021 19:51:18 GMT
ARG ASSET=ce
# Wed, 15 Sep 2021 19:51:18 GMT
ENV ASSET=ce
# Wed, 15 Sep 2021 19:51:19 GMT
ARG EE_PORTS
# Wed, 15 Sep 2021 19:51:19 GMT
COPY file:ff02c070e4c89f043b176279a7e41464b5fab8cb98cfcd6332fad2d2741fc41d in /tmp/kong.rpm 
# Wed, 15 Sep 2021 19:52:07 GMT
ARG KONG_VERSION=2.4.1
# Wed, 15 Sep 2021 19:52:07 GMT
ENV KONG_VERSION=2.4.1
# Wed, 15 Sep 2021 19:52:07 GMT
ARG KONG_SHA256=b8083a6c268f69865e66a8d504fcdacab49ba36a4194ccfc9737d65e6863c30a
# Wed, 15 Sep 2021 19:52:42 GMT
# ARGS: KONG_SHA256=b8083a6c268f69865e66a8d504fcdacab49ba36a4194ccfc9737d65e6863c30a
RUN set -ex;   if [ "$ASSET" = "ce" ] ; then   curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-centos-7/Packages/k/kong-$KONG_VERSION.el7.amd64.rpm -o /tmp/kong.rpm     && echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -;   fi;   yum install -y -q unzip shadow-utils git   && yum clean all -q   && rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki   && yum install -y /tmp/kong.rpm   && yum clean all   && rm /tmp/kong.rpm   && chown kong:0 /usr/local/bin/kong   && chown -R kong:0 /usr/local/kong &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Wed, 15 Sep 2021 19:52:43 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 15 Sep 2021 19:52:43 GMT
USER kong
# Wed, 15 Sep 2021 19:52:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 15 Sep 2021 19:52:44 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 15 Sep 2021 19:52:44 GMT
STOPSIGNAL SIGQUIT
# Wed, 15 Sep 2021 19:52:44 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf5a22c33293d0d5fc35b813a8f71d89abcd8398213f41285640177d7580dac`  
		Last Modified: Wed, 15 Sep 2021 19:53:15 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7bbc591d91f6a82fd63289e983b1baa055494e373060828ea98a396e7860bdc`  
		Last Modified: Wed, 15 Sep 2021 19:53:48 GMT  
		Size: 51.5 MB (51548551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fcc045327ddc9eda05feb281dcbf8434f27be814258455a2b415a6f13544d03`  
		Last Modified: Wed, 15 Sep 2021 19:53:39 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.4.1-ubuntu`

```console
$ docker pull kong@sha256:cceeace7bd46399b90a013088b614aa253c540620c6c4a32d8f07ee836c4c22d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.4.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:1b238a9ef17d623392714e7a5a498a16874b87ae19d56c6f85cb0f937289a079
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134752818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ee52b964888ac2d31cac4c35679b93f316cde405b3d62620dfdfd6d466ac6c8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:27 GMT
ADD file:11b425d4c08e81a3e0cb2e0345d27cd5fc844dd83f1096af4cc05f635824ff5d in / 
# Tue, 31 Aug 2021 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:21:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:21:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:21:30 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 03:40:30 GMT
ARG ASSET=ce
# Tue, 31 Aug 2021 03:40:31 GMT
ENV ASSET=ce
# Tue, 31 Aug 2021 03:40:31 GMT
ARG EE_PORTS
# Tue, 31 Aug 2021 03:40:31 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Tue, 31 Aug 2021 03:41:06 GMT
ARG KONG_VERSION=2.4.1
# Tue, 31 Aug 2021 03:41:06 GMT
ENV KONG_VERSION=2.4.1
# Tue, 31 Aug 2021 03:41:28 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL 		https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-xenial/pool/all/k/kong/kong_${KONG_VERSION}_$(dpkg --print-architecture).deb -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Tue, 31 Aug 2021 03:41:29 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Tue, 31 Aug 2021 03:41:29 GMT
USER kong
# Tue, 31 Aug 2021 03:41:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:41:30 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 31 Aug 2021 03:41:30 GMT
STOPSIGNAL SIGQUIT
# Tue, 31 Aug 2021 03:41:30 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:58690f9b18fca6469a14da4e212c96849469f9b1be6661d2342a4bf01774aa50`  
		Last Modified: Thu, 05 Aug 2021 00:25:05 GMT  
		Size: 46.5 MB (46497548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51569e7c50720acf6860327847fe342a1afbe148d24c529fb81df105e3eed01`  
		Last Modified: Tue, 31 Aug 2021 01:23:09 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ef40b9ecabc2679fe2419957220c0272a965c5cf7e0269fa1aeeb8c56f2e1`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb15d46c38dcd1ea0b1990006c3366ecd10c79d374f341687eb2cb23a2c8672e`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f9bf842551a4304b6e9bb37db25ba1932a186b178e50b94d7ba879d235b8ef`  
		Last Modified: Tue, 31 Aug 2021 03:42:03 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2b40add1d10ca76f9333f9a91f0c033556d4058acbcbb216d98d522fd9d6d1`  
		Last Modified: Tue, 31 Aug 2021 03:42:37 GMT  
		Size: 63.2 MB (63171073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a244e218996bdeaf548d3d178afa2a7f14e419f5a6359218e3983fab9f08b71`  
		Last Modified: Tue, 31 Aug 2021 03:42:26 GMT  
		Size: 688.0 B  
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
$ docker pull kong@sha256:a90175f1a3290007122ad5b397e4f2db67a4ca5870dc755230b6c397a08ec021
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.5` - linux; amd64

```console
$ docker pull kong@sha256:a667daead4dbbef0fbb6da8e860fe1c16cb10ae3889f3ba02e1ed600e2f1c7cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49542131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fac313c49d6bee3db1dbbf099ed50c7921640d125e75d742267ac0cf113b3160`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 03:08:41 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 01 Sep 2021 03:08:41 GMT
ARG ASSET=ce
# Wed, 01 Sep 2021 03:08:41 GMT
ENV ASSET=ce
# Wed, 01 Sep 2021 03:08:41 GMT
ARG EE_PORTS
# Wed, 01 Sep 2021 03:08:42 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 01 Sep 2021 03:08:42 GMT
ARG KONG_VERSION=2.5.0
# Wed, 01 Sep 2021 03:08:42 GMT
ENV KONG_VERSION=2.5.0
# Wed, 01 Sep 2021 03:08:42 GMT
ARG KONG_AMD64_SHA=ebe0cf3a3e71d202774ede5083c98e2ae39fae0459d11140f53401a66527e1b7
# Wed, 01 Sep 2021 03:08:42 GMT
ENV KONG_AMD64_SHA=ebe0cf3a3e71d202774ede5083c98e2ae39fae0459d11140f53401a66527e1b7
# Wed, 01 Sep 2021 03:08:43 GMT
ARG KONG_ARM64_SHA=131964ce443f2d08dc98191fcc442867f2dee2f741ccee9cc519bb99c765f3cf
# Wed, 01 Sep 2021 03:08:43 GMT
ENV KONG_ARM64_SHA=131964ce443f2d08dc98191fcc442867f2dee2f741ccee9cc519bb99c765f3cf
# Wed, 01 Sep 2021 03:08:51 GMT
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Wed, 01 Sep 2021 03:08:51 GMT
COPY file:a9828df20ead648b4c991bfb67a40d0065e248e50a2ae98fad0104e78f32d234 in /docker-entrypoint.sh 
# Wed, 01 Sep 2021 03:08:51 GMT
USER kong
# Wed, 01 Sep 2021 03:08:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Sep 2021 03:08:52 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Sep 2021 03:08:52 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Sep 2021 03:08:52 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 01 Sep 2021 03:08:53 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a932a260c1e4852852f30dfd019cb0eaeca493933da107b49b478f97a8114a`  
		Last Modified: Wed, 01 Sep 2021 03:09:44 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af18b1a4934e2c5e54790d320d17240ba331b21f0df9b2d4892f9b8a5a57c5aa`  
		Last Modified: Wed, 01 Sep 2021 03:09:53 GMT  
		Size: 46.7 MB (46727187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97ef9b6bde488c17df64ac1a14770099af9f764e728f626da456fcd3cff2afc`  
		Last Modified: Wed, 01 Sep 2021 03:09:45 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.5` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:8231711dae245456227c2b5eb1fe12f907f9fd9c0205a09627fc9430d2ab9765
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48937742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:325cf6127197d92d3cb30f7f71cc004eb1f74955a5c067d775da6f299074785d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 13:09:28 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 01 Sep 2021 13:09:28 GMT
ARG ASSET=ce
# Wed, 01 Sep 2021 13:09:29 GMT
ENV ASSET=ce
# Wed, 01 Sep 2021 13:09:29 GMT
ARG EE_PORTS
# Wed, 01 Sep 2021 13:09:29 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 01 Sep 2021 13:09:29 GMT
ARG KONG_VERSION=2.5.0
# Wed, 01 Sep 2021 13:09:29 GMT
ENV KONG_VERSION=2.5.0
# Wed, 01 Sep 2021 13:09:30 GMT
ARG KONG_AMD64_SHA=ebe0cf3a3e71d202774ede5083c98e2ae39fae0459d11140f53401a66527e1b7
# Wed, 01 Sep 2021 13:09:30 GMT
ENV KONG_AMD64_SHA=ebe0cf3a3e71d202774ede5083c98e2ae39fae0459d11140f53401a66527e1b7
# Wed, 01 Sep 2021 13:09:30 GMT
ARG KONG_ARM64_SHA=131964ce443f2d08dc98191fcc442867f2dee2f741ccee9cc519bb99c765f3cf
# Wed, 01 Sep 2021 13:09:30 GMT
ENV KONG_ARM64_SHA=131964ce443f2d08dc98191fcc442867f2dee2f741ccee9cc519bb99c765f3cf
# Wed, 01 Sep 2021 13:09:37 GMT
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Wed, 01 Sep 2021 13:09:38 GMT
COPY file:a9828df20ead648b4c991bfb67a40d0065e248e50a2ae98fad0104e78f32d234 in /docker-entrypoint.sh 
# Wed, 01 Sep 2021 13:09:38 GMT
USER kong
# Wed, 01 Sep 2021 13:09:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Sep 2021 13:09:38 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Sep 2021 13:09:39 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Sep 2021 13:09:39 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 01 Sep 2021 13:09:39 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834874c5e974b53eb28baf25287cb6506a1ba5b4e01ff118aaa9566fcecb5c39`  
		Last Modified: Wed, 01 Sep 2021 13:10:44 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f1885bae9c378b0ed22b0f54882317aa2b369c3437d48dde9383bde00fe9cc`  
		Last Modified: Wed, 01 Sep 2021 13:10:55 GMT  
		Size: 46.2 MB (46223868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:749c3863a80bc68fa2ffebe71f27d856b6914678264e891679ad6554ec59c613`  
		Last Modified: Wed, 01 Sep 2021 13:10:44 GMT  
		Size: 735.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.5-centos`

```console
$ docker pull kong@sha256:c4b986e95eafd8535d19af8bc437b0decfff9159b1b4caf22f28e7ddaf7b85bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:2.5-centos` - linux; amd64

```console
$ docker pull kong@sha256:1928d45ffbe00b0b49e96580d8d887d952bbe7daf620c0495fdbc31458e69092
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127677142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b76b7d589e8a9b405e2f23047dd76b5d3bb84828e90bcffabadab57c9389f43`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:23 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Wed, 15 Sep 2021 18:20:23 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 18:20:23 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 19:51:18 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 15 Sep 2021 19:51:18 GMT
ARG ASSET=ce
# Wed, 15 Sep 2021 19:51:18 GMT
ENV ASSET=ce
# Wed, 15 Sep 2021 19:51:19 GMT
ARG EE_PORTS
# Wed, 15 Sep 2021 19:51:19 GMT
COPY file:ff02c070e4c89f043b176279a7e41464b5fab8cb98cfcd6332fad2d2741fc41d in /tmp/kong.rpm 
# Wed, 15 Sep 2021 19:51:19 GMT
ARG KONG_VERSION=2.5.0
# Wed, 15 Sep 2021 19:51:19 GMT
ENV KONG_VERSION=2.5.0
# Wed, 15 Sep 2021 19:51:19 GMT
ARG KONG_SHA256=87b789aed871991b92d264b02ceca3c66246c825c28dd71e73faac7293e43fa2
# Wed, 15 Sep 2021 19:51:56 GMT
# ARGS: KONG_SHA256=87b789aed871991b92d264b02ceca3c66246c825c28dd71e73faac7293e43fa2
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then       curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-centos-7/Packages/k/kong-$KONG_VERSION.el7.amd64.rpm -o /tmp/kong.rpm       && echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -;     fi;     yum install -y -q unzip shadow-utils git     && yum clean all -q     && rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki     && yum install -y /tmp/kong.rpm     && yum clean all     && rm /tmp/kong.rpm     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 15 Sep 2021 19:51:57 GMT
COPY file:a9828df20ead648b4c991bfb67a40d0065e248e50a2ae98fad0104e78f32d234 in /docker-entrypoint.sh 
# Wed, 15 Sep 2021 19:51:57 GMT
USER kong
# Wed, 15 Sep 2021 19:51:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 15 Sep 2021 19:51:57 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 15 Sep 2021 19:51:58 GMT
STOPSIGNAL SIGQUIT
# Wed, 15 Sep 2021 19:51:58 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 15 Sep 2021 19:51:58 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf5a22c33293d0d5fc35b813a8f71d89abcd8398213f41285640177d7580dac`  
		Last Modified: Wed, 15 Sep 2021 19:53:15 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c55ecca617c73dd7b430dd8357e9dbe938057c0042fe6d5e726a30f379d2d9`  
		Last Modified: Wed, 15 Sep 2021 19:53:24 GMT  
		Size: 51.6 MB (51579122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43a421991328f1f39cd093e8a8ece0cbb79e399ef450e1b494442d191805149`  
		Last Modified: Wed, 15 Sep 2021 19:53:15 GMT  
		Size: 735.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.5-ubuntu`

```console
$ docker pull kong@sha256:97d6b3979328cfe737070bc726fa5463d679c5fdb101408b75ffe7e0e4bb9dcd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.5-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:6b75c3d10c7b969d3a7d8ce5b979625867b5d82b7ed6f8a13cf95ee9c1a6b56d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134774884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70deec2d9da44076bbcd96b7e6a682fa5775fad5352038369858f0c531604a4d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:27 GMT
ADD file:11b425d4c08e81a3e0cb2e0345d27cd5fc844dd83f1096af4cc05f635824ff5d in / 
# Tue, 31 Aug 2021 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:21:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:21:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:21:30 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 03:40:30 GMT
ARG ASSET=ce
# Tue, 31 Aug 2021 03:40:31 GMT
ENV ASSET=ce
# Tue, 31 Aug 2021 03:40:31 GMT
ARG EE_PORTS
# Tue, 31 Aug 2021 03:40:31 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Tue, 31 Aug 2021 03:40:31 GMT
ARG KONG_VERSION=2.5.0
# Tue, 31 Aug 2021 03:40:32 GMT
ENV KONG_VERSION=2.5.0
# Tue, 31 Aug 2021 03:40:55 GMT
RUN set -ex     && apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)/pool/all/k/kong/kong_${KONG_VERSION}_$(dpkg --print-architecture).deb -o /tmp/kong.deb       && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 31 Aug 2021 03:40:56 GMT
COPY file:ae813ec19d3fef1de3793f6717c2aed3a9daa94e583e9e55448084541de3c5ff in /docker-entrypoint.sh 
# Tue, 31 Aug 2021 03:40:56 GMT
USER kong
# Tue, 31 Aug 2021 03:40:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:40:56 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 31 Aug 2021 03:40:57 GMT
STOPSIGNAL SIGQUIT
# Tue, 31 Aug 2021 03:40:57 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 31 Aug 2021 03:40:57 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:58690f9b18fca6469a14da4e212c96849469f9b1be6661d2342a4bf01774aa50`  
		Last Modified: Thu, 05 Aug 2021 00:25:05 GMT  
		Size: 46.5 MB (46497548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51569e7c50720acf6860327847fe342a1afbe148d24c529fb81df105e3eed01`  
		Last Modified: Tue, 31 Aug 2021 01:23:09 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ef40b9ecabc2679fe2419957220c0272a965c5cf7e0269fa1aeeb8c56f2e1`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb15d46c38dcd1ea0b1990006c3366ecd10c79d374f341687eb2cb23a2c8672e`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f9bf842551a4304b6e9bb37db25ba1932a186b178e50b94d7ba879d235b8ef`  
		Last Modified: Tue, 31 Aug 2021 03:42:03 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bab5733c17a786298cfad2b3c4d83f85f95c702cab217eeb2f0ca75e1fa2c1`  
		Last Modified: Tue, 31 Aug 2021 03:42:11 GMT  
		Size: 63.2 MB (63193136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63029535d411ee20e1efe45d2593e98f28e1cee823edba60780cfa3c6381cd4`  
		Last Modified: Tue, 31 Aug 2021 03:42:01 GMT  
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

## `kong:2.5.1`

**does not exist** (yet?)

## `kong:2.5.1-alpine`

**does not exist** (yet?)

## `kong:2.5.1-centos`

**does not exist** (yet?)

## `kong:2.5.1-ubuntu`

**does not exist** (yet?)

## `kong:alpine`

```console
$ docker pull kong@sha256:a90175f1a3290007122ad5b397e4f2db67a4ca5870dc755230b6c397a08ec021
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:alpine` - linux; amd64

```console
$ docker pull kong@sha256:a667daead4dbbef0fbb6da8e860fe1c16cb10ae3889f3ba02e1ed600e2f1c7cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49542131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fac313c49d6bee3db1dbbf099ed50c7921640d125e75d742267ac0cf113b3160`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 03:08:41 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 01 Sep 2021 03:08:41 GMT
ARG ASSET=ce
# Wed, 01 Sep 2021 03:08:41 GMT
ENV ASSET=ce
# Wed, 01 Sep 2021 03:08:41 GMT
ARG EE_PORTS
# Wed, 01 Sep 2021 03:08:42 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 01 Sep 2021 03:08:42 GMT
ARG KONG_VERSION=2.5.0
# Wed, 01 Sep 2021 03:08:42 GMT
ENV KONG_VERSION=2.5.0
# Wed, 01 Sep 2021 03:08:42 GMT
ARG KONG_AMD64_SHA=ebe0cf3a3e71d202774ede5083c98e2ae39fae0459d11140f53401a66527e1b7
# Wed, 01 Sep 2021 03:08:42 GMT
ENV KONG_AMD64_SHA=ebe0cf3a3e71d202774ede5083c98e2ae39fae0459d11140f53401a66527e1b7
# Wed, 01 Sep 2021 03:08:43 GMT
ARG KONG_ARM64_SHA=131964ce443f2d08dc98191fcc442867f2dee2f741ccee9cc519bb99c765f3cf
# Wed, 01 Sep 2021 03:08:43 GMT
ENV KONG_ARM64_SHA=131964ce443f2d08dc98191fcc442867f2dee2f741ccee9cc519bb99c765f3cf
# Wed, 01 Sep 2021 03:08:51 GMT
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Wed, 01 Sep 2021 03:08:51 GMT
COPY file:a9828df20ead648b4c991bfb67a40d0065e248e50a2ae98fad0104e78f32d234 in /docker-entrypoint.sh 
# Wed, 01 Sep 2021 03:08:51 GMT
USER kong
# Wed, 01 Sep 2021 03:08:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Sep 2021 03:08:52 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Sep 2021 03:08:52 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Sep 2021 03:08:52 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 01 Sep 2021 03:08:53 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a932a260c1e4852852f30dfd019cb0eaeca493933da107b49b478f97a8114a`  
		Last Modified: Wed, 01 Sep 2021 03:09:44 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af18b1a4934e2c5e54790d320d17240ba331b21f0df9b2d4892f9b8a5a57c5aa`  
		Last Modified: Wed, 01 Sep 2021 03:09:53 GMT  
		Size: 46.7 MB (46727187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97ef9b6bde488c17df64ac1a14770099af9f764e728f626da456fcd3cff2afc`  
		Last Modified: Wed, 01 Sep 2021 03:09:45 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:8231711dae245456227c2b5eb1fe12f907f9fd9c0205a09627fc9430d2ab9765
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48937742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:325cf6127197d92d3cb30f7f71cc004eb1f74955a5c067d775da6f299074785d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 13:09:28 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 01 Sep 2021 13:09:28 GMT
ARG ASSET=ce
# Wed, 01 Sep 2021 13:09:29 GMT
ENV ASSET=ce
# Wed, 01 Sep 2021 13:09:29 GMT
ARG EE_PORTS
# Wed, 01 Sep 2021 13:09:29 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 01 Sep 2021 13:09:29 GMT
ARG KONG_VERSION=2.5.0
# Wed, 01 Sep 2021 13:09:29 GMT
ENV KONG_VERSION=2.5.0
# Wed, 01 Sep 2021 13:09:30 GMT
ARG KONG_AMD64_SHA=ebe0cf3a3e71d202774ede5083c98e2ae39fae0459d11140f53401a66527e1b7
# Wed, 01 Sep 2021 13:09:30 GMT
ENV KONG_AMD64_SHA=ebe0cf3a3e71d202774ede5083c98e2ae39fae0459d11140f53401a66527e1b7
# Wed, 01 Sep 2021 13:09:30 GMT
ARG KONG_ARM64_SHA=131964ce443f2d08dc98191fcc442867f2dee2f741ccee9cc519bb99c765f3cf
# Wed, 01 Sep 2021 13:09:30 GMT
ENV KONG_ARM64_SHA=131964ce443f2d08dc98191fcc442867f2dee2f741ccee9cc519bb99c765f3cf
# Wed, 01 Sep 2021 13:09:37 GMT
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Wed, 01 Sep 2021 13:09:38 GMT
COPY file:a9828df20ead648b4c991bfb67a40d0065e248e50a2ae98fad0104e78f32d234 in /docker-entrypoint.sh 
# Wed, 01 Sep 2021 13:09:38 GMT
USER kong
# Wed, 01 Sep 2021 13:09:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Sep 2021 13:09:38 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Sep 2021 13:09:39 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Sep 2021 13:09:39 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 01 Sep 2021 13:09:39 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834874c5e974b53eb28baf25287cb6506a1ba5b4e01ff118aaa9566fcecb5c39`  
		Last Modified: Wed, 01 Sep 2021 13:10:44 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f1885bae9c378b0ed22b0f54882317aa2b369c3437d48dde9383bde00fe9cc`  
		Last Modified: Wed, 01 Sep 2021 13:10:55 GMT  
		Size: 46.2 MB (46223868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:749c3863a80bc68fa2ffebe71f27d856b6914678264e891679ad6554ec59c613`  
		Last Modified: Wed, 01 Sep 2021 13:10:44 GMT  
		Size: 735.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:centos`

```console
$ docker pull kong@sha256:c4b986e95eafd8535d19af8bc437b0decfff9159b1b4caf22f28e7ddaf7b85bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:centos` - linux; amd64

```console
$ docker pull kong@sha256:1928d45ffbe00b0b49e96580d8d887d952bbe7daf620c0495fdbc31458e69092
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127677142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b76b7d589e8a9b405e2f23047dd76b5d3bb84828e90bcffabadab57c9389f43`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:23 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Wed, 15 Sep 2021 18:20:23 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 18:20:23 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 19:51:18 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 15 Sep 2021 19:51:18 GMT
ARG ASSET=ce
# Wed, 15 Sep 2021 19:51:18 GMT
ENV ASSET=ce
# Wed, 15 Sep 2021 19:51:19 GMT
ARG EE_PORTS
# Wed, 15 Sep 2021 19:51:19 GMT
COPY file:ff02c070e4c89f043b176279a7e41464b5fab8cb98cfcd6332fad2d2741fc41d in /tmp/kong.rpm 
# Wed, 15 Sep 2021 19:51:19 GMT
ARG KONG_VERSION=2.5.0
# Wed, 15 Sep 2021 19:51:19 GMT
ENV KONG_VERSION=2.5.0
# Wed, 15 Sep 2021 19:51:19 GMT
ARG KONG_SHA256=87b789aed871991b92d264b02ceca3c66246c825c28dd71e73faac7293e43fa2
# Wed, 15 Sep 2021 19:51:56 GMT
# ARGS: KONG_SHA256=87b789aed871991b92d264b02ceca3c66246c825c28dd71e73faac7293e43fa2
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then       curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-centos-7/Packages/k/kong-$KONG_VERSION.el7.amd64.rpm -o /tmp/kong.rpm       && echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -;     fi;     yum install -y -q unzip shadow-utils git     && yum clean all -q     && rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki     && yum install -y /tmp/kong.rpm     && yum clean all     && rm /tmp/kong.rpm     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 15 Sep 2021 19:51:57 GMT
COPY file:a9828df20ead648b4c991bfb67a40d0065e248e50a2ae98fad0104e78f32d234 in /docker-entrypoint.sh 
# Wed, 15 Sep 2021 19:51:57 GMT
USER kong
# Wed, 15 Sep 2021 19:51:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 15 Sep 2021 19:51:57 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 15 Sep 2021 19:51:58 GMT
STOPSIGNAL SIGQUIT
# Wed, 15 Sep 2021 19:51:58 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 15 Sep 2021 19:51:58 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf5a22c33293d0d5fc35b813a8f71d89abcd8398213f41285640177d7580dac`  
		Last Modified: Wed, 15 Sep 2021 19:53:15 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c55ecca617c73dd7b430dd8357e9dbe938057c0042fe6d5e726a30f379d2d9`  
		Last Modified: Wed, 15 Sep 2021 19:53:24 GMT  
		Size: 51.6 MB (51579122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43a421991328f1f39cd093e8a8ece0cbb79e399ef450e1b494442d191805149`  
		Last Modified: Wed, 15 Sep 2021 19:53:15 GMT  
		Size: 735.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:latest`

```console
$ docker pull kong@sha256:a90175f1a3290007122ad5b397e4f2db67a4ca5870dc755230b6c397a08ec021
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:latest` - linux; amd64

```console
$ docker pull kong@sha256:a667daead4dbbef0fbb6da8e860fe1c16cb10ae3889f3ba02e1ed600e2f1c7cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49542131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fac313c49d6bee3db1dbbf099ed50c7921640d125e75d742267ac0cf113b3160`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 03:08:41 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 01 Sep 2021 03:08:41 GMT
ARG ASSET=ce
# Wed, 01 Sep 2021 03:08:41 GMT
ENV ASSET=ce
# Wed, 01 Sep 2021 03:08:41 GMT
ARG EE_PORTS
# Wed, 01 Sep 2021 03:08:42 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 01 Sep 2021 03:08:42 GMT
ARG KONG_VERSION=2.5.0
# Wed, 01 Sep 2021 03:08:42 GMT
ENV KONG_VERSION=2.5.0
# Wed, 01 Sep 2021 03:08:42 GMT
ARG KONG_AMD64_SHA=ebe0cf3a3e71d202774ede5083c98e2ae39fae0459d11140f53401a66527e1b7
# Wed, 01 Sep 2021 03:08:42 GMT
ENV KONG_AMD64_SHA=ebe0cf3a3e71d202774ede5083c98e2ae39fae0459d11140f53401a66527e1b7
# Wed, 01 Sep 2021 03:08:43 GMT
ARG KONG_ARM64_SHA=131964ce443f2d08dc98191fcc442867f2dee2f741ccee9cc519bb99c765f3cf
# Wed, 01 Sep 2021 03:08:43 GMT
ENV KONG_ARM64_SHA=131964ce443f2d08dc98191fcc442867f2dee2f741ccee9cc519bb99c765f3cf
# Wed, 01 Sep 2021 03:08:51 GMT
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Wed, 01 Sep 2021 03:08:51 GMT
COPY file:a9828df20ead648b4c991bfb67a40d0065e248e50a2ae98fad0104e78f32d234 in /docker-entrypoint.sh 
# Wed, 01 Sep 2021 03:08:51 GMT
USER kong
# Wed, 01 Sep 2021 03:08:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Sep 2021 03:08:52 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Sep 2021 03:08:52 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Sep 2021 03:08:52 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 01 Sep 2021 03:08:53 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a932a260c1e4852852f30dfd019cb0eaeca493933da107b49b478f97a8114a`  
		Last Modified: Wed, 01 Sep 2021 03:09:44 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af18b1a4934e2c5e54790d320d17240ba331b21f0df9b2d4892f9b8a5a57c5aa`  
		Last Modified: Wed, 01 Sep 2021 03:09:53 GMT  
		Size: 46.7 MB (46727187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97ef9b6bde488c17df64ac1a14770099af9f764e728f626da456fcd3cff2afc`  
		Last Modified: Wed, 01 Sep 2021 03:09:45 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:latest` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:8231711dae245456227c2b5eb1fe12f907f9fd9c0205a09627fc9430d2ab9765
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48937742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:325cf6127197d92d3cb30f7f71cc004eb1f74955a5c067d775da6f299074785d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 13:09:28 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 01 Sep 2021 13:09:28 GMT
ARG ASSET=ce
# Wed, 01 Sep 2021 13:09:29 GMT
ENV ASSET=ce
# Wed, 01 Sep 2021 13:09:29 GMT
ARG EE_PORTS
# Wed, 01 Sep 2021 13:09:29 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 01 Sep 2021 13:09:29 GMT
ARG KONG_VERSION=2.5.0
# Wed, 01 Sep 2021 13:09:29 GMT
ENV KONG_VERSION=2.5.0
# Wed, 01 Sep 2021 13:09:30 GMT
ARG KONG_AMD64_SHA=ebe0cf3a3e71d202774ede5083c98e2ae39fae0459d11140f53401a66527e1b7
# Wed, 01 Sep 2021 13:09:30 GMT
ENV KONG_AMD64_SHA=ebe0cf3a3e71d202774ede5083c98e2ae39fae0459d11140f53401a66527e1b7
# Wed, 01 Sep 2021 13:09:30 GMT
ARG KONG_ARM64_SHA=131964ce443f2d08dc98191fcc442867f2dee2f741ccee9cc519bb99c765f3cf
# Wed, 01 Sep 2021 13:09:30 GMT
ENV KONG_ARM64_SHA=131964ce443f2d08dc98191fcc442867f2dee2f741ccee9cc519bb99c765f3cf
# Wed, 01 Sep 2021 13:09:37 GMT
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Wed, 01 Sep 2021 13:09:38 GMT
COPY file:a9828df20ead648b4c991bfb67a40d0065e248e50a2ae98fad0104e78f32d234 in /docker-entrypoint.sh 
# Wed, 01 Sep 2021 13:09:38 GMT
USER kong
# Wed, 01 Sep 2021 13:09:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Sep 2021 13:09:38 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Sep 2021 13:09:39 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Sep 2021 13:09:39 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 01 Sep 2021 13:09:39 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834874c5e974b53eb28baf25287cb6506a1ba5b4e01ff118aaa9566fcecb5c39`  
		Last Modified: Wed, 01 Sep 2021 13:10:44 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f1885bae9c378b0ed22b0f54882317aa2b369c3437d48dde9383bde00fe9cc`  
		Last Modified: Wed, 01 Sep 2021 13:10:55 GMT  
		Size: 46.2 MB (46223868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:749c3863a80bc68fa2ffebe71f27d856b6914678264e891679ad6554ec59c613`  
		Last Modified: Wed, 01 Sep 2021 13:10:44 GMT  
		Size: 735.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:ubuntu`

```console
$ docker pull kong@sha256:97d6b3979328cfe737070bc726fa5463d679c5fdb101408b75ffe7e0e4bb9dcd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:6b75c3d10c7b969d3a7d8ce5b979625867b5d82b7ed6f8a13cf95ee9c1a6b56d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134774884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70deec2d9da44076bbcd96b7e6a682fa5775fad5352038369858f0c531604a4d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:27 GMT
ADD file:11b425d4c08e81a3e0cb2e0345d27cd5fc844dd83f1096af4cc05f635824ff5d in / 
# Tue, 31 Aug 2021 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:21:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:21:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:21:30 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 03:40:30 GMT
ARG ASSET=ce
# Tue, 31 Aug 2021 03:40:31 GMT
ENV ASSET=ce
# Tue, 31 Aug 2021 03:40:31 GMT
ARG EE_PORTS
# Tue, 31 Aug 2021 03:40:31 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Tue, 31 Aug 2021 03:40:31 GMT
ARG KONG_VERSION=2.5.0
# Tue, 31 Aug 2021 03:40:32 GMT
ENV KONG_VERSION=2.5.0
# Tue, 31 Aug 2021 03:40:55 GMT
RUN set -ex     && apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)/pool/all/k/kong/kong_${KONG_VERSION}_$(dpkg --print-architecture).deb -o /tmp/kong.deb       && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 31 Aug 2021 03:40:56 GMT
COPY file:ae813ec19d3fef1de3793f6717c2aed3a9daa94e583e9e55448084541de3c5ff in /docker-entrypoint.sh 
# Tue, 31 Aug 2021 03:40:56 GMT
USER kong
# Tue, 31 Aug 2021 03:40:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:40:56 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 31 Aug 2021 03:40:57 GMT
STOPSIGNAL SIGQUIT
# Tue, 31 Aug 2021 03:40:57 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 31 Aug 2021 03:40:57 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:58690f9b18fca6469a14da4e212c96849469f9b1be6661d2342a4bf01774aa50`  
		Last Modified: Thu, 05 Aug 2021 00:25:05 GMT  
		Size: 46.5 MB (46497548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51569e7c50720acf6860327847fe342a1afbe148d24c529fb81df105e3eed01`  
		Last Modified: Tue, 31 Aug 2021 01:23:09 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ef40b9ecabc2679fe2419957220c0272a965c5cf7e0269fa1aeeb8c56f2e1`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb15d46c38dcd1ea0b1990006c3366ecd10c79d374f341687eb2cb23a2c8672e`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f9bf842551a4304b6e9bb37db25ba1932a186b178e50b94d7ba879d235b8ef`  
		Last Modified: Tue, 31 Aug 2021 03:42:03 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bab5733c17a786298cfad2b3c4d83f85f95c702cab217eeb2f0ca75e1fa2c1`  
		Last Modified: Tue, 31 Aug 2021 03:42:11 GMT  
		Size: 63.2 MB (63193136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63029535d411ee20e1efe45d2593e98f28e1cee823edba60780cfa3c6381cd4`  
		Last Modified: Tue, 31 Aug 2021 03:42:01 GMT  
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
