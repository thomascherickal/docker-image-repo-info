## `kong:centos`

```console
$ docker pull kong@sha256:432b712e3986f4d29c180c23d05b7218c9e6fdd3d0bfb0cd256bc01dea02c5e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:centos` - linux; amd64

```console
$ docker pull kong@sha256:7b8ef6ec4bade7158d51d1a17a58dfbf53e009aca211cd88f2d11b177598fd9b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.1 MB (127094606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d5cebf1502c6c6ef8091b6e91eef1d301ad2a54a3ad4f93a2d82a1d24f5f81c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:37:24 GMT
LABEL maintainer=Kong <support@konghq.com>
# Mon, 10 Aug 2020 18:37:24 GMT
ARG ASSET=ce
# Mon, 10 Aug 2020 18:37:25 GMT
ENV ASSET=ce
# Mon, 10 Aug 2020 18:37:25 GMT
ARG EE_PORTS
# Mon, 10 Aug 2020 18:37:25 GMT
COPY file:ff02c070e4c89f043b176279a7e41464b5fab8cb98cfcd6332fad2d2741fc41d in /tmp/kong.rpm 
# Thu, 29 Oct 2020 18:22:22 GMT
ARG KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:22:22 GMT
ENV KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:22:22 GMT
ARG KONG_SHA256=17f8a8f5084c7ff0b5807f0a161d900d08f410e4e6fa2c40d469c01604371557
# Thu, 29 Oct 2020 18:22:54 GMT
# ARGS: KONG_SHA256=17f8a8f5084c7ff0b5807f0a161d900d08f410e4e6fa2c40d469c01604371557
RUN set -ex;   if [ "$ASSET" = "ce" ] ; then     curl -fL "https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm" -o /tmp/kong.rpm     && echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -;   fi;   yum install -y -q unzip shadow-utils git   && yum clean all -q   && rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki   && { useradd kong || true ;}   && mkdir -p "/usr/local/kong"   && yum install -y /tmp/kong.rpm   && yum clean all   && rm /tmp/kong.rpm   && chown -R kong:0 /usr/local/kong   && chown kong:0 /usr/local/bin/kong   && chmod -R g=u /usr/local/kong &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Thu, 29 Oct 2020 18:22:55 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 29 Oct 2020 18:22:55 GMT
USER kong
# Thu, 29 Oct 2020 18:22:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Oct 2020 18:22:55 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 29 Oct 2020 18:22:55 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Oct 2020 18:22:56 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c636c1fa5b3254b7692cb41da3aee6a2547a919e7a84290bd6f7c05f9ef334`  
		Last Modified: Mon, 10 Aug 2020 18:39:00 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b6f1cc9a74e605ca58b7e8067ac49e23007ba7ecb0a345dcfca80bdb18b256`  
		Last Modified: Thu, 29 Oct 2020 18:24:21 GMT  
		Size: 51.2 MB (51230557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b780a719739bf794e436031abec561e49f0bda8f6132e6f96ef2112fa7ebea67`  
		Last Modified: Thu, 29 Oct 2020 18:24:10 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
