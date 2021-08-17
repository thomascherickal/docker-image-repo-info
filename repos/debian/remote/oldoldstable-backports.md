## `debian:oldoldstable-backports`

```console
$ docker pull debian@sha256:7ab09986504266aead39a7d0a2aad62abe9cb659fc152930d37b8fd580ecdc36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `debian:oldoldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:f17f1b96bac832ba793c20ae63622f6dd69ec430ab7d72e51b2baa25b57e34ab
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39339986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9630acf5b95b1d3c38f602f84d13565f6896c86d64db2fd8bd1e5fee3cfe0ff`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 04 Mar 2019 23:20:40 GMT
ADD file:d41de34f44b3dd6bc7a9b200b90f2ba9f46e207a09e8570249fed0d065c755a3 in / 
# Mon, 04 Mar 2019 23:20:40 GMT
CMD ["bash"]
# Mon, 04 Mar 2019 23:20:44 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b6a968a0691c47dc3c7b611b431cbf904377404615d57dc6495fea107ebd2a91`  
		Last Modified: Mon, 04 Mar 2019 23:24:49 GMT  
		Size: 39.3 MB (39339757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4618da449022f247ff61a4dc757021272c0c1935aae412faf2926d92201b5095`  
		Last Modified: Mon, 04 Mar 2019 23:24:52 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:3deca4346d0adf71bcd478a88754939c5dac494d82773f3edd752f9a3001a434
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (37992445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1834fc0ffff552efedcc907c222095a831067576098339a283cc70f089b98e6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Mar 2019 09:51:01 GMT
ADD file:e25e1071b4ceec7a66ec17228b9554de6480a84efd8347423f93298a2b815fd4 in / 
# Tue, 05 Mar 2019 09:51:02 GMT
CMD ["bash"]
# Tue, 05 Mar 2019 09:51:10 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f9d75622569e42bad4acffe99f3f89c7cba69821375e6bcd39e8a9f1df4ea903`  
		Last Modified: Tue, 05 Mar 2019 09:59:58 GMT  
		Size: 38.0 MB (37992215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc6b8c1ea5eed4ddff5e88a462bd69c2763b72c70fd7e03fa1d2f753d6e9e3c`  
		Last Modified: Tue, 05 Mar 2019 10:00:04 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:59057ed0ab64f48f4602059ca431d3ad9ebd369cffea5b54b79776bdac450dd7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.6 MB (36620191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af713ba3aec6f1645af0f3a129c4d1af4b83b851cbc58b6fd3df9e7422c56f2a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Mar 2019 13:06:27 GMT
ADD file:0caee109b4cdcee58b1f6d8abcd0cf00f38860b85cf7a8909615e37b6954b58f in / 
# Tue, 05 Mar 2019 13:06:28 GMT
CMD ["bash"]
# Tue, 05 Mar 2019 13:06:37 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:65fc7f64df1df19bf879ad0a100f67326a874355f02d8bc25769fdb3d7e7e2ee`  
		Last Modified: Tue, 05 Mar 2019 13:16:06 GMT  
		Size: 36.6 MB (36619961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb7b16994722c8b29fbc263967ed8cf48f4f625c7e2383ea2bc7c290b9ec6ff`  
		Last Modified: Tue, 05 Mar 2019 13:16:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:02934282f1bf5990e789f85d3399a7feca9e75538328dad0cb4fe80a071e1dea
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.5 MB (40533121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4de7bbe0ff3a19e8a2beba3624a37ed0e08ebc6b47bf3552863bea7e75e1a0d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Mar 2019 11:41:55 GMT
ADD file:4a0f80e3355f455ee17c582e67924e55068cb62a14a05a612d803de9657247be in / 
# Tue, 05 Mar 2019 11:41:55 GMT
CMD ["bash"]
# Tue, 05 Mar 2019 11:42:01 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4e9a483af00406f4fa56a07c819dafc6ad023c04c6879b60587ad968e3f02541`  
		Last Modified: Tue, 05 Mar 2019 11:51:56 GMT  
		Size: 40.5 MB (40532895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9416cfeff104e050253395d35cedc5080cb5730b59258a0f09bf610c51e46cf`  
		Last Modified: Tue, 05 Mar 2019 11:52:03 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
