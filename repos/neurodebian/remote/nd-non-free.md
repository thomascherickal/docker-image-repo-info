## `neurodebian:nd-non-free`

```console
$ docker pull neurodebian@sha256:f2030a908c409718d6c90159421711457ef3fcb26647df373d5566023f7f2990
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:nd-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:4443c48cbd61ef9aa35643ab81923739885f5ac5a940df98e1615bd430be1fbd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66525771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cb8bc2811d70c65ec3844a165dc4664e7d73413b33fdc32bda1c7745fec4bde`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:21:14 GMT
ADD file:5745436941906af011c9450820c7baff61a091235f04da258ba218ca450622a5 in / 
# Wed, 23 Jun 2021 00:21:15 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 07:23:21 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 07:23:24 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 23 Jun 2021 07:23:26 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 23 Jun 2021 07:23:32 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 07:23:40 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:bbd4da8ff6e19a9b86585f9b55dede690ca6dca9f96d946fa1fb6456182931cd`  
		Last Modified: Wed, 23 Jun 2021 00:26:45 GMT  
		Size: 54.9 MB (54902493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a5a2c72313ac51d866c076a89c3540e611bdc73545260c7f70c475df5f1cff`  
		Last Modified: Wed, 23 Jun 2021 07:25:50 GMT  
		Size: 11.3 MB (11309840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92eb70a81ca6327edea84859e4ff141253cb59511431ad3ac6da2f941c3ebdcb`  
		Last Modified: Wed, 23 Jun 2021 07:25:49 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cabfbb93c84835b95d4159a09d34e643b523103be306df0a9dab8f3bf5d6233`  
		Last Modified: Wed, 23 Jun 2021 07:25:49 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497641a826e5d0d1ee92f387abd7e3d1bf39c11c26c1a9c1f962c864ccb9077a`  
		Last Modified: Wed, 23 Jun 2021 07:25:49 GMT  
		Size: 311.1 KB (311111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4528b76019414da81f0f135b11a6bcf180c23a7def44e8561f8b13685c0d9f82`  
		Last Modified: Wed, 23 Jun 2021 07:26:01 GMT  
		Size: 318.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
