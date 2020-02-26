## `varnish:stable`

```console
$ docker pull varnish@sha256:6fca0ca2946aaeb1bed34d64811b4d93a6ae1dd36bb64793d19e5a7f47225bcb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:stable` - linux; amd64

```console
$ docker pull varnish@sha256:bc1215bb451808d6e9a630ea7bc0f0213888d42f0b7a2da20a13599560615f19
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67208195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc9abde2874739c518e1533e38e737c63924ba32492b553623351a61bfa521bf`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `["varnishd","-F","-f","\/etc\/varnish\/default.vcl"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:38 GMT
ADD file:1256c62f77a54c982fdb2790d682049b2ad64c8466466e846f3d33ad1ed4035d in / 
# Wed, 26 Feb 2020 00:41:38 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 20:13:14 GMT
ENV VARNISH_VERSION=6.0.6-1~stretch
# Wed, 26 Feb 2020 20:13:38 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver http://ha.pool.sks-keyservers.net/ --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ stretch main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 20:13:38 GMT
WORKDIR /etc/varnish
# Wed, 26 Feb 2020 20:13:38 GMT
COPY file:0301ec458d312e5c085462f916888bc85bb94c134ed6116667d225487db56cac in /usr/local/bin/ 
# Wed, 26 Feb 2020 20:13:39 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 26 Feb 2020 20:13:39 GMT
EXPOSE 80
# Wed, 26 Feb 2020 20:13:39 GMT
CMD ["varnishd" "-F" "-f" "/etc/varnish/default.vcl"]
```

-	Layers:
	-	`sha256:6d28e14ab8c85bf8a4331de0667c27d19ef4092b12531eec0334b5c2a1012668`  
		Last Modified: Wed, 26 Feb 2020 00:47:21 GMT  
		Size: 22.5 MB (22513365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cfb65f89d166776d2e4d51f0b61d8d5b77e2fd384e359e8be6c4e95ac22975c`  
		Last Modified: Wed, 26 Feb 2020 20:14:15 GMT  
		Size: 44.7 MB (44694450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b867613e54808b6c7235a9814e282571ad4aa9d9e541f3e4cb3efce3ff137b9`  
		Last Modified: Wed, 26 Feb 2020 20:14:07 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
