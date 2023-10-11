## `debian:buster-backports`

```console
$ docker pull debian@sha256:62dfdca4e456aa1daa3c83f4e621a36e11822b780cb2b93eb24000dd45e3b1c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:buster-backports` - linux; amd64

```console
$ docker pull debian@sha256:7d6cf6e80308f63202661624403f00c90695749b655ba921e65ef03114a57e16
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50498386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb828d06d58c2e0155b6cd92611a4240d51c3930e0b6dd1c661ca87f8a22f4e4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 04:56:13 GMT
ADD file:5a868c8105f7b621ffe46e19453d846faef824601a70979f6ef2bb46076151b5 in / 
# Wed, 20 Sep 2023 04:56:13 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 04:56:18 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0dfc3f78750b97e03b66f316b37e155e3de173a8ac79942f0511888531fbe5ac`  
		Last Modified: Wed, 20 Sep 2023 05:01:23 GMT  
		Size: 50.5 MB (50498165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722eb998e07f3fb72145a706b643aade819dc34b9e7b98e37b4eb6554def739b`  
		Last Modified: Wed, 20 Sep 2023 05:01:35 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:ece761e4b3a61126a8c7bab94f5b3298cccbc96a8f2c1c2fc0552568d819560e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (45966576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46d6ecd9faeb11c3ac91544267acf48e4e03c813a6c78c36981096febee2631a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:37 GMT
ADD file:90492dd68d097af40a6208353165e1b7e2bc04a31cd2270232e085416f6e940e in / 
# Wed, 11 Oct 2023 17:42:38 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:42:41 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2ecd2705b9dde659b853da74fbe8d7227d02acd96f1d34766d44193b82468b37`  
		Last Modified: Wed, 11 Oct 2023 17:47:27 GMT  
		Size: 46.0 MB (45966353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c7277fd2e2c97e576f9c891f54b79826e08a712630034fa8d7814866b73d07`  
		Last Modified: Wed, 11 Oct 2023 17:47:42 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:40564b071a06cf92cfc75676968cccb93712c96637129df5ac69cc72e9801ce2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49291109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea13722262708c2a01ecbb48806d3c93d50475bbadf90ac8d7274bddf92cfb68`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:34 GMT
ADD file:3ec160f0e210563bfac108f23e5034dda5bc7b513b824ee276e4fc6daf80c89e in / 
# Wed, 20 Sep 2023 02:44:35 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 02:44:38 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:acd8b5ac4bd39653c2ebe6bd243f4ad2ee504ec9f8feeda9ef727446baf30721`  
		Last Modified: Wed, 20 Sep 2023 02:48:30 GMT  
		Size: 49.3 MB (49290887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca7b9c16ebea7f5028919e69d1d425c3882d50736daba1bfc0ae33fca3242d7`  
		Last Modified: Wed, 20 Sep 2023 02:48:41 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; 386

```console
$ docker pull debian@sha256:e427385be52fbcd45a1ec54cf7c504a08ce12ff411d8dd24817a2fd1d04feb26
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.3 MB (51256296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21bb61c0041b6e5420ffd7d27640fc6bc4c4cd2ca6e3b91b9f127a0897b6483c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:41:14 GMT
ADD file:47cece2eff96bf7383dd2a9c5632f0ad7bb31b3a459677530f77a78e22658e98 in / 
# Wed, 11 Oct 2023 17:41:14 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:41:18 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:62bc68699d611f4c048328a0468ebc10de528260c7823c8938796da30db31a17`  
		Last Modified: Wed, 11 Oct 2023 17:46:45 GMT  
		Size: 51.3 MB (51256071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f86b1e43f0734ffa16e319109f07e32b13b868c1bff5f71a082c31c12d925a2`  
		Last Modified: Wed, 11 Oct 2023 17:47:00 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
