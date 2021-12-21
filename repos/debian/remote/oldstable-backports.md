## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:e71727b2086cd4a37fe417357ff9afc940c617baeabaa2df16f3584ed11cdf71
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
$ docker pull debian@sha256:8817f7e9169adcb1550c73d2a6b4964fbff6adafefa28debbecbaa6bdf144867
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50437367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cea87495549a449977780cf8d5554883ce35913905076150aa73c39d9b032901`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:33 GMT
ADD file:01d4d39be06fbf95ae81fff0a269566102be821560c2b09c91a1d7ad09c03d20 in / 
# Tue, 21 Dec 2021 01:23:34 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:23:37 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:77245358ecd9717f050393dfd48400a8fd0cb71a4527fae22c5b0229b02107f5`  
		Last Modified: Tue, 21 Dec 2021 01:29:29 GMT  
		Size: 50.4 MB (50437142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7abe1f9f8eb3d1536cf3d71c1bee0848ab65d4921371953529e282c8d0ed9b5`  
		Last Modified: Tue, 21 Dec 2021 01:29:39 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:adaf728b2bb83375529e1baaaea180a9345f2ed775ee259eb3e5076454972d85
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48154554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b47f338d5d6d55b5518d91bf56c62bb939ec4328f90b05c48f092c0ab408e3cc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:52:54 GMT
ADD file:1a710ea282cd5d0c3a4a9b8f78a2236a123395bab356c5a373ee20a7eb2520b0 in / 
# Tue, 21 Dec 2021 01:52:54 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:53:07 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f7d4ff054d0270c117d279bddbaff9d319a0c080451130e6a174edfb798faed4`  
		Last Modified: Tue, 21 Dec 2021 02:09:19 GMT  
		Size: 48.2 MB (48154329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:371a903f7a90359a8d769ac14ffd9ed2b8bf9f74ec3e423af84fb3f5d650483b`  
		Last Modified: Tue, 21 Dec 2021 02:09:30 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:ffd3aa9d8303eb40f67646ca91643b82d2ab9b239f07ce815ad06fac846bdfcd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45918373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1280ad4745d8fb8720aa1f1c266566efe211f252eaba1fe5136c4dcd058e3aff`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 09:07:48 GMT
ADD file:d689e3ffbe5a9093757a074e3d1acdb65c85272d0eb78c1aa2e3f06f1851ed3e in / 
# Thu, 02 Dec 2021 09:07:49 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 09:08:03 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:55d0d188b6cef9fa757431d5096d86fdeba0ed57204b92b46b8c5693ed803cf8`  
		Last Modified: Thu, 02 Dec 2021 09:24:17 GMT  
		Size: 45.9 MB (45918145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b6051864e1e88fa4659e2150c64e97542345331c5de08703736519651dd706`  
		Last Modified: Thu, 02 Dec 2021 09:24:29 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:5276b6a3fd2821d852037235114c9c68540791ef9205aae1f5a415f7a4695b4d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49223349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7fd50a47136fc62d18384558caa49e3e45cac6203622792c97016543ff0f560`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:43:21 GMT
ADD file:da55f63309c3e3eeaf9b6d9ab141fe3fea1750a44e59e739a5683fb985bd90fc in / 
# Tue, 21 Dec 2021 01:43:22 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:43:28 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:aed84f893300b9a43b86015ddd8e76ed296f1643ad906676e325a0b1169aa37f`  
		Last Modified: Tue, 21 Dec 2021 01:50:44 GMT  
		Size: 49.2 MB (49223123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8629043442ccc1e328225297f392a8e80332ceab99894e5288906a24dbb5d9a2`  
		Last Modified: Tue, 21 Dec 2021 01:50:54 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:55044506e23b45c1cdf7ef0a0287edd6fa344dd5979f6c5dffcc0a2ba017f043
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51208019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa00f0ebd9a7830235fcde073a628c264eb57bd7f41cc4ea80a72018ca45d35b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:41:32 GMT
ADD file:67c4844a5e7d215e401cb1a526e7d1849ef0215091cc28f1f932585a50711b2e in / 
# Tue, 21 Dec 2021 01:41:33 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:41:40 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:06055311534f5eb75b41b08fdde9cc4d677943a7aba8f14d611b02ed14a127ca`  
		Last Modified: Tue, 21 Dec 2021 01:51:00 GMT  
		Size: 51.2 MB (51207794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0cdb00242e44bb1226d001fb657ffbd513e650fd44a73095cc1736090b1a43`  
		Last Modified: Tue, 21 Dec 2021 01:51:14 GMT  
		Size: 225.0 B  
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
$ docker pull debian@sha256:25bbea59e568d57f820a1019a53af009435dc5f869aff6753f5037aff7a14cd6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54184024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fd601da654041d2569905fc3bce556389d948132c00615962ab226dbfb85c27`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 07:22:34 GMT
ADD file:5e7326e39d36f27614697f320d418f06a9752f32126bbb2340960d01470a974f in / 
# Thu, 02 Dec 2021 07:22:42 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 07:22:56 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:15873646b07eef157f2a4878c244f2cae2dbaffc11d4dee6f73d2eed62bb3e1c`  
		Last Modified: Thu, 02 Dec 2021 07:33:08 GMT  
		Size: 54.2 MB (54183798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497bb367449c5142ceb23a5e6c7f3c3fdc742e122bfc70833cb6288ccc8b0fd0`  
		Last Modified: Thu, 02 Dec 2021 07:33:20 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; s390x

```console
$ docker pull debian@sha256:366ebc9a46114249e29c2727c6d15ec3be4822db45843aa4ac0591828ed90a57
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49005678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:214f1025f83080afdb4f42af7d8204fdf62807cc086c0f1a983deb2eef874e07`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:43:09 GMT
ADD file:37e3ccece672e6c0ba669033fc5d6a331e6c60cb93bd1100e2a98a24a8cbd364 in / 
# Tue, 21 Dec 2021 01:43:11 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:43:18 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c479c9091d0265cf5a542e1317d5c169672f55acab6d6d1ddc52e016192e8a1d`  
		Last Modified: Tue, 21 Dec 2021 01:49:07 GMT  
		Size: 49.0 MB (49005452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac8cf4897c440fba4e9f046ce602e341c23bce7faf0dbcea9e70f109f029474a`  
		Last Modified: Tue, 21 Dec 2021 01:49:14 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
