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
