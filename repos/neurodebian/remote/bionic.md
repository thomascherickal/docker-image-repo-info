## `neurodebian:bionic`

```console
$ docker pull neurodebian@sha256:e8aa2e07ed152271d2a5d637822c89591de036281647a8d0410d0fc2b51c1469
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:bionic` - linux; amd64

```console
$ docker pull neurodebian@sha256:ebab31ec1db3c7acab4884adc54733c64502629cf75e31da74fff1302e0bc095
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31766690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e41018d23fccbd78e4c00c824ee32e87a5594b358633a033db8df77d86a0e4a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 22:59:58 GMT
ADD file:5131314b62b7386e388b173018be7058491e96459344f78e6a2220771a65a2cd in / 
# Thu, 21 Apr 2022 22:59:58 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:59:11 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:59:12 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Fri, 22 Apr 2022 02:59:13 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bionic main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bionic main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Fri, 22 Apr 2022 02:59:18 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:88736512a147458c580cd28c969698561f236abba2ef04dbf0d7940cb3d7375e`  
		Last Modified: Tue, 19 Apr 2022 13:10:00 GMT  
		Size: 26.7 MB (26709883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08256d051e194fbb9e0931a418cf175c40e7b16e79efac7dc42c4c11c99e74e`  
		Last Modified: Fri, 22 Apr 2022 03:01:23 GMT  
		Size: 4.8 MB (4813411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad73344063670c2f04b3a9f2432bd65f7fd1d6641bbd53b300ac09426db0cf8a`  
		Last Modified: Fri, 22 Apr 2022 03:01:22 GMT  
		Size: 3.2 KB (3157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3089680f3e443ef1591b8f55333ac785d1d67c54b8551a66198717f7ca537d5`  
		Last Modified: Fri, 22 Apr 2022 03:01:22 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208df3bf99600b8cf7f0c9cd73ba9180a426f14ff7b8a60c8c0089e3cb4772e2`  
		Last Modified: Fri, 22 Apr 2022 03:01:23 GMT  
		Size: 240.0 KB (239992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
