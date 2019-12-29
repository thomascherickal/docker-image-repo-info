## `neurodebian:stretch`

```console
$ docker pull neurodebian@sha256:8064285fb2e3a650bb42d32392944c0dd3ecd3bbbea8e6993a695b61925a5892
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:stretch` - linux; amd64

```console
$ docker pull neurodebian@sha256:25dc0570a5530d67d8b6512b9344bb53040f1aef870b36f53777ed57713eb0b5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.2 MB (52242376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9342fd70df9d8985149e0dd86765eff1a1c2b07b706db3331cad04dfe502b2c`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:33 GMT
ADD file:8f7dc710e276f54a3a73d34b6b8fa261950a781d68ceb7401fa18dabc601c5a5 in / 
# Sat, 28 Dec 2019 04:23:34 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 23:27:07 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 23:27:10 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 28 Dec 2019 23:27:11 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian stretch main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel stretch main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 28 Dec 2019 23:27:15 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:146bd6a886182fde06fbf747470b1c89814bc8ab1c96fdf1aef6107171959fe6`  
		Last Modified: Sat, 28 Dec 2019 04:28:25 GMT  
		Size: 45.4 MB (45380744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea06d146a6a39fb01281d249dac15e77920e4b325e5a7157409ca968449f6fab`  
		Last Modified: Sat, 28 Dec 2019 23:29:08 GMT  
		Size: 6.6 MB (6566499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51aa5f00a0ed10a226340d9dbdb2a20a378418cf94926eb930613c768e36949`  
		Last Modified: Sat, 28 Dec 2019 23:29:08 GMT  
		Size: 3.2 KB (3153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454916bf956d33fc796b4a868fb5618afaa12d498477c90f0ba1c6f113c4f264`  
		Last Modified: Sat, 28 Dec 2019 23:29:08 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8b8da32a9c22883b4aaeaa02de1f2b994becb2dee0a14f9ecfe375fbbf3fe5`  
		Last Modified: Sat, 28 Dec 2019 23:29:07 GMT  
		Size: 291.7 KB (291736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
