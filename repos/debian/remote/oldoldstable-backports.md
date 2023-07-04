## `debian:oldoldstable-backports`

```console
$ docker pull debian@sha256:8263cc248d16ce0c54805f7e080cefe8190316ffa382ce8913c5705674540c25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:oldoldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:2826d85a3a1461d057104dbed17a212d0b2e15f3e4f5d5f29f4ab67dbfe9b8ba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50448905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55f0334078bd9a3d3a5805fba265a93a02c60e9eca5b80c011a7a914ad205d01`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:59 GMT
ADD file:3b029f3178b5e1b4334c6406617e14df5bf0ce15ce935acc2cb2dc51b6f151aa in / 
# Tue, 04 Jul 2023 01:20:59 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 01:21:04 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6b44c60b4ef8f05f0a7be874cdf80559a40b3584e9146bcef80caf7c3bd47f55`  
		Last Modified: Tue, 04 Jul 2023 01:26:40 GMT  
		Size: 50.4 MB (50448681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78762e368694aac5183db60432839840fd36b2b774681232bda6ea38c0cc543`  
		Last Modified: Tue, 04 Jul 2023 01:26:48 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:27705c3287f2a99db1dd0812f2cf7f07c6f10f338559136db7bf2b984f1f747a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45916703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99c3a89bed79b89b80de79c9612e1da0c327516081357c9562157ecd5f960aab`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:51 GMT
ADD file:fb0d0efa496216eb4150798e9acf6220f344ec01a00121d2ac5eb8efb61344c5 in / 
# Tue, 04 Jul 2023 00:58:53 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 00:58:56 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:003d12612fcea91fa985efa292e97219fbb80e0975883488634bf9f8193e765b`  
		Last Modified: Tue, 04 Jul 2023 01:04:36 GMT  
		Size: 45.9 MB (45916479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da294ea69efbe031e32997ebca5cce08305ed429a659b96f9b5e05ac2dac2480`  
		Last Modified: Tue, 04 Jul 2023 01:04:45 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:92a6846b9f5dc4f8c39e012db9ccc6b6f0fd9e98fcb8421ad3e115c5868a302a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49238650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d9f32baf70ffc449e8f2195a0f3c38e00f1ceb962685497d34a0452badf836c`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:41:01 GMT
ADD file:e2942c977c101539f35f37f69e020802ef763ca33d8ef4ffd4bfca8f5cb496d0 in / 
# Mon, 12 Jun 2023 23:41:01 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:41:03 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:023125a50c120c98a11d445d8dc0121fa2823e4f053e7c98b2d61b97b9a2012d`  
		Last Modified: Mon, 12 Jun 2023 23:45:37 GMT  
		Size: 49.2 MB (49238427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5275cb97965ee9ad2241db6b71fc491c7754588916460fc848f53ac95197c3fd`  
		Last Modified: Mon, 12 Jun 2023 23:45:45 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:982a1dc77be9aabf0ead3de931492413d41282f4f57108027f8e36dba1caf723
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51206223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9774975734b7bfb1d346176bbd6cf912fed5d2405058fdc0d39beea2040c2d7c`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:54 GMT
ADD file:c1185fe141b862f97bde1607c0ac6b9f6243d5d7a763296a82c72466de9e9c28 in / 
# Mon, 12 Jun 2023 23:40:55 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:41:00 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:cb5c8a7aa1b433e8ef99af81a22f654ee247118cfc32f82f86af969632128bc5`  
		Last Modified: Mon, 12 Jun 2023 23:48:11 GMT  
		Size: 51.2 MB (51205998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90d68062b587693fa848f406f83c7e8a8501c7899b6e99518b6b6bcc8e6b38f`  
		Last Modified: Mon, 12 Jun 2023 23:48:19 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
