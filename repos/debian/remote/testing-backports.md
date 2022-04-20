## `debian:testing-backports`

```console
$ docker pull debian@sha256:227d08ffcde90da47ea78116ebe2e2eafb25d7f1f20f52e9e7f8dd18f9898844
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

### `debian:testing-backports` - linux; amd64

```console
$ docker pull debian@sha256:f637f11a2ff4380f65f935775cc7c41e96a32cbdb675e15635cbe101104d5da9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.6 MB (55579088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3480a9f7a4bca34b5b6cd26603deb0bea01bc2791686f7bca25b936c77208dfe`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:45:35 GMT
ADD file:fb66d619557384a14385fa7b5371be954594c4aff1700edcbd9cff422c3498f0 in / 
# Wed, 20 Apr 2022 04:45:35 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 04:45:38 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:536039adbcd59ca1bf50e1393d4c116319d1f29168898c56d21c192d219c4832`  
		Last Modified: Wed, 20 Apr 2022 04:52:49 GMT  
		Size: 55.6 MB (55578869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2954f5cd8207b7dac4a769e9a5d2bd826aef31f018a912501ee32b6244b1aca7`  
		Last Modified: Wed, 20 Apr 2022 04:53:00 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:c7eba5c344db35398a31101df7ae4187ab10ea6d6b2c09c6e10d68a7dc84c648
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (53001342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:614cb3e15d39d2e228804b8cb67076650eae5d36da74daa08bf5d352a4c9c24e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:23:11 GMT
ADD file:1a78dbadec303b303272bf60526069e90e5b10883a8d0400749940066e1366ca in / 
# Wed, 20 Apr 2022 07:23:12 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:23:25 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0966e12cf6b5ce5f837d6a4be5f22fc3bf1a9f73f8f399eda6ba93087d2fab69`  
		Last Modified: Wed, 20 Apr 2022 07:41:08 GMT  
		Size: 53.0 MB (53001119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5719d2b8c2420a309123ce8c0999b249c9740db341e9540ecda4eb80245d33`  
		Last Modified: Wed, 20 Apr 2022 07:41:20 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:aa3101b785d5c5ac5d9d0ec46c628f5b5e1eca7ea8a72396311971c5423fbbb4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50609932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d357eba0f4ad2900cf46f2e64c4229430c0e77d6471da51e71b47b61894290d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 02:25:01 GMT
ADD file:b3e85f1474d193b977ab578a548dec606711cbc5b6570c8c0905fcc4b9252882 in / 
# Tue, 29 Mar 2022 02:25:02 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 02:25:16 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:87d7eb8842f0400851261593da9adb00f4ecfb155e1396dfcba71f1890de3293`  
		Last Modified: Tue, 29 Mar 2022 02:41:58 GMT  
		Size: 50.6 MB (50609707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ccf580b46bc760c2daa8df9382aa5a32ce6132e8bb10b62c9cf75a7f4cfdd8`  
		Last Modified: Tue, 29 Mar 2022 02:42:10 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:5268989e7331d9b0996eccbb735bbd8e604f70430511f83f31eec32ae4591e07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.5 MB (54493560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:489d522af0e00f742c3ffaddc107729942676665752c2284b9d972f13579ecd3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:31:45 GMT
ADD file:273f985806cb79b6f6b619ba5b9db50ba151174fde33bffc81c25187b0999170 in / 
# Wed, 20 Apr 2022 04:31:45 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 04:31:51 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3124af2dc12fec2edfce6b676869cb7dbcea85f39bf473efd3b5674765b68351`  
		Last Modified: Wed, 20 Apr 2022 04:40:29 GMT  
		Size: 54.5 MB (54493338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeec0554206fe7d868b12cfaff256babefc48ca0d621611263220d3124283725`  
		Last Modified: Wed, 20 Apr 2022 04:40:39 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:19cc5083c3fb725a1f6cbc932bcdfb2f7ee5ff47fdb057f11b1d4b7021ccc2cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.6 MB (56624736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8a8be1d997035a4f58ce782764809bc96c5a1e761223938dcdec1aa54b3550b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:40:25 GMT
ADD file:990bedbbc12a848e4ddb2e9645f1c6a5e7d1b282f26d2ce1112fa7f0765e84cc in / 
# Wed, 20 Apr 2022 07:40:26 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:40:31 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:25dd2dde37c9ed5b4c67bd973631862a34b0b2b837c36d134cc8116840ec0a1a`  
		Last Modified: Wed, 20 Apr 2022 07:49:40 GMT  
		Size: 56.6 MB (56624517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6eea383b106de4cac855efd53f667442c6201715451a60af96b9984df748957`  
		Last Modified: Wed, 20 Apr 2022 07:49:50 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; mips64le

```console
$ docker pull debian@sha256:a4b0dc4649f5a934e9c29eed98303f1d885376e2256cab6ebbea6650192fdb6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54240403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72e2109bea6f18f9ef024529c2d611bf31023588a94e0c0512e3525c3704735e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 07:47:32 GMT
ADD file:024d3880d7b57925a179be264896b146d4cfeac87003866bb0e336c33400106e in / 
# Tue, 29 Mar 2022 07:47:36 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 07:47:46 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:246ac5e155c140a71ba5195b835c78579b686fb0d9cbe2cf062e39583ddeac22`  
		Last Modified: Tue, 29 Mar 2022 07:58:46 GMT  
		Size: 54.2 MB (54240178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09255a198d562b80a7f219aab7d72c19e26b492ba0d9b5107b45640f913a4a8b`  
		Last Modified: Tue, 29 Mar 2022 07:58:55 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:f4e236df8ccde81037d5de775616442fdc2f5dd0dc9f4f9f6c49a294271f0c58
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.0 MB (59982778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ef5ebc4fa88dfcfaaad716dbb46e736918ff20a7692a6c425bce888aab766c7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 09:51:07 GMT
ADD file:0441cbd5b80c3154a95cf5f152472d9f238a42a1d874898b18c876944e830675 in / 
# Wed, 20 Apr 2022 09:51:19 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:51:37 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6a660090735cb86ef009831259b3363aa899b4b1f765ffad3047dd93f2146807`  
		Last Modified: Wed, 20 Apr 2022 10:01:09 GMT  
		Size: 60.0 MB (59982556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39fa69df81c97ac7a3ad7411e6e28a3fb92b13f378a5187e454931200bbf563a`  
		Last Modified: Wed, 20 Apr 2022 10:01:22 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:ada62ead09a70633c9247a230e237007fdbba4ec9a52d86a902951d2591801ba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.8 MB (53813739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f683e1c642a85d7f8feac85a7ecacaed5666269318809e4bb5dc92fde13a2f86`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 08:44:07 GMT
ADD file:23684e7af9a096cf83a114c361e7879ed97ef5fbf7cb9607e40ffaf19dd0bed7 in / 
# Wed, 20 Apr 2022 08:44:14 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 08:44:23 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:362ce0a85fc3f682e0adac2df3a00133068c959c8dbf9d7872eb24b1b68f55a3`  
		Last Modified: Wed, 20 Apr 2022 08:52:12 GMT  
		Size: 53.8 MB (53813515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab3ab942c84a5ca094429e8c1fa42731e06a77aaed1d68117d52a60c8f16fcb`  
		Last Modified: Wed, 20 Apr 2022 08:52:20 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
