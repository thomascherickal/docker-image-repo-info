## `kong:alpine`

```console
$ docker pull kong@sha256:38c82bcf40f627c1ed3edef3eb0ac9ab3d1fb29fe7eb8df69f5166b324a22153
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:alpine` - linux; amd64

```console
$ docker pull kong@sha256:eaf0443b11346f6b7f4ac6c0979430462e5070b86a31f5cb2b16a0477773c715
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.9 MB (50938328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cd6edfe129b1c02465b0927dcfdc0d52765486279f5916a2c24d06f070dbd95`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 14:57:37 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 14:57:37 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ARG EE_PORTS
# Thu, 17 Dec 2020 14:57:38 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 27 Jan 2021 06:32:07 GMT
ARG KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 06:32:07 GMT
ENV KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 06:32:07 GMT
ARG KONG_AMD64_SHA=8a33a919f75bdb8bb708de23c0701def2aedfcd2679d27b7849040c3edf273f9
# Wed, 27 Jan 2021 06:32:07 GMT
ENV KONG_AMD64_SHA=8a33a919f75bdb8bb708de23c0701def2aedfcd2679d27b7849040c3edf273f9
# Wed, 27 Jan 2021 06:32:08 GMT
ARG KONG_ARM64_SHA=4ae43ecf9b1fcf11930d859efec475e216729b89b76de80a4c38e1fe58e3874f
# Wed, 27 Jan 2021 06:32:08 GMT
ENV KONG_ARM64_SHA=4ae43ecf9b1fcf11930d859efec475e216729b89b76de80a4c38e1fe58e3874f
# Wed, 27 Jan 2021 06:32:15 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;; 		aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Wed, 27 Jan 2021 06:32:16 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 27 Jan 2021 06:32:16 GMT
USER kong
# Wed, 27 Jan 2021 06:32:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 27 Jan 2021 06:32:16 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 27 Jan 2021 06:32:16 GMT
STOPSIGNAL SIGQUIT
# Wed, 27 Jan 2021 06:32:17 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274efec6805c2b13808c7bcb7932f07b136c0be74bf02bdbf77f79e89dc58725`  
		Last Modified: Thu, 17 Dec 2020 14:59:10 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b18e55f2934bb191d816e87b86e196e1c8d35d815f72f93f7e5f51c0f17319e`  
		Last Modified: Wed, 27 Jan 2021 06:35:34 GMT  
		Size: 48.1 MB (48122597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1f7f35984e4dfe3874035c9af0e74955cc49424e7f4a0d50411d336f9228fa`  
		Last Modified: Wed, 27 Jan 2021 06:35:24 GMT  
		Size: 735.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:d87959fb87a61b8f9fba68a010a6e444317df9ca4bbba731d1374c9035077d0e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50462144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065a1ea94079d9d30ef22ca0cbfffc961327ac4759c8ab96e9473a3daeb1b436`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:57:05 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 04:57:06 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 04:57:07 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 04:57:08 GMT
ARG EE_PORTS
# Thu, 17 Dec 2020 04:57:09 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 27 Jan 2021 00:45:22 GMT
ARG KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 00:45:23 GMT
ENV KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 00:45:23 GMT
ARG KONG_AMD64_SHA=8a33a919f75bdb8bb708de23c0701def2aedfcd2679d27b7849040c3edf273f9
# Wed, 27 Jan 2021 00:45:24 GMT
ENV KONG_AMD64_SHA=8a33a919f75bdb8bb708de23c0701def2aedfcd2679d27b7849040c3edf273f9
# Wed, 27 Jan 2021 00:45:24 GMT
ARG KONG_ARM64_SHA=4ae43ecf9b1fcf11930d859efec475e216729b89b76de80a4c38e1fe58e3874f
# Wed, 27 Jan 2021 00:45:25 GMT
ENV KONG_ARM64_SHA=4ae43ecf9b1fcf11930d859efec475e216729b89b76de80a4c38e1fe58e3874f
# Wed, 27 Jan 2021 00:45:38 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;; 		aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Wed, 27 Jan 2021 00:45:40 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 27 Jan 2021 00:45:40 GMT
USER kong
# Wed, 27 Jan 2021 00:45:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 27 Jan 2021 00:45:42 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 27 Jan 2021 00:45:42 GMT
STOPSIGNAL SIGQUIT
# Wed, 27 Jan 2021 00:45:43 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3181cc464c4af55ff9dd73d4603f67578cdc16237deb0e5e467594b40164ab6`  
		Last Modified: Thu, 17 Dec 2020 04:58:48 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:686913a20dd73c0bdaa7517e69803b84807b71b99b4ff55cc9764516b90461f7`  
		Last Modified: Wed, 27 Jan 2021 00:47:56 GMT  
		Size: 47.7 MB (47736063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5429c14c14d5050bce7546a62fa4539c4c325f122c109881ea4dc5f0b628ed6`  
		Last Modified: Wed, 27 Jan 2021 00:47:42 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
