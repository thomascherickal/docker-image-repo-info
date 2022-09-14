## `kong:ubuntu`

```console
$ docker pull kong@sha256:8d61de4b25fcae2d7e0c3368f485486ef9132cec892b53657a79c2eaba544fe6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:e1b7a02b9e7a135b191170fde9406935383d015b7219c3a198a068430a68a29d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.7 MB (126666532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba3d56c232a3c9280f7ca9ed88c42b20112ba4997ef20356f1dc00c442f7d012`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Wed, 14 Sep 2022 00:07:33 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 14 Sep 2022 00:07:33 GMT
ARG ASSET=ce
# Wed, 14 Sep 2022 00:07:33 GMT
ENV ASSET=ce
# Wed, 14 Sep 2022 00:07:33 GMT
ARG EE_PORTS
# Wed, 14 Sep 2022 00:07:33 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 14 Sep 2022 00:07:34 GMT
ARG KONG_VERSION=3.0.0
# Wed, 14 Sep 2022 00:07:34 GMT
ENV KONG_VERSION=3.0.0
# Wed, 14 Sep 2022 00:07:34 GMT
ARG KONG_AMD64_SHA=3a38f6c4ba1cfc8897e655e46b957c7b0f2dd930111bf3d02411fedd1de53d6d
# Wed, 14 Sep 2022 00:07:34 GMT
ARG KONG_ARM64_SHA=190f82dd47df19339c025f37701e62191aa3063e77e15c5e57d5b77869058f69
# Wed, 14 Sep 2022 00:08:34 GMT
# ARGS: KONG_AMD64_SHA=3a38f6c4ba1cfc8897e655e46b957c7b0f2dd930111bf3d02411fedd1de53d6d KONG_ARM64_SHA=190f82dd47df19339c025f37701e62191aa3063e77e15c5e57d5b77869058f69
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 14 Sep 2022 00:08:35 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 14 Sep 2022 00:08:35 GMT
USER kong
# Wed, 14 Sep 2022 00:08:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Sep 2022 00:08:35 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 14 Sep 2022 00:08:35 GMT
STOPSIGNAL SIGQUIT
# Wed, 14 Sep 2022 00:08:35 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 14 Sep 2022 00:08:36 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f8ea18d6c5f278fa5820835cb24eea6a767e0f2db8069fa45a0a1a2e56c4b68`  
		Last Modified: Wed, 14 Sep 2022 00:09:51 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1fcce01ccb3758b7e74adaa6b4b0cb227b2ce8c0dde5c431af462be4e1fe93`  
		Last Modified: Wed, 14 Sep 2022 00:10:02 GMT  
		Size: 73.0 MB (73011012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a8c5f807f396934e8a026572c5fdc4c0ef99588049369adfdaac08e05f1d34`  
		Last Modified: Wed, 14 Sep 2022 00:09:50 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:7b2bf1303f661c575da457a9046b9620590b17bed4890b88bac7e818277a17a2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.7 MB (121715925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8824d66ce1a3f044fb009a0dd979f97b8dbf80491e6fa2a55c138baab821271e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:45:21 GMT
ARG ASSET=ce
# Fri, 02 Sep 2022 06:45:21 GMT
ENV ASSET=ce
# Fri, 02 Sep 2022 06:45:22 GMT
ARG EE_PORTS
# Fri, 02 Sep 2022 06:45:24 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Fri, 02 Sep 2022 06:45:24 GMT
ARG KONG_VERSION=2.8.1
# Fri, 02 Sep 2022 06:45:25 GMT
ENV KONG_VERSION=2.8.1
# Fri, 02 Sep 2022 06:45:26 GMT
ARG KONG_AMD64_SHA=10d12d23e5890414d666663094d51a42de41f8a9806fbc0baaf9ac4d37794361
# Fri, 02 Sep 2022 06:45:27 GMT
ARG KONG_ARM64_SHA=61c13219ef64dac9aeae5ae775411e8cfcd406f068cf3e75d463f916ae6513cb
# Fri, 02 Sep 2022 06:45:56 GMT
# ARGS: KONG_AMD64_SHA=10d12d23e5890414d666663094d51a42de41f8a9806fbc0baaf9ac4d37794361 KONG_ARM64_SHA=61c13219ef64dac9aeae5ae775411e8cfcd406f068cf3e75d463f916ae6513cb
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 02 Sep 2022 06:45:57 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 02 Sep 2022 06:45:57 GMT
USER kong
# Fri, 02 Sep 2022 06:45:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 06:45:59 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 02 Sep 2022 06:46:00 GMT
STOPSIGNAL SIGQUIT
# Fri, 02 Sep 2022 06:46:01 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 02 Sep 2022 06:46:02 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37921fee9fdc77f083b1d7e6150fcc91eaf74164601930750627e75ec46159c9`  
		Last Modified: Fri, 02 Sep 2022 06:50:16 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b2eb7f3cec9c8ba77ac0b9ea6c162a9999e3a4375f390e6e44c94e701bca00a`  
		Last Modified: Fri, 02 Sep 2022 06:50:26 GMT  
		Size: 69.4 MB (69441275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd6508437ef72723b0df33a3e5356b79b4143a273c6e2b63819b32a60b10904`  
		Last Modified: Fri, 02 Sep 2022 06:50:14 GMT  
		Size: 879.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
