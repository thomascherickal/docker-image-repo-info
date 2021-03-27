## `varnish:stable`

```console
$ docker pull varnish@sha256:957807c4e02d0c33385f19a9d5095d4147127c53cd5ede7e9485347401c976d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:stable` - linux; amd64

```console
$ docker pull varnish@sha256:fbf80ec71ece3271b7b87872b1bde1271db99786ad568e9c734b333d9cebca6a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.4 MB (76436759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b77668bae4795f04befdc105189d713cd48fb938874dc00886c040c212b188b2`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 26 Mar 2021 15:20:59 GMT
ADD file:b2085f4b0a7cb0e5754874c712254e5cd941062b27b8d7ed2080520196b91597 in / 
# Fri, 26 Mar 2021 15:20:59 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 10:16:11 GMT
ENV VARNISH_VERSION=6.0.7-1~buster
# Sat, 27 Mar 2021 10:16:12 GMT
ENV VARNISH_SIZE=100M
# Sat, 27 Mar 2021 10:16:30 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 10:16:30 GMT
WORKDIR /etc/varnish
# Sat, 27 Mar 2021 10:16:30 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Sat, 27 Mar 2021 10:16:31 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Sat, 27 Mar 2021 10:16:31 GMT
EXPOSE 80 8443
# Sat, 27 Mar 2021 10:16:31 GMT
CMD []
```

-	Layers:
	-	`sha256:ac2522cc72690febc428fb46fb39a4efc5e0a721c3ad15d9992b01515f2fad1a`  
		Last Modified: Fri, 26 Mar 2021 15:27:47 GMT  
		Size: 27.1 MB (27100996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c937c76920eabaacdd92359cc4d6c972e16c157279b8169969d8f54efb7f5d1`  
		Last Modified: Sat, 27 Mar 2021 10:17:53 GMT  
		Size: 49.3 MB (49335288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8811b6f861fa73a0edac0430ae8ab98617e74c8f2cd18a18f82fe991182bbf`  
		Last Modified: Sat, 27 Mar 2021 10:17:45 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
