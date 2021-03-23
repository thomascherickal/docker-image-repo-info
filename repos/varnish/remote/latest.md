## `varnish:latest`

```console
$ docker pull varnish@sha256:8cf38287c290c9d68300b5b396c6a8db796a55a5fdb8a912dfab5eae709c854f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:latest` - linux; amd64

```console
$ docker pull varnish@sha256:abbe9f98f1c26796a2014fc559d30be444b9039f5035f8e6dd96bfe07f872343
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (77020532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4f88e08735c4645e54cb279987d3b4dabe6a2d25f125da671e007bbb4eb337e`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Mar 2021 02:20:40 GMT
ADD file:3c32f1cd03198e141dd233a7ffd13444157d4150ad917d548f3ee9bf5953ce22 in / 
# Fri, 12 Mar 2021 02:20:41 GMT
CMD ["bash"]
# Tue, 23 Mar 2021 01:30:20 GMT
ENV VARNISH_VERSION=6.6.0-1~buster
# Tue, 23 Mar 2021 01:30:20 GMT
ENV VARNISH_SIZE=100M
# Tue, 23 Mar 2021 01:30:38 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A0378A38E4EACA3660789E570BAC19E3F6C90CD5; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish66/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Mar 2021 01:30:38 GMT
WORKDIR /etc/varnish
# Tue, 23 Mar 2021 01:30:39 GMT
COPY file:f2d309dd6f06236e6a883ab100c62fc6396ac93510452f7833d2089b005f3213 in /usr/local/bin/ 
# Tue, 23 Mar 2021 01:30:39 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Tue, 23 Mar 2021 01:30:39 GMT
EXPOSE 80 8443
# Tue, 23 Mar 2021 01:30:39 GMT
CMD []
```

-	Layers:
	-	`sha256:6f28985ad1843afd6fd4fe0b42a30bfab63c27d302362e7341e3316e8ba25ced`  
		Last Modified: Fri, 12 Mar 2021 02:26:11 GMT  
		Size: 27.1 MB (27101001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05740eb791f9a263fc983f531f772cc92536f0f328e8ed09069136937c7dab00`  
		Last Modified: Tue, 23 Mar 2021 01:31:08 GMT  
		Size: 49.9 MB (49919058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ad7f3b793d6b86898063f4a21a5d5112c25af58e5c71368f95f5f0344409b`  
		Last Modified: Tue, 23 Mar 2021 01:30:59 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
