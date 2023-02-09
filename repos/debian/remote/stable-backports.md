## `debian:stable-backports`

```console
$ docker pull debian@sha256:3ebb32d8cbc6fa4983316e2168ff4c0b23dab882a9217694e697ddb6940370cf
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

### `debian:stable-backports` - linux; amd64

```console
$ docker pull debian@sha256:9bd8176988def350c101b7fdac55ad3c98bb8765802b8cafcc3f6607402dbdd4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (55047041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07e16b4165ebf9c72df55ee9bfafc0c120937b4ea92270d95eda5b56dca95ce9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:21:55 GMT
ADD file:c025e3edb60576cc17e1d993eed97f6e915a365cdfc0128413fb22bf92cf0807 in / 
# Thu, 09 Feb 2023 03:21:56 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 03:21:59 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:03e73b441cda11b2a092f85ba0703d78d37de8028d778fe081cb0a2a0ab48727`  
		Last Modified: Thu, 09 Feb 2023 03:27:13 GMT  
		Size: 55.0 MB (55046818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e211077a1e1189b0b434f43abeeba36e71fd1b907e12054df9a580feea3bde4f`  
		Last Modified: Thu, 09 Feb 2023 03:27:22 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:6a834e02a1aa895e197df3bf087783a47d90b003244e034cc78629f67e66e7bc
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.6 MB (52552058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:233ed63fb97e65a267bc560946852c1207e1a13e1ddca74f258fbf805db56f55`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:01:09 GMT
ADD file:aadb8a3f3bb4d76da194ca1430801792db5486b4c6bb085361b661730817bdca in / 
# Thu, 09 Feb 2023 02:01:09 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 02:01:15 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5104b3c59ba30358f01df3920ae0670fa072d624e723c64d7d3110f14ec2258b`  
		Last Modified: Thu, 09 Feb 2023 02:06:43 GMT  
		Size: 52.6 MB (52551835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d99d99ccf74aed9d1b3c11b7b28d89f4a9229bb1172ccf1380f84e91a78476`  
		Last Modified: Thu, 09 Feb 2023 02:06:55 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:e0e4c2bfc08848d28fe7791ed58dd423c3fbddc78dcddf69e235355ff2eb4064
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50213949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8dd0486e8d030949cd48a41f2217625099d72ef50c48d4dd756ed0a3a15a2f2`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 06:14:01 GMT
ADD file:d88fff6b7cca831dd50f6d54e49d2462a85166255dbdf652da52394dbe246c58 in / 
# Thu, 09 Feb 2023 06:14:02 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:14:09 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8fb204581a907b3d3fa4ef35b6491e3cafd3fe2a82ab45b128a1bef9bb3c532d`  
		Last Modified: Thu, 09 Feb 2023 06:21:47 GMT  
		Size: 50.2 MB (50213727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8433b0eebd846c6fe4c3fe67ce7e13170a825fa8dc75748aded182692880e62c`  
		Last Modified: Thu, 09 Feb 2023 06:21:59 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:1d641cdb3ac06ea3edadf0cfd400e879b408ace1092f847fbd0857ece15d7126
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53703596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30e1cd9adcdcd90574febe6efb9e62e1dd71e24bf917e89ad56d1cdae742e0b3`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:59:44 GMT
ADD file:7d29ca4b03e85d823cdd9d56a3ba5587209931dfe2b8ad3ed19f87087e9362b7 in / 
# Thu, 09 Feb 2023 03:59:45 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 03:59:47 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:fabcc9af3275e9129273a4d9bf6432afde97d0533db2c98faf6dc821eda698c1`  
		Last Modified: Thu, 09 Feb 2023 04:04:29 GMT  
		Size: 53.7 MB (53703374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c65b9557dee2464b571d24821fd10ae5b1260ebc1795e95d799e9f933f9e287`  
		Last Modified: Thu, 09 Feb 2023 04:04:38 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:241217d45769242c12553be8ee71d3668fb75036cc331a5b3e994a2671eb192e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56030383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e40804bd209d227142ddb419cfe2e4a1cc4f50a6f93c84bc63fc94f34238bb29`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 05:14:22 GMT
ADD file:b76f9ab3265ff124ec1c3ef6f67d031318e4acccd978ed0414f092eb71a73442 in / 
# Thu, 09 Feb 2023 05:14:23 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 05:14:29 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7a0c879ddf3bdd4d3f7979495def00dc102714103384f2302d5cbbbba569b5ce`  
		Last Modified: Thu, 09 Feb 2023 05:21:02 GMT  
		Size: 56.0 MB (56030159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26df46c64dc7e1476053bdfc005ff5b877017126bdea473a7c5cd53b313c6df4`  
		Last Modified: Thu, 09 Feb 2023 05:21:12 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:3c5d1cedec5848f4f782946f03e01e5dafde1934455076a1e3418343fd460a74
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53267017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69e48b897957d72e97c84ca7719e7526a3f8ad742d96cedf087230f9bec42fd2`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:47:08 GMT
ADD file:39a6afae8c3eacac911f0dfb3bea652228471909c6f8ea7094123715128d81c3 in / 
# Thu, 09 Feb 2023 02:47:13 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 02:47:21 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b2ab1fb26b812ee53551d009c13311e13292f3f7e96ffa8b0b8641da27632c07`  
		Last Modified: Thu, 09 Feb 2023 02:55:42 GMT  
		Size: 53.3 MB (53266792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b3362f40ceb2d402f3533305481d5c8ae9bc82245ec719db06d058ff895c8a7`  
		Last Modified: Thu, 09 Feb 2023 02:55:51 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:c8c7ea24dc5761d913b727ea56555e82ddfe2e780b7010815618e601b279fe2a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58923673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5aff23af33421d26829d8fa11eb4cff290e4190ea18ba3a3842d42b2b54a74d7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 06:22:59 GMT
ADD file:8c1a1a4ed2fc4f1e5765130b29684dfa6ca8ccd3456ad76984a4560d2b862ae3 in / 
# Thu, 09 Feb 2023 06:23:02 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:23:11 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:04017f27164cf0d8cb15087dabab0e3b8a3003eed9b0e254970181616dc9ff71`  
		Last Modified: Thu, 09 Feb 2023 06:29:40 GMT  
		Size: 58.9 MB (58923451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988685e1c2d87957c70f52704b3ee2c41ce140d93e99feca9279e4785abe505e`  
		Last Modified: Thu, 09 Feb 2023 06:29:50 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:049e68bf86ae5120bade64ea065950d3c3fb41260c346c95eccc3df99c37f743
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53279128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c137493c6494a19ef7b0609c471a1f6f5761c0c75df49fb7316edbc212b2c79`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:42:21 GMT
ADD file:4057138fad7c5aecd192988c593dd7b997c8ade6e44621307639f5669b64cf3f in / 
# Thu, 09 Feb 2023 02:42:23 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 02:42:29 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c36299b95efe6adafeeca8401d4fe17de21c7947488846e43393351dd4e3c451`  
		Last Modified: Thu, 09 Feb 2023 02:46:46 GMT  
		Size: 53.3 MB (53278906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103511dc331478ea76f6238a7d8df7b3a487f3db791930cf0234df21a03bfbe3`  
		Last Modified: Thu, 09 Feb 2023 02:46:53 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
