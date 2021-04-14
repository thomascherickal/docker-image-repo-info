## `kong:latest`

```console
$ docker pull kong@sha256:6945a47f45cd607e7608c2eac542cfc393fa042ffb1522ef211623d227f91cb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:latest` - linux; amd64

```console
$ docker pull kong@sha256:0372a0a05c5a4066cbfa1836766d6726edd55a4e3e1ee3a962c85c517a137339
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51157442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04e950e221f43ed7989260b2a61accb568d9d3cdd7df13c9a42f4edd83329851`
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
# Wed, 14 Apr 2021 19:23:23 GMT
ARG KONG_VERSION=2.4.0
# Wed, 14 Apr 2021 19:23:23 GMT
ENV KONG_VERSION=2.4.0
# Wed, 14 Apr 2021 19:23:23 GMT
ARG KONG_AMD64_SHA=a69246ac847e63fa878a4c91fcd097d3ce11db00fd2ce647f1afdf60b5271fa8
# Wed, 14 Apr 2021 19:23:24 GMT
ENV KONG_AMD64_SHA=a69246ac847e63fa878a4c91fcd097d3ce11db00fd2ce647f1afdf60b5271fa8
# Wed, 14 Apr 2021 19:23:24 GMT
ARG KONG_ARM64_SHA=59150130fa4571a406ba72e71dc9ac64ccf48bdf3941ee1965e6a3626d0fbc18
# Wed, 14 Apr 2021 19:23:24 GMT
ENV KONG_ARM64_SHA=59150130fa4571a406ba72e71dc9ac64ccf48bdf3941ee1965e6a3626d0fbc18
# Wed, 14 Apr 2021 19:23:38 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;; 		aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Wed, 14 Apr 2021 19:23:39 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 14 Apr 2021 19:23:39 GMT
USER kong
# Wed, 14 Apr 2021 19:23:40 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Apr 2021 19:23:40 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 14 Apr 2021 19:23:40 GMT
STOPSIGNAL SIGQUIT
# Wed, 14 Apr 2021 19:23:41 GMT
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
	-	`sha256:cc91e546b96c68aa68775d1e466977f5340f41446ca8722944a19c714306e48b`  
		Last Modified: Wed, 14 Apr 2021 19:29:15 GMT  
		Size: 48.3 MB (48340332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b835101a2100b139d649deb78fbeeec2a8efd295f076021c79fc15e733fbeaaa`  
		Last Modified: Wed, 14 Apr 2021 19:29:06 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:latest` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:8baef1499c836a5ead7cc313d644345288268814b399cb3c090aa0dde7157e42
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50474917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4216112af0ba6ba50e70f28a3ee5ff501cde49429852d0f555344afbb48a365b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 31 Mar 2021 17:22:02 GMT
ADD file:174ba1b913c5cf549fcdfc259e8e3aa8f49cea660865fd54b8aacb430602a783 in / 
# Wed, 31 Mar 2021 17:22:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:39:21 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 01 Apr 2021 13:39:22 GMT
ARG ASSET=ce
# Thu, 01 Apr 2021 13:39:23 GMT
ENV ASSET=ce
# Thu, 01 Apr 2021 13:39:23 GMT
ARG EE_PORTS
# Thu, 01 Apr 2021 13:39:24 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 01 Apr 2021 13:39:25 GMT
ARG KONG_VERSION=2.3.3
# Thu, 01 Apr 2021 13:39:26 GMT
ENV KONG_VERSION=2.3.3
# Thu, 01 Apr 2021 13:39:26 GMT
ARG KONG_AMD64_SHA=82a4eac75d45a1f2ce65ae185467e20533428b3d368e5e091fe4ddf427296e0b
# Thu, 01 Apr 2021 13:39:27 GMT
ENV KONG_AMD64_SHA=82a4eac75d45a1f2ce65ae185467e20533428b3d368e5e091fe4ddf427296e0b
# Thu, 01 Apr 2021 13:39:28 GMT
ARG KONG_ARM64_SHA=b2b8a0fe0cdb81d244e08c23a3143e4ae08b7c771a2cc35e24ffabfc54f4ba60
# Thu, 01 Apr 2021 13:39:29 GMT
ENV KONG_ARM64_SHA=b2b8a0fe0cdb81d244e08c23a3143e4ae08b7c771a2cc35e24ffabfc54f4ba60
# Thu, 01 Apr 2021 13:39:40 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;; 		aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Thu, 01 Apr 2021 13:39:42 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 01 Apr 2021 13:39:43 GMT
USER kong
# Thu, 01 Apr 2021 13:39:44 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 01 Apr 2021 13:39:44 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 01 Apr 2021 13:39:45 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Apr 2021 13:39:46 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a3cf95b55367cb73f51318ee9c854def347373482336709ca1882a5d4c20b7c7`  
		Last Modified: Wed, 31 Mar 2021 17:23:00 GMT  
		Size: 2.7 MB (2725871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d662de68ef79de2102c7d691f0bb8460e07f4a80512f0e5c52df2db9e20f8e8`  
		Last Modified: Thu, 01 Apr 2021 13:41:32 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f800ac016936c6e32cd04afc15191ce1233c8fe5e976a57747e4e8d5b8db8b5a`  
		Last Modified: Thu, 01 Apr 2021 13:41:46 GMT  
		Size: 47.7 MB (47748181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07581418082abae0fc5003a3f36bfb7bc4466b474e066da8cd565723676e2596`  
		Last Modified: Thu, 01 Apr 2021 13:41:33 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
