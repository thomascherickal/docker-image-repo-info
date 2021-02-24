## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:265fe7751a52d6417642fa98d1b4ce32252251b5fbafd3ce3122874d308a132e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:f0dbd0cc8700d8f2e52d18405f6dfe5977f2ab7bbf901e85cd0ce07a0eea8dcf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.8 MB (542801255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2cefba199f86a2ef9bf699de2d6e3ecb4f979f20a369a7a65928e0b34336d21`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 19:19:48 GMT
ADD file:40bc6ac9b95149d9077e8e692feea2208fcd1c5883673953b295e6acd014ea38 in / 
# Wed, 24 Feb 2021 19:19:48 GMT
CMD ["/bin/bash"]
# Wed, 24 Feb 2021 19:20:21 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-abc7929fca91cdb8ef05600baeb5500309ad7e959bdc5801e05e960937a1887a.tar.gz"  && echo "e0f5a2c5b165bbebd736a75582dc89040c9f64c6d1ddfd84b0421bc44e46de5d  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:9da98c321efd693e1dc19cc24c7c2cfa365c649f178da8ebdfdc5243d0b2f91a`  
		Last Modified: Wed, 24 Feb 2021 10:37:31 GMT  
		Size: 61.9 MB (61935160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdaa1128d47df628000ceea076363b38d2eef08ce7d1c0ab5303f2c990bb90c`  
		Last Modified: Wed, 24 Feb 2021 19:21:23 GMT  
		Size: 480.9 MB (480866095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:255e2711fddbc90e0f7c16eff50c2c60b152b173272155b3156f7b695d67f711
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.5 MB (544490662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:792b8eba21b647bfa2fa93de4a6f8efc6cdcec0ec21ffc227a7e8192165698b4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 24 Feb 2021 18:44:28 GMT
ADD file:e57e27bb2d338405f702e133eb22bfd61d172471ce8bad647c7f7d9b0b30bf7b in / 
# Wed, 24 Feb 2021 18:44:32 GMT
CMD ["/bin/bash"]
# Wed, 24 Feb 2021 18:45:06 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-abc7929fca91cdb8ef05600baeb5500309ad7e959bdc5801e05e960937a1887a.tar.gz"  && echo "e0f5a2c5b165bbebd736a75582dc89040c9f64c6d1ddfd84b0421bc44e46de5d  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:c669744e929468ab3571a83e2386710816116036b648ebd90ecc44d86705b51e`  
		Last Modified: Wed, 24 Feb 2021 18:45:40 GMT  
		Size: 63.6 MB (63624537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad3b7efff34c518f97a45ee14bb41ef9f3cbde804a18a4a1e3f35ee7586bfc5`  
		Last Modified: Wed, 24 Feb 2021 18:46:27 GMT  
		Size: 480.9 MB (480866125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
