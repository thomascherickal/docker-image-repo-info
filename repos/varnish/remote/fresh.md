## `varnish:fresh`

```console
$ docker pull varnish@sha256:00632161a7cda1b40d211875daf3ebf171541fb33ef5c9b2a112f32194afe125
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:fresh` - linux; amd64

```console
$ docker pull varnish@sha256:3059c2077201fc5cd6363f3f81c44ae8adad93f2c154f1c89276f24d50f5ac14
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76857008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e72a4600a0e93dd7b07513236c622ef06a4acdc0519ccbc25688d961cf5c40ea`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 22:18:05 GMT
ENV VARNISH_VERSION=6.5.1~buster-1
# Tue, 13 Oct 2020 22:18:05 GMT
ENV VARNISH_SIZE=100M
# Tue, 13 Oct 2020 22:18:27 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A487F9BE81D9DF5121488CFE1C7B4E9FF149D65B; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish65/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:18:27 GMT
WORKDIR /etc/varnish
# Tue, 13 Oct 2020 22:18:28 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Tue, 13 Oct 2020 22:18:28 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Tue, 13 Oct 2020 22:18:28 GMT
EXPOSE 80 8443
# Tue, 13 Oct 2020 22:18:28 GMT
CMD []
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2098ab260e42414bf98043b9205e06f62b960b988a9e48247dade07c5a7db72`  
		Last Modified: Tue, 13 Oct 2020 22:19:17 GMT  
		Size: 49.8 MB (49764306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce057018ac767118d0da6a6bd0fadd5e4338a2eed1a481590c859badbb92e790`  
		Last Modified: Tue, 13 Oct 2020 22:19:08 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
