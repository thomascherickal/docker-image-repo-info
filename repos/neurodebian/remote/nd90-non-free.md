## `neurodebian:nd90-non-free`

```console
$ docker pull neurodebian@sha256:ccfe48cad85d360fec483025b020df1b5a520d45f5b074b4dec2322e0b898b99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:nd90-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:9cfeb8ab7b5745a4ac3e0ba6c1065a9d65ed1e54a2fdef454d16d7cf5ca63f61
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.2 MB (52242742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd80cd6c3b035173594de55ca80388718ced248e556dcb4a8837ced70e610a32`
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
# Sat, 28 Dec 2019 23:27:21 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
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
	-	`sha256:8e5b654632a20433497d3eab7d41d94a83e077210c074e0a0d9589a19bef4876`  
		Last Modified: Sat, 28 Dec 2019 23:29:11 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
