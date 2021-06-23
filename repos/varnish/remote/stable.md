## `varnish:stable`

```console
$ docker pull varnish@sha256:9308b1705476a5fe67b659e8d3250a66fc9fc6c868e7ed13268d8ffa56eb9e73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:stable` - linux; amd64

```console
$ docker pull varnish@sha256:772332d6a1d82a34c2f33b90de602d70563f23869db23f100302cef9b6f4b49e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76482138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f8ee11ac6ce7b70dbb30c1cc1e4d3005686bbbb9a7263b26c0e14a01c5a3090`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 18:27:49 GMT
ENV VARNISH_VERSION=6.0.7-1~buster
# Wed, 23 Jun 2021 18:27:49 GMT
ENV VARNISH_SIZE=100M
# Wed, 23 Jun 2021 18:28:10 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 18:28:11 GMT
WORKDIR /etc/varnish
# Wed, 23 Jun 2021 18:28:11 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 23 Jun 2021 18:28:11 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 23 Jun 2021 18:28:11 GMT
EXPOSE 80 8443
# Wed, 23 Jun 2021 18:28:12 GMT
CMD []
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc52b1199388d019eb0f4cf5b62f00b50d816a2fcec674487c20e73e2738c6d`  
		Last Modified: Wed, 23 Jun 2021 18:29:28 GMT  
		Size: 49.3 MB (49335585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e87b33fddabbe2bf5003d04073075a36b0c3a24661cb3cad7bb8bc9d100dd72`  
		Last Modified: Wed, 23 Jun 2021 18:29:19 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
