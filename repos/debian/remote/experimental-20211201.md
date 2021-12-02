## `debian:experimental-20211201`

```console
$ docker pull debian@sha256:343852fc97641bccada562285da76ca6f6b17a1d8a293e0d0f6dcfdb9618cd2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; 386
	-	linux; mips64le
	-	linux; riscv64

### `debian:experimental-20211201` - linux; amd64

```console
$ docker pull debian@sha256:44f9f038fe3e2e94793096b020e9d53c02420409f4022c683ec09ff9ce0e53c7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.7 MB (55747104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04cfd8921f5e7ea5351d50f6f44d58fe5e6c8ea90c677c77269efbd3d746f03a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:51:05 GMT
ADD file:8ea96c53533f2bfc7d6a15c4d156b56c6ad3a2d3993e1a2b50e15b31bfe2be46 in / 
# Thu, 02 Dec 2021 02:51:06 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 02:51:17 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:1793db1a9beb666044badf0630ef3582bbc734ee46316e7d7789cee2ba37ef67`  
		Last Modified: Thu, 02 Dec 2021 02:58:39 GMT  
		Size: 55.7 MB (55746882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a1368fecb24e7c8120fd6ab0a53db8f59e2e277753fea194e6aa734b99af705`  
		Last Modified: Thu, 02 Dec 2021 02:59:03 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20211201` - linux; arm variant v5

```console
$ docker pull debian@sha256:1a82af1a26c8e3142df6648910031aaa68fb2a3a5d0b02327ee7311a4c0d11e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53226509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90a96927b6680bc45d1b50897b3cc2f1c147e3c49e708237e683265aa9c93089`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 03:00:04 GMT
ADD file:bdb1bf58320a788a3b3115425f34ebf3385ed3fd166fd9f62516fd4f80512490 in / 
# Thu, 02 Dec 2021 03:00:06 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:00:55 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:2d1699f433119b57c3eceaf5d93c93e7ca4a79b6d9bd74ae5d8a94e414aa9e12`  
		Last Modified: Thu, 02 Dec 2021 03:17:44 GMT  
		Size: 53.2 MB (53226285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7b6603ce38ad48f444a48ff36047cc522b88cd118358bc2f38fdf976da5f23`  
		Last Modified: Thu, 02 Dec 2021 03:18:21 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20211201` - linux; 386

```console
$ docker pull debian@sha256:4d07f9ec76fdca2d647f9df432aa2fbfb2c3aa033372e48c42c2e6bdda062824
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.8 MB (56808254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4892c67694c71e13d26f7313ae50bf308a98242dc42f60f9ca1e1cce53cb2289`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:43:27 GMT
ADD file:c8d17c45bc65348040374c6e7d5196c1d847ebed15871400c4da3df704515be6 in / 
# Thu, 02 Dec 2021 02:43:27 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 02:43:43 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:a2779241dd313cf1f06fa859a8361159673690c680955e423984567eed669647`  
		Last Modified: Thu, 02 Dec 2021 02:54:28 GMT  
		Size: 56.8 MB (56808033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e263303a85c0d1de1a995bdb27e635bac1218c59d17e945f3fd9b5fe56e9b94`  
		Last Modified: Thu, 02 Dec 2021 02:54:56 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20211201` - linux; mips64le

```console
$ docker pull debian@sha256:22f36216c2ce0fc07cd3d0d14c933947d4ab98bb6db4f034739cfbad1bfcd293
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.5 MB (54455677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6f041258d541a5cd019ee60de00dd8dd7d76be95d6cd5dcfe04c327eda8a2cf`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 03:14:01 GMT
ADD file:2d61dbbf49a978c5b903ad6810df99f11bcc9585d06f3fc5eeaa97beb27d6742 in / 
# Thu, 02 Dec 2021 03:14:02 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:14:29 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:7e0c1253ea9ee2c36fcc159313f9d8af0a88857a9aba47ea44e0fdee2bcc4881`  
		Last Modified: Thu, 02 Dec 2021 03:52:36 GMT  
		Size: 54.5 MB (54455453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0f42e520aefdff8b68f6604c0e9776716ee6d87ede5acb91bbf48ecbba5e07`  
		Last Modified: Thu, 02 Dec 2021 03:53:16 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20211201` - linux; riscv64

```console
$ docker pull debian@sha256:efe1ae8eaee5a194a51bd2ba5fb1ec2322c19836a1bd7ecc2de349b316814882
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51509504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0efc905b0f3905b3e9d6ed142793c4295ac6aef4892a5fa16fe25aa311915976`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 03:19:59 GMT
ADD file:a323413cfbbb9d9c5d8922ab6a65704b34c4b5057fd08cd09ec03166656c6500 in / 
# Thu, 02 Dec 2021 03:20:02 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:23:10 GMT
RUN echo 'deb http://deb.debian.org/debian-ports experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:cd756f7feb59c540dfa3f77898eb4c318cd0e47cd0f90c29ac1dba47238a0322`  
		Last Modified: Thu, 02 Dec 2021 03:36:06 GMT  
		Size: 51.5 MB (51509275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f36b1fc37c32aca05d3d10d71276780689dab5ce163e9a99474a2dd1a4f76f`  
		Last Modified: Thu, 02 Dec 2021 03:38:43 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
