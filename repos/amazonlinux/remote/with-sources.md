## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:999665d9a2213ea2bf8093cd9cefcc6d7978438730e1a080c8682c801096757f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

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

### `amazonlinux:with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:eb66bea13e8eb8b6402f2396470190f5201029f1740f7571511d66fdd157dcdd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.0 MB (486950607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2615f7bdf3f4ddc681610c299da2d5c5c1dfb862ccb4e2f3c5ff0558c98ff73f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:36:59 GMT
ADD file:2b2d809ac07187a252399bb24721c7a295cf5fa71ef4e526ea56bb8d1bf77fd0 in / 
# Fri, 18 Mar 2022 00:37:00 GMT
CMD ["/bin/bash"]
# Fri, 18 Mar 2022 00:37:23 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-3c9668ec048dfa6db814960c8f21d657525398c311820322e74a0cd5c740a565.tar.gz"  && echo "28f895ddb81eab8d861e7f1adc7c54a47146dc14956644e699d4eb9ead29f515  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:16a64fa775cc87d32953ff0ed81775d6ea6b725a7946b4260298cc1ec4b5b32b`  
		Last Modified: Thu, 17 Mar 2022 02:22:32 GMT  
		Size: 63.8 MB (63828887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01cd7a9d9c15edb2f1e103b9fc3acb6251a5ee9d252dae649c8d9c61b88973b5`  
		Last Modified: Fri, 18 Mar 2022 00:39:16 GMT  
		Size: 423.1 MB (423121720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
