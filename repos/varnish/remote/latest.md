## `varnish:latest`

```console
$ docker pull varnish@sha256:c7fbf7c5fa5c5b1ee4b512c0237740136d86551f04c54376c80e7436a47ae994
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:latest` - linux; amd64

```console
$ docker pull varnish@sha256:33901580d26fb83093fe4f5d3bf9dc949c6041054e1148cfae3e8a287af760b1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76767889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b6d153e995c84a2649a50836407ea9ea25a4839102e0755010109b045ce2a9e`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 26 Feb 2020 00:37:39 GMT
ADD file:e5a364615e0f6961626089c7d658adbf8c8d95b3ae95a390a8bb33875317d434 in / 
# Wed, 26 Feb 2020 00:37:39 GMT
CMD ["bash"]
# Wed, 25 Mar 2020 21:32:36 GMT
ENV VARNISH_VERSION=6.4.0-1~buster
# Wed, 25 Mar 2020 21:32:37 GMT
ENV VARNISH_SIZE=100M
# Wed, 25 Mar 2020 21:32:57 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A9897320C397E3A60C03E8BF821AD320F71BFF3D; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish64/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Mar 2020 21:32:57 GMT
WORKDIR /etc/varnish
# Wed, 25 Mar 2020 21:32:57 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Wed, 25 Mar 2020 21:32:57 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 25 Mar 2020 21:32:58 GMT
EXPOSE 80 8443
# Wed, 25 Mar 2020 21:32:58 GMT
CMD []
```

-	Layers:
	-	`sha256:68ced04f60ab5c7a5f1d0b0b4e7572c5a4c8cce44866513d30d9df1a15277d6b`  
		Last Modified: Wed, 26 Feb 2020 00:44:23 GMT  
		Size: 27.1 MB (27091819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9baf6d7f5902865b7612b931e32e7fe4d6c4181522242b5ae5c6a3ef70d6b9`  
		Last Modified: Wed, 25 Mar 2020 21:33:31 GMT  
		Size: 49.7 MB (49675617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8f0f9612b31b862a504cee5b804f160110ba8780faf749bdc2825da5f00123`  
		Last Modified: Wed, 25 Mar 2020 21:33:22 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
