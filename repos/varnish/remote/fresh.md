## `varnish:fresh`

```console
$ docker pull varnish@sha256:d2756c2e203b7a7234344495da5eac0b1545bf8edd321338954db1cee15dd11d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:fresh` - linux; amd64

```console
$ docker pull varnish@sha256:796047dc0a7834892d2c19778557213ee79b921ed33d701b17e2f5486e19137b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76767230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d43ade62147980441582d1faa915652ae0e59ab6b468e43383f7600a83ff15a`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:23:57 GMT
ENV VARNISH_VERSION=6.4.0-1~buster
# Tue, 04 Aug 2020 23:23:57 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Aug 2020 22:21:51 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A9897320C397E3A60C03E8BF821AD320F71BFF3D; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish64/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Aug 2020 22:21:51 GMT
WORKDIR /etc/varnish
# Wed, 12 Aug 2020 22:21:51 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Wed, 12 Aug 2020 22:21:51 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 12 Aug 2020 22:21:52 GMT
EXPOSE 80 8443
# Wed, 12 Aug 2020 22:21:52 GMT
CMD []
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c137904a1e0e9fad90bdcb8cc1aa3de75751e58327f7f3e551b8204c76fcd24`  
		Last Modified: Wed, 12 Aug 2020 22:22:26 GMT  
		Size: 49.7 MB (49674657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6224d37fa9015c5b8e012e19ff5e49f04dfa0ab58e9d832e30b4625ba8787403`  
		Last Modified: Wed, 12 Aug 2020 22:22:17 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
