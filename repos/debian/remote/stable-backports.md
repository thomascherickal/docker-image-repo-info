## `debian:stable-backports`

```console
$ docker pull debian@sha256:da894fec1dbf9ecc6d80841a5599bac71d3129be99b2d1f261cc24c1769ee675
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
$ docker pull debian@sha256:c389fee01796258fab912fd288f878ae3b220c31239c0414ecf496c40bf52d71
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50397916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a6168a3520ede88c680a71fb471219fc95786c9db52fe4fa74c31af8cf1ac65`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:08:12 GMT
ADD file:45f42bdb6a1e7c35d2c99036b0719848ec9d30bef2ebf69dd5b91562f11b3331 in / 
# Fri, 11 Dec 2020 02:08:13 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:08:18 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5e0d4a82136cf43df758ea4260c3aba2203db5ed27b727940a7e2b7cfd6af580`  
		Last Modified: Fri, 11 Dec 2020 02:14:49 GMT  
		Size: 50.4 MB (50397693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ac736715f259573e375c49061aaf7828c33b525bfff4419f554e360e8b390a`  
		Last Modified: Fri, 11 Dec 2020 02:14:55 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:04a953b46781bffb0274e2d9910a1cd3fc103aef34b4bdde4e6b427cdab41ba6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48111150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc30fc6fc2cbd47c0ad1d5230a3296ee71cc4a11b5f35fe4c6084f7f0c6a4cca`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:08:30 GMT
ADD file:55ab5bc0f69499e5ea48662377442d05a681c74d1afe2b7b1ab4f43af7953655 in / 
# Fri, 11 Dec 2020 02:08:37 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:08:48 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3b640bbe81831905fd7cd3efb0d7d912e036d2d8f4a47360d88b6d7d9a3428a7`  
		Last Modified: Fri, 11 Dec 2020 02:17:53 GMT  
		Size: 48.1 MB (48110926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f3a234d443dbbf95a0751c7a00ddbc573b91bb58bbab33e6fee1922869b3116`  
		Last Modified: Fri, 11 Dec 2020 02:18:01 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:c694c2c630687ba7dd3ae5abbaf84bbd3c46950196dd193e582a395c22959f55
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45868166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39992b52bccf2854b921fbf00e726566b7a10b79327b17d76b41900c38005bae`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:27:16 GMT
ADD file:b5289fc173c783ba03269df9db0e7578d0d5bccd63ae41ee527742214485bc13 in / 
# Fri, 11 Dec 2020 02:27:19 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:27:30 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b3af222b9997a5c9f80ea584b6a5d47ede720d1b24b3b05ebf815f1786bb5757`  
		Last Modified: Fri, 11 Dec 2020 02:36:10 GMT  
		Size: 45.9 MB (45867940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be06304a51c009d9e29a6c4cf002dd9fcb52f5c980452dbdd1b96c992326847`  
		Last Modified: Fri, 11 Dec 2020 02:36:18 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:d86df5929b5b86128cb1b9352ea8d39b2fa6ceee58e536f1517b599cd29b873f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49180498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6257614efe64f09f973f954a8f859bacb7f74f869f22d15262603a638d9ee75`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:47:27 GMT
ADD file:4a2d9c4db09c17e1a290d0cf1788f23c41a53b5597f9d43ce6813bf9b4ed4d73 in / 
# Fri, 11 Dec 2020 02:47:33 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:47:42 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:282dd64cc7ba9325ae813d4abff9643894126b68d42804927ceef9f83e640e89`  
		Last Modified: Fri, 11 Dec 2020 02:54:54 GMT  
		Size: 49.2 MB (49180273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2584a2a1048127454c6636a853fec4528c57f2c9d3bf6894c9913729f3db3ce`  
		Last Modified: Fri, 11 Dec 2020 02:55:03 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:fb62590f23279f2cf5aa46a27c7407ae30f32089213a91d52e4ac5580c792db5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51161425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c8588908cabf31a54df28f36cd2fbe24e373c43b84d30d0df938610d435920c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:05:08 GMT
ADD file:627b6b992ded46c543d2ebb88c35e7eeef6380eb735f66b7d6bed1a06ee1db3f in / 
# Fri, 11 Dec 2020 02:05:09 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:05:14 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:53a43a75123df6cfb2cf36aa13e59fd9c1b6946f536f875b0002947f25aff946`  
		Last Modified: Fri, 11 Dec 2020 02:12:47 GMT  
		Size: 51.2 MB (51161202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89bdaf432c2671a1aeb079b828694ad74dd68b267ed711a483c880f0e47541f`  
		Last Modified: Fri, 11 Dec 2020 02:12:53 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:a3608e0f9b31bbe89d31133fd4105b46bd148d94b9071aa73661de1e65a42a42
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49022819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9d68f3dc3636966f11a9b026a5b22c344f96df47fd54942a8b02e6a5138c221`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:38 GMT
ADD file:aed8f53e57fbd49d05b28154d4973621e5dec28eb9a084dd5d87df879deca96b in / 
# Fri, 11 Dec 2020 02:04:39 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:04:46 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e10b6267b593dd71c8007099359a7a115b3120e34f5e80e55282f361f252cccb`  
		Last Modified: Fri, 11 Dec 2020 02:12:19 GMT  
		Size: 49.0 MB (49022594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1991be1b840df49c513058cb44c0c2463b2ef05541d57562b6f4a80457375991`  
		Last Modified: Fri, 11 Dec 2020 02:12:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:292e3478b70d14c6e30c8584e599282e36db7ddd2da9637bc67ed1e305af7bde
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.1 MB (54143286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7b5993cfe249dc8e159b65dcec35e26f878316329ac89d49c8a29fe77aa1cc1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 23:24:20 GMT
ADD file:eb4c7def901bc2986e679334ee173b97affd3d52d7490e333efcad3803423f54 in / 
# Tue, 17 Nov 2020 23:24:30 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 23:24:43 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f36467046d39e664c9f24108fe797b190b581fcd74fb7341ad681da46c89232d`  
		Last Modified: Tue, 17 Nov 2020 23:36:22 GMT  
		Size: 54.1 MB (54143060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcbe1cacaf3f3917b5a2d38b946d9db6464df25ac744ac4363994b32861a943`  
		Last Modified: Tue, 17 Nov 2020 23:36:34 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:1cb609df080be6b9faab38c426e2730240a9a13d215c56cb3c48b182f1cb372c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48968491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75b37b8f4db2719e88a022578ed624d10115980b817bcf3b22727cd4a741f7bc`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:13:06 GMT
ADD file:ebed0976d063c02a4dba90a53f88053333166b9f9a4c8664ac5529427c9e7e17 in / 
# Fri, 11 Dec 2020 02:13:13 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:13:20 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2da58dc26121aabb68aaacf217eb730208aec75aaa194a943819ba7067f6a129`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 49.0 MB (48968265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca62c566284bbf7e0bdefa95994c95dac9f566645eb8897566ba90457db24f7`  
		Last Modified: Fri, 11 Dec 2020 02:18:06 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
