## `kong:ubuntu`

```console
$ docker pull kong@sha256:f6c20b21b6f3ce4fd87fe9576b2bb8bc56bc9f5706c946c93484d74f86154735
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:fdfe2b3097e19964e2293ddc218ac714ab630483be0f835f4f5f52ca1ee9a7cb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.8 MB (97807207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15f8728ef0fb2fb541d6e878e73327c53d88a471dbf8ebfebe86d7c574def672`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 16 Aug 2023 06:01:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:01:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:01:54 GMT
ADD file:aa9b51e9f0067860cebbc9930374452d1384ec3c59badb5e4733130eedc90329 in / 
# Wed, 16 Aug 2023 06:01:54 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 01:16:57 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Sat, 02 Sep 2023 01:16:57 GMT
ARG ASSET=ce
# Sat, 02 Sep 2023 01:16:57 GMT
ENV ASSET=ce
# Sat, 02 Sep 2023 01:16:57 GMT
ARG EE_PORTS
# Sat, 02 Sep 2023 01:16:57 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Sat, 02 Sep 2023 01:16:58 GMT
ARG KONG_VERSION=3.4.0
# Sat, 02 Sep 2023 01:16:58 GMT
ENV KONG_VERSION=3.4.0
# Sat, 02 Sep 2023 01:16:58 GMT
ARG KONG_AMD64_SHA=9a4203174a29895d5dd71092a05b15b26ee9644e068d14d970aed28461d358fa
# Sat, 02 Sep 2023 01:16:58 GMT
ARG KONG_ARM64_SHA=b64e19216ce125039a6a832dc93bf277e05f233a91f1647b351cad3f166edd81
# Sat, 02 Sep 2023 01:17:43 GMT
# ARGS: KONG_AMD64_SHA=9a4203174a29895d5dd71092a05b15b26ee9644e068d14d970aed28461d358fa KONG_ARM64_SHA=b64e19216ce125039a6a832dc93bf277e05f233a91f1647b351cad3f166edd81
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Sat, 02 Sep 2023 01:17:43 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Sat, 02 Sep 2023 01:17:43 GMT
USER kong
# Sat, 02 Sep 2023 01:17:44 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 02 Sep 2023 01:17:44 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 02 Sep 2023 01:17:44 GMT
STOPSIGNAL SIGQUIT
# Sat, 02 Sep 2023 01:17:44 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Sat, 02 Sep 2023 01:17:44 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:44ba2882f8eb14264e5f2f9f6ec55bcf5306527b637279f2cd9d4858762388af`  
		Last Modified: Wed, 16 Aug 2023 10:32:51 GMT  
		Size: 30.4 MB (30438977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0a0ee58de66ad7c8c097e7374c568345c8ed1fd389e41e093bc91e6f9e13bd`  
		Last Modified: Sat, 02 Sep 2023 01:19:16 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410914e02f09941e3599613388b717a81917f1cb2fc9064af03078cb7f40426c`  
		Last Modified: Sat, 02 Sep 2023 01:19:28 GMT  
		Size: 67.4 MB (67366950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5639714d6880ffa83b692aef597837375bd693b96b308a5cc291d6d3dcc6ca54`  
		Last Modified: Sat, 02 Sep 2023 01:19:16 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:a82e486a76a31f6f010c544100eae833df63e71b9e2c50b593f78d74e6583a4b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.2 MB (94160171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10eff2787901e6046a691f0e74e4c79884f39820d194817c35e2d9d830a1826e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 16 Aug 2023 06:19:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:19:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:19:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:19:53 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:19:59 GMT
ADD file:3fcf00866c55150f1ea0a5ef7b8473c39275c1fdbf6aba0acd84cacb83d0c564 in / 
# Wed, 16 Aug 2023 06:19:59 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:15:44 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Sat, 02 Sep 2023 00:15:44 GMT
ARG ASSET=ce
# Sat, 02 Sep 2023 00:15:44 GMT
ENV ASSET=ce
# Sat, 02 Sep 2023 00:15:44 GMT
ARG EE_PORTS
# Sat, 02 Sep 2023 00:15:44 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Sat, 02 Sep 2023 00:15:44 GMT
ARG KONG_VERSION=3.4.0
# Sat, 02 Sep 2023 00:15:44 GMT
ENV KONG_VERSION=3.4.0
# Sat, 02 Sep 2023 00:15:44 GMT
ARG KONG_AMD64_SHA=9a4203174a29895d5dd71092a05b15b26ee9644e068d14d970aed28461d358fa
# Sat, 02 Sep 2023 00:15:45 GMT
ARG KONG_ARM64_SHA=b64e19216ce125039a6a832dc93bf277e05f233a91f1647b351cad3f166edd81
# Sat, 02 Sep 2023 00:16:20 GMT
# ARGS: KONG_AMD64_SHA=9a4203174a29895d5dd71092a05b15b26ee9644e068d14d970aed28461d358fa KONG_ARM64_SHA=b64e19216ce125039a6a832dc93bf277e05f233a91f1647b351cad3f166edd81
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Sat, 02 Sep 2023 00:16:21 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Sat, 02 Sep 2023 00:16:21 GMT
USER kong
# Sat, 02 Sep 2023 00:16:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 02 Sep 2023 00:16:21 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 02 Sep 2023 00:16:21 GMT
STOPSIGNAL SIGQUIT
# Sat, 02 Sep 2023 00:16:21 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Sat, 02 Sep 2023 00:16:21 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:8b5db5f6400d85199afbfde601a9e3c2051ebceb1ed9cc0fe25fe6b91e79afa9`  
		Last Modified: Thu, 17 Aug 2023 19:55:40 GMT  
		Size: 28.4 MB (28392978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299a552b12f9233c187a58c3aef24ace9fb79a42658f23a4e860b3f373cd5004`  
		Last Modified: Sat, 02 Sep 2023 00:17:23 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:525a815ee6ac75ca68b373cac570c8057dcb3f93810151a8024a5b2bd964c6ba`  
		Last Modified: Sat, 02 Sep 2023 00:17:31 GMT  
		Size: 65.8 MB (65765912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4564c33a56aadd89767f6bf2774cee3e9b9cee848309e8248e4fd7f06197d45`  
		Last Modified: Sat, 02 Sep 2023 00:17:23 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
