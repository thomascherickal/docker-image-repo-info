## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:f66f05473f90aa6e14ac926ec03d61af16828a2ff9205fbfa1d3713670b0c166
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:9a3fbba8f30fbd72a0aa0116fd0ef46e8af25d260d01073c266347f116f20399
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **485.7 MB (485712608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6855b0eeeef206786c8c7ac97e546f8677b9d18b2fead70262d5cebc674f86d2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 May 2022 23:19:31 GMT
ADD file:386c34c6960464ef8f88891333fb091aef731602a28a185a9d6db27726fbe504 in / 
# Tue, 03 May 2022 23:19:32 GMT
CMD ["/bin/bash"]
# Tue, 03 May 2022 23:19:53 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-27e5885b1b2e681d27e9e8c451079b8f7f6444b820900db76e8e1f583d454a37.tar.gz"  && echo "fae8bd9cc002cf6ab3af9d777f1bc2646993e0340f2ffac4ddc984a5821a77c2  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:8de5b65bd171294b1e04e0df439f4ea11ce923b642eddf3b3d76d297bfd2670c`  
		Last Modified: Mon, 02 May 2022 22:06:03 GMT  
		Size: 62.3 MB (62291142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0efe039696303bb91bcd3177af472d1339e2e4cd62297fabd75e1763b9bcb9`  
		Last Modified: Tue, 03 May 2022 23:21:15 GMT  
		Size: 423.4 MB (423421466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:124eb9a22c4bd8d59ea311f776bae5213d1e66db6103732c2c10741bb263f459
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.3 MB (487323598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671abfcb4f4c6d925fbecf84883a36ca87a0e7e8aa40bc10b0c3a1678f2b1168`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 May 2022 22:39:32 GMT
ADD file:c351a8c80719ef38e02c26849f50bb7d79c24a6347cc2a72ae1a0768964bd113 in / 
# Tue, 03 May 2022 22:39:34 GMT
CMD ["/bin/bash"]
# Tue, 03 May 2022 22:39:57 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-27e5885b1b2e681d27e9e8c451079b8f7f6444b820900db76e8e1f583d454a37.tar.gz"  && echo "fae8bd9cc002cf6ab3af9d777f1bc2646993e0340f2ffac4ddc984a5821a77c2  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:ec3b4c26678b188d3874bed5e14dd278311fc05c81e418d5f0da36ec38d9f488`  
		Last Modified: Tue, 03 May 2022 03:07:52 GMT  
		Size: 63.9 MB (63902179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189fd58a2d5dc106fd8a0dee23c67eaa14f4c78c0e8fecb154e921df7a05540e`  
		Last Modified: Tue, 03 May 2022 22:41:23 GMT  
		Size: 423.4 MB (423421419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
