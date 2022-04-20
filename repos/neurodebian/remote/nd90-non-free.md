## `neurodebian:nd90-non-free`

```console
$ docker pull neurodebian@sha256:3042dcce25838b1f570e3e7bfdbbe7aa00e4da2d36145615291622f5f3828896
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd90-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:8dca56d8137061c244f2ef70e7f29bf89e6ccc1e413d2ebc4b161963bd23b0d9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.3 MB (52296165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a079ddb63e84f6cf1e59917bb891258e75c3bf2d1ad7762e8ed2538aceac792`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:45:14 GMT
ADD file:6ed691b65385dede44a92f9de9e1428af431197c66461aa0f9c61e2f7c8bade5 in / 
# Wed, 20 Apr 2022 04:45:15 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 10:08:16 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:08:20 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 20 Apr 2022 10:08:20 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian stretch main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel stretch main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 20 Apr 2022 10:08:24 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:08:27 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:f5196cdf25181bc7e4411865a2e002932b7b6b0ffce787c04c1bdeaf1f204f20`  
		Last Modified: Wed, 20 Apr 2022 04:52:01 GMT  
		Size: 45.4 MB (45427434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a812c03c0e763f65d03ca72ad204f87a76a3b726aa42c4eafcfc390b1ad7d7ab`  
		Last Modified: Wed, 20 Apr 2022 10:10:29 GMT  
		Size: 6.6 MB (6572683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546378b26d459e11734b4b8d52f619001b18f9d00e51ff097da668dcaaefcaff`  
		Last Modified: Wed, 20 Apr 2022 10:10:28 GMT  
		Size: 3.2 KB (3155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4daa8fca6f010c46f391b5e8d6353ed673bd1ce1937f99d79fa5bd8e84fe6a91`  
		Last Modified: Wed, 20 Apr 2022 10:10:28 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a8f952b638747e5d48931d78357e16c80040ca3efbe31067e233cd35da5a5b`  
		Last Modified: Wed, 20 Apr 2022 10:10:28 GMT  
		Size: 292.3 KB (292287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4198a3aed48299adb61402bee4fcefe0586496ebe2222d7203620c44e25ea0ff`  
		Last Modified: Wed, 20 Apr 2022 10:10:38 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
