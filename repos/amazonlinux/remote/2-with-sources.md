## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:4b6e67a53d53b77ab9d0ab7b4904c6e0fd00000f0143e8e42cbf14f247609cc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:3567d9d9eeeeac94ddbd2c08b4ebe9c003a415d4adfb30a4c982f3418d425a36
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **485.4 MB (485353196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e954a7af0320b059d91c2fa85155e202c6b2267be94efa101212fa30328abf78`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Mar 2022 04:17:58 GMT
ADD file:6e25b6e9b3976f8d699ddf69117d5af30565798c52f777c8b4b99e38aca8523f in / 
# Fri, 04 Mar 2022 04:17:59 GMT
CMD ["/bin/bash"]
# Fri, 04 Mar 2022 04:18:26 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-743baa7c60c3c54741d5e55ae3430a659604633fb03e9616435ba83760e96755.tar.gz"  && echo "a2d893e0aae7d4bbe63bc587b4df87ae9ba7f2de8a15de13e766f74031044843  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:bda57ff2d0d885374555b8bf3f1aaa48d5f044446a24a98acedbef6acc0b727e`  
		Last Modified: Thu, 03 Mar 2022 02:21:35 GMT  
		Size: 62.2 MB (62239296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acfc84eae14a8f5517f777f3df3cc60ac8cf33a648d677bc33fab552696f8869`  
		Last Modified: Fri, 04 Mar 2022 04:19:56 GMT  
		Size: 423.1 MB (423113900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2-with-sources` - linux; arm64 variant v8

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
