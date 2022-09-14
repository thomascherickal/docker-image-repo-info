## `kong:latest`

```console
$ docker pull kong@sha256:fac529e0bca71571548f0dc65f240e8f94b780c115ca5deab654fe0687dacc5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:latest` - linux; amd64

```console
$ docker pull kong@sha256:8a54bbf5026200150c46a182e0d56d74ba7572d6cfe98e863fb20cdafce1d95e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51522357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5bce760c29ce855d5935d777f2ec45b3a9ca895a09334825360cebd26a222e6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 14 Sep 2022 00:07:19 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 14 Sep 2022 00:07:19 GMT
ARG ASSET=ce
# Wed, 14 Sep 2022 00:07:19 GMT
ENV ASSET=ce
# Wed, 14 Sep 2022 00:07:19 GMT
ARG EE_PORTS
# Wed, 14 Sep 2022 00:07:19 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 14 Sep 2022 00:07:19 GMT
ARG KONG_VERSION=3.0.0
# Wed, 14 Sep 2022 00:07:19 GMT
ENV KONG_VERSION=3.0.0
# Wed, 14 Sep 2022 00:07:20 GMT
ARG KONG_AMD64_SHA=b8e21beb32f803fae0959694ce7b6cec796a4159757e61b9cc0d30bed9682d10
# Wed, 14 Sep 2022 00:07:20 GMT
ARG KONG_ARM64_SHA=4c5407c5ef2f0f29468e15ea4dc6a3f27011dbde3ce18170e4a4fd7e2bb2c03b
# Wed, 14 Sep 2022 00:07:28 GMT
# ARGS: KONG_AMD64_SHA=b8e21beb32f803fae0959694ce7b6cec796a4159757e61b9cc0d30bed9682d10 KONG_ARM64_SHA=4c5407c5ef2f0f29468e15ea4dc6a3f27011dbde3ce18170e4a4fd7e2bb2c03b
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Wed, 14 Sep 2022 00:07:28 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 14 Sep 2022 00:07:28 GMT
USER kong
# Wed, 14 Sep 2022 00:07:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Sep 2022 00:07:29 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 14 Sep 2022 00:07:29 GMT
STOPSIGNAL SIGQUIT
# Wed, 14 Sep 2022 00:07:29 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 14 Sep 2022 00:07:29 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df4f8c583856d7a692eae94f47792d4cc4a214e2b9d36d1b6dd5eaded569804f`  
		Last Modified: Wed, 14 Sep 2022 00:09:25 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd3d1d803c378e5eb206c29367530e2f8a92578534afdf16cd4ff0da3e687f5`  
		Last Modified: Wed, 14 Sep 2022 00:09:33 GMT  
		Size: 48.7 MB (48715295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7a99de7f80d542680872b47fc5405bf068af5fa56916f994a15149ce05e441`  
		Last Modified: Wed, 14 Sep 2022 00:09:25 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:latest` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:2e4a51fba3b574ee35f990aef3bfd1120ad2e2704f3bc618697382a9f13eaa5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.5 MB (48542736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef17c5908a084b9879dac56870037eccf0c01f792d09fde4b1509019edcc6834`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:42:36 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 09 Aug 2022 20:42:37 GMT
ARG ASSET=ce
# Tue, 09 Aug 2022 20:42:38 GMT
ENV ASSET=ce
# Tue, 09 Aug 2022 20:42:39 GMT
ARG EE_PORTS
# Tue, 09 Aug 2022 20:42:41 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 09 Aug 2022 20:42:41 GMT
ARG KONG_VERSION=2.8.1
# Tue, 09 Aug 2022 20:42:42 GMT
ENV KONG_VERSION=2.8.1
# Tue, 09 Aug 2022 20:42:43 GMT
ARG KONG_AMD64_SHA=ccda33bf02803b6b8dd46b22990f92265fe61d900ba94e3e0fa26db0433098c0
# Tue, 09 Aug 2022 20:42:44 GMT
ARG KONG_ARM64_SHA=d21690332a89adf9900f7266e083f41f565eb009f2771ef112f3564878eeff53
# Tue, 09 Aug 2022 20:42:53 GMT
# ARGS: KONG_AMD64_SHA=ccda33bf02803b6b8dd46b22990f92265fe61d900ba94e3e0fa26db0433098c0 KONG_ARM64_SHA=d21690332a89adf9900f7266e083f41f565eb009f2771ef112f3564878eeff53
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Tue, 09 Aug 2022 20:42:54 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 09 Aug 2022 20:42:54 GMT
USER kong
# Tue, 09 Aug 2022 20:42:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:42:56 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 09 Aug 2022 20:42:57 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Aug 2022 20:42:58 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 09 Aug 2022 20:42:59 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70974eef12350195e179ac6f7e3f7ece7a292a31c6a4f5e19006b7df7f02df11`  
		Last Modified: Tue, 09 Aug 2022 20:45:58 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8314b864c236792b78293d546cc56ce12740413e395c5cc628457e893f46c905`  
		Last Modified: Tue, 09 Aug 2022 20:46:06 GMT  
		Size: 45.8 MB (45834060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:422419cd811d0936d352e9b792f92bcf50bdc9af873da1eb9c5f91f48f0570ca`  
		Last Modified: Tue, 09 Aug 2022 20:45:58 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
