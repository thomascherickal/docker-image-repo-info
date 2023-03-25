## `kong:ubuntu`

```console
$ docker pull kong@sha256:86f9b1e316dcddeb30dc045cedd239d8573bff4d8acbf231f7d11902c1a83adf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:f5f51af49fa1f5a7600e60bb51ebd760b16fd020bb16bba2b70d36a54f3d6ac8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.4 MB (74381601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b5a4a92323976685af4f320261472e8c4575583169192c82d27e246681fc216`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Sat, 25 Mar 2023 00:51:10 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Sat, 25 Mar 2023 00:51:10 GMT
ARG ASSET=ce
# Sat, 25 Mar 2023 00:51:10 GMT
ENV ASSET=ce
# Sat, 25 Mar 2023 00:51:10 GMT
ARG EE_PORTS
# Sat, 25 Mar 2023 00:51:11 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Sat, 25 Mar 2023 00:51:11 GMT
ARG KONG_VERSION=3.2.2
# Sat, 25 Mar 2023 00:51:11 GMT
ENV KONG_VERSION=3.2.2
# Sat, 25 Mar 2023 00:51:11 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Sat, 25 Mar 2023 00:51:11 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Sat, 25 Mar 2023 00:52:03 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Sat, 25 Mar 2023 00:52:04 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Sat, 25 Mar 2023 00:52:04 GMT
USER kong
# Sat, 25 Mar 2023 00:52:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Mar 2023 00:52:04 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 25 Mar 2023 00:52:04 GMT
STOPSIGNAL SIGQUIT
# Sat, 25 Mar 2023 00:52:04 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Sat, 25 Mar 2023 00:52:04 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a798f30a08e58465197ea53af5348cb1920b409dce739c8c1191fa526b779c26`  
		Last Modified: Sat, 25 Mar 2023 00:52:51 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:192c4afa29b67585a708114ac6e302a8de969f95b6037af093514f0b41e1a873`  
		Last Modified: Sat, 25 Mar 2023 00:52:58 GMT  
		Size: 44.0 MB (43950354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8497c811ba9ee1b3aa10434828370b73152317680fd95a5b7718672c3cfb2b2c`  
		Last Modified: Sat, 25 Mar 2023 00:52:51 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:4d0e6518979970d7795ebfd3996daa3f6f2414ed7a2282ba15c35ac299dc4f50
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.5 MB (78466508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad2ac3aea873b6b79878a75119e8b9481f7bb257b98bccb497854f6567a738bc`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Fri, 24 Mar 2023 23:39:31 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 24 Mar 2023 23:39:31 GMT
ARG ASSET=ce
# Fri, 24 Mar 2023 23:39:31 GMT
ENV ASSET=ce
# Fri, 24 Mar 2023 23:39:31 GMT
ARG EE_PORTS
# Fri, 24 Mar 2023 23:39:31 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 24 Mar 2023 23:39:32 GMT
ARG KONG_VERSION=3.2.2
# Fri, 24 Mar 2023 23:39:32 GMT
ENV KONG_VERSION=3.2.2
# Fri, 24 Mar 2023 23:39:32 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Fri, 24 Mar 2023 23:39:32 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Fri, 24 Mar 2023 23:40:38 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 24 Mar 2023 23:40:38 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 24 Mar 2023 23:40:39 GMT
USER kong
# Fri, 24 Mar 2023 23:40:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Mar 2023 23:40:39 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Mar 2023 23:40:39 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Mar 2023 23:40:39 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 24 Mar 2023 23:40:39 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc7b355e64c2bd4ae186d762e75dcf38abb3a3a38feca3d07c5de89f24c54b6`  
		Last Modified: Fri, 24 Mar 2023 23:41:11 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cca0f56b895a7954dcff8ef25eac39c8aaa299cee84f520714508573ee2cee`  
		Last Modified: Fri, 24 Mar 2023 23:41:17 GMT  
		Size: 50.1 MB (50077673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09190020715369973a3868d7c33a1e59d33c39a77be8a68ed47d9a875256f22`  
		Last Modified: Fri, 24 Mar 2023 23:41:11 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
