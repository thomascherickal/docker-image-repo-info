## `varnish:latest`

```console
$ docker pull varnish@sha256:09a2a01d6d41c5cc88c9d85e750c2b031dce4c909a1b4865cf25f01a12b6f213
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:latest` - linux; amd64

```console
$ docker pull varnish@sha256:d7878aa0cbbdca4a33883edb7daa259de272e809cb8018f1fe99a9451735591c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76774853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ce9bdf363596a6e335f526f99de9bfdcd5598ccb05b9e47de9a9b62d09cb432`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:28:20 GMT
ENV VARNISH_VERSION=6.4.0-1~buster
# Fri, 15 May 2020 17:28:20 GMT
ENV VARNISH_SIZE=100M
# Fri, 15 May 2020 17:28:46 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A9897320C397E3A60C03E8BF821AD320F71BFF3D; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish64/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:28:46 GMT
WORKDIR /etc/varnish
# Fri, 15 May 2020 17:28:47 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Fri, 15 May 2020 17:28:47 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Fri, 15 May 2020 17:28:47 GMT
EXPOSE 80 8443
# Fri, 15 May 2020 17:28:47 GMT
CMD []
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ed80e2c033a5c92c8910b2d74a0913592f80017f593e9b46be2274e7cdad48`  
		Last Modified: Fri, 15 May 2020 17:30:07 GMT  
		Size: 49.7 MB (49675645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1f398e3c208fd74434937915d6c020fb90dcee00d6298697ef141aa79fbec4`  
		Last Modified: Fri, 15 May 2020 17:29:36 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
