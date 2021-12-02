## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:16465b247260dd81fec3c56af306f80f1cddf0308b582361302eda6196313b70
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `debian:oldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:fa0fc44f6769657f062a211c90fd2aff6a84f7ea709d7597ade8a8466f1cbbd2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50437374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:689dd8a8c0190098bb69db46a4410ed7f7072026d4b728dbeb3629aa58282f69`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:49:13 GMT
ADD file:727d381013020657d0ea06936e18db69c00d3d7918cc16c77d2cfb6a9ad026ed in / 
# Thu, 02 Dec 2021 02:49:14 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 02:49:18 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c3c495d499fdeac64577c90a02b6f56ffe3bb292a5933eccdecc356592911990`  
		Last Modified: Thu, 02 Dec 2021 02:55:29 GMT  
		Size: 50.4 MB (50437148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716506d5d2e79f47423db32049a2aba0305f4f3efb45ede74c082fe2c3d287ce`  
		Last Modified: Thu, 02 Dec 2021 02:55:38 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:f5bb61ddcaa8f202c63d805c7c2ec0053a8f4e9fdb128b0caa4f31337a419aa1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48154481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e99ec2c79c2a252dd1858213bb53b1b24b76566186fa3ec50e2ec003cf50d20`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:53:27 GMT
ADD file:d8c62c2c6db6ac7253c8966bbab4a452f351083da48bce4e8a7e023d05cb4868 in / 
# Thu, 02 Dec 2021 02:53:28 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 02:53:46 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9443aed163ada1996b6a4926db892bae972cb41a90eb43fc1aa3e41e548cc6ef`  
		Last Modified: Thu, 02 Dec 2021 03:12:26 GMT  
		Size: 48.2 MB (48154253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039682d56034b43852b6943aa2a09ebc6593128a0a4fb1683cbb8970b46bf437`  
		Last Modified: Thu, 02 Dec 2021 03:12:39 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:d8eab25cdec6ee0208542e2cd49d649065538a83ba8f49f840a83d1f8042b4e6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45918333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:727832e9bf3b5d7eafbef22872f4e50bebfd9b313e444d675f9c682eba7ae018`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:02:12 GMT
ADD file:23851ef44d699801f834722aa6530215ac3a6dcd500c76d1bdcded99688a68d8 in / 
# Wed, 17 Nov 2021 02:02:13 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:02:25 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b959e8636c3fbc4fbcb87bab1fd1c0342f5c73abfb922f435e0607f1c1937f03`  
		Last Modified: Wed, 17 Nov 2021 02:18:34 GMT  
		Size: 45.9 MB (45918108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32fad563492aadc2b788336a7156f6a35255f2134e6511e46b18aa2e72f3edd`  
		Last Modified: Wed, 17 Nov 2021 02:18:46 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:61f740b7821dd406e23e93d0a8feb12f2ece0589ba5b792fe26a25950ecaaac9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49223228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:784da462fd513a639ea87ed9f4f94362ab272c1d2a6c5a53641dda3672380cc3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:41:20 GMT
ADD file:0bf72871c9dc02db2e698d59b049f2c2e2006efd248ac786ac9aea42bcd22fc9 in / 
# Wed, 17 Nov 2021 02:41:21 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:41:27 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2926301144acff341799afd8cde6828df5c64ca6be41a692ce22a8eeababdfaa`  
		Last Modified: Wed, 17 Nov 2021 02:49:11 GMT  
		Size: 49.2 MB (49223004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24cf6ea5a67f105ab3701247bd2d44a1b8cbb48f1108d960c64e7d2e838ba386`  
		Last Modified: Wed, 17 Nov 2021 02:49:22 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:a354c1cf38d2aea5506af93c882c00fd5c75ba648bd971a02bc37525d37f98c2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51207920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9aa6c3913b62d21f5f9bb3881836fce20e3cccd99e3cc2b652c14d12d9d49c7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:41:05 GMT
ADD file:6b57ce5fa1d11564a26e5ab54847764d46fe0883cfac29e2307148381922aeda in / 
# Thu, 02 Dec 2021 02:41:06 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 02:41:12 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3183e716e1ddb8ec3eed0a1203242019e72c30039c8a85751a3cc0b7d4904eb9`  
		Last Modified: Thu, 02 Dec 2021 02:50:17 GMT  
		Size: 51.2 MB (51207693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81bed7be1fce687f992c3b7979323d56e76a6767c4e0cb13560396b3c19608e`  
		Last Modified: Thu, 02 Dec 2021 02:50:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:75be13bd9520041c3eaec40e3f572a3f4769e471f85de9fa6ca58541fc658263
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49079728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:239ac22140d20d190e15da35e966cbf4de02e4b5f32a553a4edcc89a822f9a6b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 03:10:30 GMT
ADD file:051ec5dbe3f56d986bb36a6fe098d9d6151ddb551084397500a4a4dca3251734 in / 
# Thu, 02 Dec 2021 03:10:31 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:10:39 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:40aa185b5b46f05f565b33bb29719a5397bd901481c4197dc2bf0dad30b6e898`  
		Last Modified: Thu, 02 Dec 2021 03:20:06 GMT  
		Size: 49.1 MB (49079501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ba36d7997ef6c5662337196087ce175f37fce8b8bf0ba45fdeb2dec8f84961`  
		Last Modified: Thu, 02 Dec 2021 03:20:16 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:ded4dfd1da929e17b696a0ce766e6dbff701c93e9cde5ec20ceef8492562f4d3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54184003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abf55232a6aba6d7750abbb9a677598ee413f4ab0eef90ced53e44c88355acb0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 03:30:53 GMT
ADD file:fb62616778cd378dd7e27257d6690a397d27b22aa7afa78026f5f0edb0c26087 in / 
# Wed, 17 Nov 2021 03:31:14 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:31:47 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4c0a5998b10e435c4caf5a1b3d6f33eb49ac12985b9e77464ccad3513447823c`  
		Last Modified: Wed, 17 Nov 2021 04:00:40 GMT  
		Size: 54.2 MB (54183775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70cc44c649c5811ae3d8fbf91f8ceb4e7225829d136a0ea9efd368b0630a8ae8`  
		Last Modified: Wed, 17 Nov 2021 04:00:54 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; s390x

```console
$ docker pull debian@sha256:22e6acb44277f5fc96883b016d438c149412434c4c8d4de2a961a7b5d138574d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49005646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8090595779a06c91b5c5ed0c0302404e3d40f696fa65d1f14c03051480e4cfc0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:43:11 GMT
ADD file:8093c4a2da0918a23f3506c7248de0407ee728c18fa9f43d6e6bcc4c1bd13691 in / 
# Wed, 17 Nov 2021 02:43:14 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:43:21 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0fec2256c1fde808b8caa285d6c8df9138e9318b933d893a2ed591acdb766c02`  
		Last Modified: Wed, 17 Nov 2021 02:49:20 GMT  
		Size: 49.0 MB (49005421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b6eb6b9bed02316d5347909404146eab77a4b65294d5f790fac5b85392c653`  
		Last Modified: Wed, 17 Nov 2021 02:49:27 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
