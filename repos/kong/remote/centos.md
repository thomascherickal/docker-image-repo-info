## `kong:centos`

```console
$ docker pull kong@sha256:29f839eedc97022967ae46e0ec2ba5dfe75b37525c409b475b7a61a7c0e0ee91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:centos` - linux; amd64

```console
$ docker pull kong@sha256:033decce472824142c52050eeb2ad85a24f1f775d00888d421ad065b3113e223
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.9 MB (160921195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5212ef94876a94444a623c7c826d7ea5bd5d0fce1958eb2cd472a8a0f58befd1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:04 GMT
ADD file:805cb5e15fb6e0bb0326ca33fd2942e068863ce2a8491bb71522c652f31fb466 in / 
# Wed, 15 Sep 2021 18:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20210915
# Wed, 15 Sep 2021 18:20:05 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 23:21:23 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 15 Sep 2021 23:21:23 GMT
ARG ASSET=ce
# Wed, 15 Sep 2021 23:21:23 GMT
ENV ASSET=ce
# Wed, 15 Sep 2021 23:21:24 GMT
ARG EE_PORTS
# Wed, 15 Sep 2021 23:21:24 GMT
COPY file:ff02c070e4c89f043b176279a7e41464b5fab8cb98cfcd6332fad2d2741fc41d in /tmp/kong.rpm 
# Wed, 15 Sep 2021 23:21:24 GMT
ARG KONG_VERSION=2.5.1
# Wed, 15 Sep 2021 23:21:24 GMT
ENV KONG_VERSION=2.5.1
# Wed, 15 Sep 2021 23:21:24 GMT
ARG KONG_SHA256=36c03c53a4e3a3f6f0968f68258fa93a584af5c33ed29fa5e05e089dfb97b730
# Wed, 15 Sep 2021 23:21:58 GMT
# ARGS: KONG_SHA256=36c03c53a4e3a3f6f0968f68258fa93a584af5c33ed29fa5e05e089dfb97b730
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then       curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-centos-7/Packages/k/kong-$KONG_VERSION.el7.amd64.rpm -o /tmp/kong.rpm       && echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -;     fi;     yum install -y -q unzip shadow-utils git     && yum clean all -q     && rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki     && yum install -y /tmp/kong.rpm     && yum clean all     && rm /tmp/kong.rpm     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 15 Sep 2021 23:21:59 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 15 Sep 2021 23:21:59 GMT
USER kong
# Wed, 15 Sep 2021 23:21:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 15 Sep 2021 23:22:00 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 15 Sep 2021 23:22:00 GMT
STOPSIGNAL SIGQUIT
# Wed, 15 Sep 2021 23:22:00 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 15 Sep 2021 23:22:00 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a1d0c75327776413fa0db9ed3adcdbadedc95a662eb1d360dad82bb913f8a1d1`  
		Last Modified: Wed, 15 Sep 2021 18:21:25 GMT  
		Size: 83.5 MB (83518086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fb8a137fa2b84d66997b2207a6880267b365a0a2d08a22a00c4965ecbec7f93`  
		Last Modified: Wed, 15 Sep 2021 23:23:25 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5520f68e079f5dbe56c351330fdc8e5688d18f21e5b3059e73da20ea1f82e79c`  
		Last Modified: Wed, 15 Sep 2021 23:23:37 GMT  
		Size: 77.4 MB (77402098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af293b6ea93ad38f2ce79b696ebdcf75d1917845c0eaf599089bea1eec48e287`  
		Last Modified: Wed, 15 Sep 2021 23:23:25 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
