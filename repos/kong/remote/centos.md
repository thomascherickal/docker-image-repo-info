## `kong:centos`

```console
$ docker pull kong@sha256:176363657cdf7dc411f1d738aae37ff5016542170c9a2696607361cb5cfb9b91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:centos` - linux; amd64

```console
$ docker pull kong@sha256:c59b96b4d57a32a72e9b8be4b6e1c14c6a1e3bb3340d80266fae91460769ef40
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127400802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6ddf4deeb4ee04ebf0f68f79a2ee0486fd26465754de034da59bd93c53d6b5b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 14 Nov 2020 00:20:04 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Sat, 14 Nov 2020 00:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:20:04 GMT
CMD ["/bin/bash"]
# Sat, 14 Nov 2020 01:01:33 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 14 Nov 2020 01:01:33 GMT
ARG ASSET=ce
# Sat, 14 Nov 2020 01:01:34 GMT
ENV ASSET=ce
# Sat, 14 Nov 2020 01:01:34 GMT
ARG EE_PORTS
# Sat, 14 Nov 2020 01:01:34 GMT
COPY file:ff02c070e4c89f043b176279a7e41464b5fab8cb98cfcd6332fad2d2741fc41d in /tmp/kong.rpm 
# Wed, 27 Jan 2021 06:33:26 GMT
ARG KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 06:33:27 GMT
ENV KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 06:33:27 GMT
ARG KONG_SHA256=c95c8306f31eb9bb3fce6d3436d3782eb352dfb17dca10edad8a0f0d982b1219
# Wed, 27 Jan 2021 06:33:56 GMT
# ARGS: KONG_SHA256=c95c8306f31eb9bb3fce6d3436d3782eb352dfb17dca10edad8a0f0d982b1219
RUN set -ex;   if [ "$ASSET" = "ce" ] ; then     curl -fL "https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm" -o /tmp/kong.rpm     && echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -;   fi;   yum install -y -q unzip shadow-utils git   && yum clean all -q   && rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki   && yum install -y /tmp/kong.rpm   && yum clean all   && rm /tmp/kong.rpm   && chown kong:0 /usr/local/bin/kong   && chown -R kong:0 /usr/local/kong &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Wed, 27 Jan 2021 06:33:56 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 27 Jan 2021 06:33:56 GMT
USER kong
# Wed, 27 Jan 2021 06:33:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 27 Jan 2021 06:33:57 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 27 Jan 2021 06:33:57 GMT
STOPSIGNAL SIGQUIT
# Wed, 27 Jan 2021 06:33:57 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4dc7c6a187fe570e563de224bd35775b78d3ff78f05cf73c4e08319b2dc232`  
		Last Modified: Sat, 14 Nov 2020 01:03:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db8e71dccdabe2284554e8e30b0937710417a94f009b08bbbc6c7f88bac451a`  
		Last Modified: Wed, 27 Jan 2021 06:36:22 GMT  
		Size: 51.3 MB (51302781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2de3757aca98a38a9abef3cdbfd3ac04a92c479502e5ae467734ecc9c60fdcc`  
		Last Modified: Wed, 27 Jan 2021 06:36:11 GMT  
		Size: 735.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
