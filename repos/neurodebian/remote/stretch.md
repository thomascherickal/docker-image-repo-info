## `neurodebian:stretch`

```console
$ docker pull neurodebian@sha256:f9e9c03e76f31cf6746389a9a1ade967115dc8d5c1424a92271799eceb4b2222
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:stretch` - linux; amd64

```console
$ docker pull neurodebian@sha256:2bf52e7e17a34d46dd9030cd901f2d14afb33ab3d32780027c3986016595a9e8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.2 MB (52237903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:183007b434fca1ffe3a53d959061a4ce57e729fd561175efa6955c290ebc23dd`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 03:27:22 GMT
ADD file:9f6f0c8b90de3204ad5db95d10d8aa76b42454def6ac811c888ad4e274292c9c in / 
# Thu, 16 Apr 2020 03:27:22 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 10:00:36 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:00:39 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 16 Apr 2020 10:00:40 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian stretch main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel stretch main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 16 Apr 2020 10:00:44 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7568c21980bd8003ca9d23a218302c6386aac91e069cc0c0be6bedf45476f056`  
		Last Modified: Thu, 16 Apr 2020 03:34:47 GMT  
		Size: 45.4 MB (45375910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f15051f30000afc7e520156b3b86dbb6a2a4d0e275cf91ac84be8a8ce626ea`  
		Last Modified: Thu, 16 Apr 2020 10:03:04 GMT  
		Size: 6.6 MB (6566537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e5a1726d1a3e208cef28e078a0be6955529e653b8601e4f0a250f670f0e58e`  
		Last Modified: Thu, 16 Apr 2020 10:03:03 GMT  
		Size: 3.2 KB (3151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5b42d53b95ffd8280360564ce130e4079c8000782e844c6e7e8fb63cf558404`  
		Last Modified: Thu, 16 Apr 2020 10:03:03 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7540718e015313559e4128b7a4deb345b7566e7b064226a883348394e5f451`  
		Last Modified: Thu, 16 Apr 2020 10:03:03 GMT  
		Size: 292.1 KB (292062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
