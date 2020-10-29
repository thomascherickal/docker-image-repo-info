## `kong:alpine`

```console
$ docker pull kong@sha256:8b141da0a8fa843e1b745720089448db0236eb9d88999f009c8bf1f20d52c033
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:alpine` - linux; amd64

```console
$ docker pull kong@sha256:19ee9b741cc0dec5276136131af486702441181180ce4a630dd55dfce6d17ded
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53143102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1550bbb81daedb5b1e1b32ff7cfebc601eb3f5e2fe0fc816b4da13e77fdfdbc9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Tue, 05 May 2020 00:19:56 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 05 May 2020 00:19:56 GMT
ARG ASSET=ce
# Tue, 05 May 2020 00:19:56 GMT
ENV ASSET=ce
# Mon, 13 Jul 2020 17:19:53 GMT
ARG EE_PORTS
# Mon, 13 Jul 2020 17:19:53 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 29 Oct 2020 18:21:14 GMT
ARG KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:21:14 GMT
ENV KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:21:21 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='6adb706eab6cc535f2703bd8993a5d5259159cf8a630c3d3974973dbe6bbf5a6' ;; 		aarch64) arch='arm64'; KONG_SHA256='a93b1c015d86b5d8b4038f3fd73332bfef97fa1c768545f353af03f54cf97fb8' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Thu, 29 Oct 2020 18:21:22 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 29 Oct 2020 18:21:22 GMT
USER kong
# Thu, 29 Oct 2020 18:21:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Oct 2020 18:21:22 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 29 Oct 2020 18:21:22 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Oct 2020 18:21:22 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e0de2dc0e7e86d092bbee85a6c1ef2769273bd1a78d87bc9a745745fe2d3b9`  
		Last Modified: Mon, 13 Jul 2020 17:21:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c25d97cc4039bd282d150d09da1590e01019a05e641c6f61495324fb35a0a6ea`  
		Last Modified: Thu, 29 Oct 2020 18:23:45 GMT  
		Size: 50.3 MB (50328923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98513f5777887ba304362c52a37f9686f876ad0af12cdb8b6e49d17de0a348a8`  
		Last Modified: Thu, 29 Oct 2020 18:23:36 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:0a0cad9b3779321b3c9a35ad077bf1e5645e291d7329e161183152692c5cb637
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52673538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d354929336a5e32ec6d0b868be426c01545ee0f07715f5d4f6574114013cb13`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Tue, 22 Sep 2020 19:05:32 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 22 Sep 2020 19:05:34 GMT
ARG ASSET=ce
# Tue, 22 Sep 2020 19:05:35 GMT
ENV ASSET=ce
# Tue, 22 Sep 2020 19:05:36 GMT
ARG EE_PORTS
# Tue, 22 Sep 2020 19:05:36 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 29 Oct 2020 18:42:33 GMT
ARG KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:42:33 GMT
ENV KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:42:46 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='6adb706eab6cc535f2703bd8993a5d5259159cf8a630c3d3974973dbe6bbf5a6' ;; 		aarch64) arch='arm64'; KONG_SHA256='a93b1c015d86b5d8b4038f3fd73332bfef97fa1c768545f353af03f54cf97fb8' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Thu, 29 Oct 2020 18:42:48 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 29 Oct 2020 18:42:48 GMT
USER kong
# Thu, 29 Oct 2020 18:42:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Oct 2020 18:42:49 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 29 Oct 2020 18:42:50 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Oct 2020 18:42:50 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f1f361b75deeea5140a58989e54db49d72c8f2794625392d9b60e5f6adea53`  
		Last Modified: Tue, 22 Sep 2020 19:08:54 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0562e5901c7c1412846095fddf0527b3aec71f8d310829523e905e5dec70db4a`  
		Last Modified: Thu, 29 Oct 2020 18:51:28 GMT  
		Size: 49.9 MB (49948248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b00d686849acde734efe3f6499685d14b6e6deea6307aa2194f32f58e7a026`  
		Last Modified: Thu, 29 Oct 2020 18:51:13 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
