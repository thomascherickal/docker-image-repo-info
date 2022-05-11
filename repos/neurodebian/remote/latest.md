## `neurodebian:latest`

```console
$ docker pull neurodebian@sha256:2b8befad2d7a844eb38099107d512aadc7fa8183d0d53782b0852254bc45d2fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:latest` - linux; amd64

```console
$ docker pull neurodebian@sha256:c4d110164170d4bdca9e70ce1d770e68c501eb3cce8bffd1761f625fa7427915
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66569291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f0513628c16693a6bebc6d4c3fbc56b68ce329915b051b0188f4a61eb615dea`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:20:05 GMT
ADD file:68a5d7d0db592625159865110c1b7dcb15cf70ecf71b5fd541ef89584cd734ba in / 
# Wed, 11 May 2022 01:20:05 GMT
CMD ["bash"]
# Wed, 11 May 2022 10:06:16 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 10:06:17 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 11 May 2022 10:06:17 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 11 May 2022 10:06:21 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:67e8aa6c8bbc76b1f2bccb3864b0887671833b8667dc1f6c965fcb0eac7e6402`  
		Last Modified: Wed, 11 May 2022 01:24:45 GMT  
		Size: 54.9 MB (54945622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea855485551a969d139bc55b443ef39735688003f23094dd31163dfdbc9495a`  
		Last Modified: Wed, 11 May 2022 10:08:27 GMT  
		Size: 11.3 MB (11310350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753b641df07243055474c63144d947e77b33d6c0e1bf027ed86410a2882f8c6b`  
		Last Modified: Wed, 11 May 2022 10:08:26 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a097ecc215842c963d95b62c41394b9a0379f956773a8093ec6984e0b4c700`  
		Last Modified: Wed, 11 May 2022 10:08:26 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84945c674298e4ba32bd90f45e502196112b0d7877396981a7ae2a26b6b13da`  
		Last Modified: Wed, 11 May 2022 10:08:26 GMT  
		Size: 311.3 KB (311308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
