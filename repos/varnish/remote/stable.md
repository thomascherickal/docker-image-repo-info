## `varnish:stable`

```console
$ docker pull varnish@sha256:fc367535ad8561eede3f70c78da42bbabcc8f7dc6b7fca78f6c3c1bac2333e38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:stable` - linux; amd64

```console
$ docker pull varnish@sha256:4b1179ccf05f5e10ec3e64d51a907f607bf6d71ea56876185efc7d915fa1f295
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.4 MB (76427200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:290f0f5f0247996f30adf14ccddb45947c03b2fd8f773ecf46aaa5325c8b1a83`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 05:47:28 GMT
ENV VARNISH_VERSION=6.0.7-1~buster
# Tue, 09 Feb 2021 05:47:28 GMT
ENV VARNISH_SIZE=100M
# Tue, 09 Feb 2021 05:47:59 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 05:47:59 GMT
WORKDIR /etc/varnish
# Tue, 09 Feb 2021 05:48:00 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Tue, 09 Feb 2021 05:48:00 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Tue, 09 Feb 2021 05:48:01 GMT
EXPOSE 80 8443
# Tue, 09 Feb 2021 05:48:01 GMT
CMD []
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20dfa6a567c7d7279901ab79584eafb4b55c876cf9c9611cee00ebd9c5d28dd1`  
		Last Modified: Tue, 09 Feb 2021 05:49:15 GMT  
		Size: 49.3 MB (49331586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3876a2e6424c3222ea7f318ee87a8f0176471730ee5ac46e6fd7db55451958`  
		Last Modified: Tue, 09 Feb 2021 05:49:03 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
