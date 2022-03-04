## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:c1ee9fc091e36d67cbe79f8acc9c56c133d8a8f0fcfdd327b2ccdab85bd088b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:c2f6a88e3f9cb6221b13a2d961456a081975b936580387b6933cfff6e664af9a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **485.4 MB (485371765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8932d75666cadda98036af5cd135cad7a648d26fc9b62458558ca3b2a56a435`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Feb 2022 23:40:28 GMT
ADD file:871c80292a1347a65a30c9d2cd343d927528a61b8d89fd82f268d5f8ad4d2944 in / 
# Fri, 04 Feb 2022 23:40:29 GMT
CMD ["/bin/bash"]
# Fri, 04 Feb 2022 23:40:56 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-86059ff059c15219c13900625367028ea52b1d95d6f6515947fe04983baf9add.tar.gz"  && echo "7cbab49134e393024873c4c8ad4937d84c8b7ed316b4d6260ae6b425cdd89e91  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:f964900200fc1f8473ac70d9da14cde8bae251ffb4a8f4792e2bf9baf6aaac70`  
		Last Modified: Thu, 27 Jan 2022 23:12:55 GMT  
		Size: 62.2 MB (62237845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df40d5f106fd4ab71023a3b15de586ad3165bbec356559856b77c24ad4d33883`  
		Last Modified: Fri, 04 Feb 2022 23:42:04 GMT  
		Size: 423.1 MB (423133920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:2896d84d7d4d35a3b2107ee151860013ff99c1b84fe61ee1dc6200724c51e84e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **486.9 MB (486930828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dc9dae5a26f2292aff8c56adebc728b2a363264201f58e30e964116af4c4832`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Mar 2022 02:54:31 GMT
ADD file:d8fe7ad66f762a8aad81401877fc5d61f1a4b58eac91f47145e6e443aa3ac8ee in / 
# Fri, 04 Mar 2022 02:54:32 GMT
CMD ["/bin/bash"]
# Fri, 04 Mar 2022 02:54:54 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-743baa7c60c3c54741d5e55ae3430a659604633fb03e9616435ba83760e96755.tar.gz"  && echo "a2d893e0aae7d4bbe63bc587b4df87ae9ba7f2de8a15de13e766f74031044843  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:12990ee66856745f12f3a508d82e3d48a09d0378d91aaca8ca153c3819e7a686`  
		Last Modified: Thu, 03 Mar 2022 02:21:31 GMT  
		Size: 63.8 MB (63816961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e88df431ce701ae5994531d21801baa8d60ebb952c1675cee8006761b12e1bb3`  
		Last Modified: Fri, 04 Mar 2022 02:56:21 GMT  
		Size: 423.1 MB (423113867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
