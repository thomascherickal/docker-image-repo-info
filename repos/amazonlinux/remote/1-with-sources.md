## `amazonlinux:1-with-sources`

```console
$ docker pull amazonlinux@sha256:728fe610c29c4b3d89fbd2447cbacf5e0861e813474b903bce48d54a0b95d9b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:ff807c30a818c92b6c322b8f8a9cda7642253c632f7f7deb3e28968fea38bd7f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **449.3 MB (449256394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a38785f24e771e397d1d05b265eb5cb9eb1cb94e223d4aeb075b78df1d94e38`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 23 Dec 2020 20:20:50 GMT
ADD file:fad21d2914f8429ddebb886e5d03ca48b4cb36eccac1e691bb6ed0f9cb7a6f03 in / 
# Wed, 23 Dec 2020 20:20:50 GMT
CMD ["/bin/bash"]
# Wed, 23 Dec 2020 20:21:13 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-8332ab379854aecfcd3ddf9c79744dfabb59c3b3aace63aaa61c9a99d8632bf1.tar.gz"  && echo "02b8c67f01479983152192070a10d4b669597d506849684e48c32d9b4b66ffde  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:0d94e7de59b4b27051eda77847a3e1fc846797f408beefa97271f541420516c3`  
		Last Modified: Wed, 23 Dec 2020 20:22:43 GMT  
		Size: 62.4 MB (62391497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92833f5796ed72fcb599787b27e5758e69fb5fba474a57eff8f180868e6ac4f`  
		Last Modified: Wed, 23 Dec 2020 20:23:07 GMT  
		Size: 386.9 MB (386864897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
