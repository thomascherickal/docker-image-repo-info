## `debian:stretch-backports`

```console
$ docker pull debian@sha256:ea465a735399c368c6057ebdd96638d1cde1569db0645dcceda5ede6bda58b7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:stretch-backports` - linux; amd64

```console
$ docker pull debian@sha256:59dc3d4c7da226400e3582074eda4f891d6f80ecf32725d77fa95f99163d59ba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45380171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78bf683f95c6724555ccbb81c142ba49410d859f61eb90b70e13e5a337a6989d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:43 GMT
ADD file:e52290391b221e1a4e52cf4e41ffe7e14f162475964fa01638e03b3ead673ba1 in / 
# Tue, 30 Mar 2021 21:50:43 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 21:50:48 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:00168f89dbe8f3c9985e536784c27517f6cc35ea56263469449a6b73e0bed595`  
		Last Modified: Tue, 30 Mar 2021 21:56:37 GMT  
		Size: 45.4 MB (45379949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db40fd101b99fd447384bfbc8831957c1ea533ee770209697119493bbd4ea3fd`  
		Last Modified: Tue, 30 Mar 2021 21:56:53 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:07acf1d202a9aaa06b878d5b0fc695a3d8511435b8b1d7062519b8e8cc5295a0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44092197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f7a37cd88947d1ed23371149099b7b9de1b9a2c1f5c67e9c404bbf02e6198e5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:53:43 GMT
ADD file:471d7a5419df3b812f9a1b0b14c1bfbc2b8fc88652b66cca395a28af61a77f4d in / 
# Tue, 30 Mar 2021 21:53:46 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 21:53:54 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a6404a8305ff6dab0e0a06c0c4291401369422bb5ba3e2b49d5447049a0928d7`  
		Last Modified: Tue, 30 Mar 2021 22:01:23 GMT  
		Size: 44.1 MB (44091975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4242cb260d788f32877089fd28e7c7c1f3967db625022f21433e2d3ebe534542`  
		Last Modified: Tue, 30 Mar 2021 22:01:35 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:74c0496fac8ae064ec4d8ed81a70fc1c20df4149f641c5ea207931d85d8b6076
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42120473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23d7387a09dd0bb0fd5533ed4252bd86668384028564188c2f0619d94b6244cf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 23:11:31 GMT
ADD file:65b5cf73b0b90f1f459a64d5706f2420deed7cdc5a9e13abacf5bcb05cc3138d in / 
# Tue, 30 Mar 2021 23:11:34 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:11:45 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:80ad3ae4821828f32ce9b3e0f76c3c8f157a7f111e64ffad3ba40287904dfc63`  
		Last Modified: Tue, 30 Mar 2021 23:18:47 GMT  
		Size: 42.1 MB (42120250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070394ffde4355037323dc3e79b746736847ac547f0f659b32b3c40dcfbb8362`  
		Last Modified: Tue, 30 Mar 2021 23:18:56 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:d010c996dec1d955f02accaffc55d899407c9780d6bc868d43c53b9f19d06430
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43177813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baaa7bf0309996fec82aa71cadc9e0dcc299a18b8161cc637e030848087f6234`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:45 GMT
ADD file:0546f28e5d1be54699d1e0756275203da731735b3212f2ff1a87cd7f8dcc9049 in / 
# Tue, 30 Mar 2021 21:49:50 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 21:49:59 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9317dc7ea567b49ade0ea730b5530d1363b065549e8b75a198e0b60bdde1f1d7`  
		Last Modified: Tue, 30 Mar 2021 21:56:46 GMT  
		Size: 43.2 MB (43177588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4e1be4e7accb60442161a621c450bf50e28949e020c17cb53f19f71e5a2671`  
		Last Modified: Tue, 30 Mar 2021 21:56:57 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; 386

```console
$ docker pull debian@sha256:99ffe68bdb9904b305c1701cc8943232ee26a2b27bf38cddade5152d01db3123
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.1 MB (46098778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:050673625fa71f914ba973cff97632067362602c7199058ac595c670120a47ef`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:41:30 GMT
ADD file:1df7a35a36c49061902cf634a894b34a55a9c020976547cf6d2dda96879854bc in / 
# Tue, 30 Mar 2021 21:41:30 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 21:41:38 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:667bc6614d317ea77075a4e2f4ee7ef7d7b696f50d426cec38048d3ca20f1aa1`  
		Last Modified: Tue, 30 Mar 2021 21:49:28 GMT  
		Size: 46.1 MB (46098556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee575e870034369bd3d26a091871a37d784401ea6ef67a346348218a4672a38`  
		Last Modified: Tue, 30 Mar 2021 21:49:51 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
