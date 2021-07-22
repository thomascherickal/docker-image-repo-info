## `neurodebian:bullseye`

```console
$ docker pull neurodebian@sha256:2625e7de7abd3d04ee57f37abc72558026048e8cc0023c85172483d478234569
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:bullseye` - linux; amd64

```console
$ docker pull neurodebian@sha256:0343475923907c9b0cb0d89e641a15e43a21a575aeecb7da3728ac287f81bef7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66527511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:538cbb0a079bab74399e2747907f54adb09fe1eec0d5aac09fc130aaa5e7286c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:02 GMT
ADD file:fca2ea6b8fc69f3efb8a2f21cd3877d23a9ee3fbeee6ebe4fe21541cd1606a8c in / 
# Thu, 22 Jul 2021 00:45:03 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 09:51:57 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 09:51:58 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 22 Jul 2021 09:51:59 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 22 Jul 2021 09:52:03 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a72d62e9d2fef13cf62e5d212cc6a3751b5c388cc6657bebf4dabc0ca3603cb`  
		Last Modified: Thu, 22 Jul 2021 00:49:21 GMT  
		Size: 54.9 MB (54904849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f80af7c5f675200465ac739aa50787ad204858b7e71bb0a4ce96ed41e44d53`  
		Last Modified: Thu, 22 Jul 2021 09:54:42 GMT  
		Size: 11.3 MB (11309473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70904cebde341b794981e76734af21ac7319970107e56dc693bb209e413cd75f`  
		Last Modified: Thu, 22 Jul 2021 09:54:40 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e537da9c3e2291faac290662b5c173737fdea9b60ba742794e974b604ecb76`  
		Last Modified: Thu, 22 Jul 2021 09:54:40 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0950288e46c4a44c74f59f4162507b0387c96e3bfdf4c4d0a291dba6da95b498`  
		Last Modified: Thu, 22 Jul 2021 09:54:40 GMT  
		Size: 311.2 KB (311175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
