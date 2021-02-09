## `varnish:fresh`

```console
$ docker pull varnish@sha256:a27a3d7bfbf120d47922c1b66aa44d687a2493b5adeeb4a8b7764802ab9bc2cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:fresh` - linux; amd64

```console
$ docker pull varnish@sha256:e1825f20b68d29e767ffff669e4810f7c8b798ec4e07594cb32ec3cde8782710
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76879513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e5af435995c43af24ca4783959c786678e443199351bb6796b7b61f5eb89cfe`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 05:48:09 GMT
ENV VARNISH_VERSION=6.5.1~buster-1
# Tue, 09 Feb 2021 05:48:09 GMT
ENV VARNISH_SIZE=100M
# Tue, 09 Feb 2021 05:48:40 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A487F9BE81D9DF5121488CFE1C7B4E9FF149D65B; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish65/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 05:48:41 GMT
WORKDIR /etc/varnish
# Tue, 09 Feb 2021 05:48:41 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Tue, 09 Feb 2021 05:48:42 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Tue, 09 Feb 2021 05:48:42 GMT
EXPOSE 80 8443
# Tue, 09 Feb 2021 05:48:42 GMT
CMD []
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f677df2a1a87e1951ea3392da24fd632ce4e01e2c59ef3e290f068fe46cd184d`  
		Last Modified: Tue, 09 Feb 2021 05:49:34 GMT  
		Size: 49.8 MB (49783901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284e7abab5e4e2981ba2e8558632cf9851c36e399ca378fc26bff87d2cf9877f`  
		Last Modified: Tue, 09 Feb 2021 05:49:23 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
