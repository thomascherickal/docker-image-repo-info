## `debian:testing-backports`

```console
$ docker pull debian@sha256:d4aefa1dbf454246fcde5725c912b75d475c60a73ffcd81c475d2768be18e9e8
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
$ docker pull debian@sha256:4d4147b530dcf3f26aaffd138aae739f3f83e3542d15cc647ab2c7cdae18b932
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.6 MB (55584410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90ca4c51000a876c4a21a89b82896e92973e7e4d14cb71a79c97b7e7cee933c8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:24:23 GMT
ADD file:b3fad2e673a4919f337ff662b27c07fc41dde96654aa93847256db892f7d9351 in / 
# Tue, 29 Mar 2022 00:24:24 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 00:24:27 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:37b80729f30546cc683fa4e28f28931117dd7df20cfa896c3074703384422445`  
		Last Modified: Tue, 29 Mar 2022 00:31:28 GMT  
		Size: 55.6 MB (55584185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e380662a664204f05ac0e388e2a4a37c9653dfd83633145ae2e13438edfd454`  
		Last Modified: Tue, 29 Mar 2022 00:31:39 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:b56830ec5043808dae11812b9a750398e36531e667dbca2517a8f20945af6598
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (52995776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:744fa615c7b020d32eeec3e2724142fcd90fefdfe9c213eabf7c3737e0ad318c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:56:34 GMT
ADD file:573c96d320664803b8377e6766f4f21f97fb0788e2165a9d3b263a206b25345c in / 
# Tue, 29 Mar 2022 00:56:35 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 00:56:47 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f2337fc8f6268a3faf54e9f5bd6b46ef2cd2b21fbf508800caebd209c1476fd1`  
		Last Modified: Tue, 29 Mar 2022 01:13:43 GMT  
		Size: 53.0 MB (52995551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8971e4ec6d5852dcb06e57f456599c5d1e76373621df23f06f2b757d1c1f0e68`  
		Last Modified: Tue, 29 Mar 2022 01:13:55 GMT  
		Size: 225.0 B  
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
$ docker pull debian@sha256:64a11cc2f08bae7f54dcef1f9220b9c607330d74ae5b0bf5ab3206756a222b65
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.5 MB (54505369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:050cfa5722a46193eb737823809d8482d113f4b744cb5b0fb002458370842ab7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:45:47 GMT
ADD file:413dc9dcd9f5e11c82f1001a16db863d9dbff7b516feb23415728af53509d523 in / 
# Tue, 29 Mar 2022 00:45:48 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 00:45:54 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ece0f6f978dd4f51c115d185eb0228719b5d854a2b600a1177ee2ff807efb2a5`  
		Last Modified: Tue, 29 Mar 2022 00:54:45 GMT  
		Size: 54.5 MB (54505148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba6a6046b4fbb3b388c32399187bfc70d7e06a6afeb80930e01ae43459843e0`  
		Last Modified: Tue, 29 Mar 2022 00:54:55 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:9afd9fba556b08dd32a844057bb4ca66e25212b1ba31f546d50fb9635ce988c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.6 MB (56628521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84fbb6e94990b8d6eef45c43983b0cfa683c762a59c2443ab77ef86e9afa1aae`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:44:35 GMT
ADD file:04c7a3673259ec46457c82e0627de245152b1a5914d5f33f54a4124b2e4baefe in / 
# Tue, 29 Mar 2022 00:44:36 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 00:44:42 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:74cebc6ad2db83c170de3f5fcf9e261c4c2d9a5b7195ac97aadd71dbd0c36820`  
		Last Modified: Tue, 29 Mar 2022 00:54:04 GMT  
		Size: 56.6 MB (56628300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6d918c14cb1fb830b10f0d53e8ed11b2fceb90baaa0bb80ccf47fc0fa3106c`  
		Last Modified: Tue, 29 Mar 2022 00:54:15 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; mips64le

```console
$ docker pull debian@sha256:3e03f37e8c3b9d76daa8fe6a65bc09a884b0dbdf1160667fcd8dcb0486caabdb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.3 MB (54339443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aeaec4fe823eebba7fd2a2dac7fbb55436ee9630e6861207936ce8e68f8fb9c4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Mar 2022 08:57:54 GMT
ADD file:37d0293ead8c516891cdd3f88dff72fb70addf7dd2381e7112760b973cd8b5a5 in / 
# Thu, 17 Mar 2022 08:57:59 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 08:58:09 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ebbe8273ea4fb310fc98390a69df247f2274b237e8bf487c86f0aa31fceb5433`  
		Last Modified: Thu, 17 Mar 2022 10:49:05 GMT  
		Size: 54.3 MB (54339219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd79e4439f5452182352b18f266b662ed2c5798f59db172f129b1c006a5bc0a`  
		Last Modified: Thu, 17 Mar 2022 10:49:14 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:ac46ff5702145f41da190f624700889c1dea69e48719435d34b3ad8b668b8927
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.0 MB (59999581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e0a8e456600bd71956df9954c25be3055e6c550a291b9058ad571e6c675d729`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:25:37 GMT
ADD file:8974d32898b791c51a9fab708550a07b9a517c5d9bd6db47acd59606984b81aa in / 
# Tue, 29 Mar 2022 00:25:42 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 00:25:55 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4b9bd4aec57ee466c8fe8d1c7e0f4e5c7e7604e860d3e58360a2dcf666c0b516`  
		Last Modified: Tue, 29 Mar 2022 00:39:35 GMT  
		Size: 60.0 MB (59999357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c044eb47ee027e16c96c45f545f4fdb93bf34bda31903b020d8da1c93b47938`  
		Last Modified: Tue, 29 Mar 2022 00:39:52 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:8d05e841fca28485a23ddb01a2b92ec19ebdafc996f9e2ba0fbc23a23faaa638
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.8 MB (53839069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc4780a43c2570e5af595f31825dbc7f116da4b468a37333a2c9bec9bbbf8bba`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:53:57 GMT
ADD file:923d8b991f14b65ad1dd12a880ccd34f0f6a517d32736abd46b5f3b4dfd767d9 in / 
# Tue, 29 Mar 2022 00:54:00 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 00:54:06 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4b047e7b46b8a2d7592481c4bae7396a7669fa7dc3667f8cc1a2cf9adca2837f`  
		Last Modified: Tue, 29 Mar 2022 01:24:45 GMT  
		Size: 53.8 MB (53838847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c8a0ad7423fd413de1371c3d462a576b0debd53789bc0cd2808f0741107ea7`  
		Last Modified: Tue, 29 Mar 2022 01:26:12 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
