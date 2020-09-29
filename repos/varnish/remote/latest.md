## `varnish:latest`

```console
$ docker pull varnish@sha256:f0cdc07eb324dc606f0f4ddac694175c46bf2b9a89270f1a66eb5c8dc3feff36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:latest` - linux; amd64

```console
$ docker pull varnish@sha256:3ae450886dc562faf9e510979f26ee7ec10d72c120cad4b48459aaadebbd7d6d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76857242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d495419413223e60e819ba0a134df4052381ea765a552d1ed0760db85685285a`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 10 Sep 2020 00:23:29 GMT
ADD file:e7407f2294ad23634565820b9669b18ff2a2ca0212a7ec84b9c89d8550859954 in / 
# Thu, 10 Sep 2020 00:23:30 GMT
CMD ["bash"]
# Tue, 29 Sep 2020 01:56:56 GMT
ENV VARNISH_VERSION=6.5.1~buster-1
# Tue, 29 Sep 2020 01:56:56 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Sep 2020 01:57:16 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A487F9BE81D9DF5121488CFE1C7B4E9FF149D65B; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish65/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Sep 2020 01:57:17 GMT
WORKDIR /etc/varnish
# Tue, 29 Sep 2020 01:57:17 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Tue, 29 Sep 2020 01:57:17 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Tue, 29 Sep 2020 01:57:17 GMT
EXPOSE 80 8443
# Tue, 29 Sep 2020 01:57:17 GMT
CMD []
```

-	Layers:
	-	`sha256:d121f8d1c4128ebc1e95e5bfad90a0189b84eadbbb2fbaad20cbb26d20b2c8a2`  
		Last Modified: Thu, 10 Sep 2020 00:34:02 GMT  
		Size: 27.1 MB (27092161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1094de8696c7a718c5851f6263d73b3872c664bffee5e004cf74846b06d451a4`  
		Last Modified: Tue, 29 Sep 2020 01:57:45 GMT  
		Size: 49.8 MB (49764606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:016497474304618d87eb702b565a0d0d0709745ad8c6e76118249c345d24dcf2`  
		Last Modified: Tue, 29 Sep 2020 01:57:36 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
