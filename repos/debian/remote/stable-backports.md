## `debian:stable-backports`

```console
$ docker pull debian@sha256:abd48eafcc64c0efa799e8d182ca2f0f20397d4589dcdcc4a399c61282794eb5
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
$ docker pull debian@sha256:17c29da22f9469eb5d9af9c409fcc60c75a5446af6fd0c5dcceb5ca4fd02e690
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50433058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1a02a1a82963a0125b1ea1354ca8320900dc5a773723392309f65fca0f5d840`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:19 GMT
ADD file:80f28ad4276ec83bf9fcc1ede1fc76380d61f1f0b1d461829663883e56b6cece in / 
# Tue, 30 Mar 2021 21:50:20 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 21:50:24 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6c285165b84904bd248aaa2f1b60bbfbe6d8a87b77898075414d1b044273b25d`  
		Last Modified: Tue, 30 Mar 2021 21:55:52 GMT  
		Size: 50.4 MB (50432834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb45d57d33f4b69fb502ccd0cda0b58b4ba73a3aa2ea2b62183ba1b4a3fec741`  
		Last Modified: Tue, 30 Mar 2021 21:56:07 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:9f7e850b402fbe075644e75b380b61aedf09a710a8b7c3e21cf034a89916b4f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48149345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d00d3dc3eaceceaf7cc2499eacbfec1657f4c61734bc4d77a486d22a75348806`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:52:54 GMT
ADD file:b5c420fec2be269b82df8ad0d02c0c61cde9208c7bec2881c54fafc69561b4a0 in / 
# Tue, 30 Mar 2021 21:52:55 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 21:53:06 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2abe5b28c72fc514a3153318a1c5d930ecc7b1f03325080b677a9c5db31f8192`  
		Last Modified: Tue, 30 Mar 2021 22:00:37 GMT  
		Size: 48.1 MB (48149122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345c3888035c8289b0ca5dcfd0fbe167843da76a7b0d4f94e5bc7d58e353d0f3`  
		Last Modified: Tue, 30 Mar 2021 22:00:48 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:d6804cc516bcc2e5532f7ba40eecd4487e9c0689d3ea6998631f51ca49c04af2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45915650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cbd2b5226813c064cc99293894e4eb5e63937b66ba4da5bdfaa92e079bc9248`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 23:10:42 GMT
ADD file:6e5fe58c2f9f9d07bfae7e666ff0c3c7be1f3e1f0f08152d03106d03e18d1e60 in / 
# Tue, 30 Mar 2021 23:10:44 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:10:52 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:05f1b368d94a408a533a786e1ca226afa65eceb0ba31541cad40369f411ed5bc`  
		Last Modified: Tue, 30 Mar 2021 23:18:08 GMT  
		Size: 45.9 MB (45915426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f22e192b3f796a2037c3b9e72855eae1d4c9245a53d50113d7ace3bad1b374e`  
		Last Modified: Tue, 30 Mar 2021 23:18:16 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:ff8510c7e0587b4fe641015947e99d0ec78196fc901c01c3d7209aae9c98a91a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49226041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47aaabe4b92fa4f513a6f3c3e124fe07fcf2675b584f20a629e31ba9098ca36d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:48:59 GMT
ADD file:218ff586d23d7f91c721d44eea2bda1ac41281603b217d862a891b4091e417ac in / 
# Tue, 30 Mar 2021 21:49:02 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 21:49:13 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b4ee9067295efdc02c7b212b09d546bcfacd3e87bee105bfdb5820a2393d88a5`  
		Last Modified: Tue, 30 Mar 2021 21:56:01 GMT  
		Size: 49.2 MB (49225818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689adededbc5a124a824b4ac5fb0a1d3cd2295cd1a1ed32b167b2c135121c75d`  
		Last Modified: Tue, 30 Mar 2021 21:56:13 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:ef5a464b575bb4becb0b5111af0e52bca8f7dcf3c62d003d8083117a6e51bc80
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51198962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a551cc7140d8ac4870ac58ccc83027ada94546ad4533be7067e5f327106e3860`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:41:01 GMT
ADD file:7a9c68e0c955ff9cd19024d29752e5aa3fbfea442ef6cb10568bb936ce5ff54c in / 
# Tue, 30 Mar 2021 21:41:02 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 21:41:08 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d7ac3e5f456b46f6a35d805cc438c6841ea57aa2122e1f3344dd017757d931d1`  
		Last Modified: Tue, 30 Mar 2021 21:48:39 GMT  
		Size: 51.2 MB (51198738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d03a7c438732f363ad6603b98fda1d205cc57fe4775bde779bc90eb359cf91`  
		Last Modified: Tue, 30 Mar 2021 21:48:51 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:7f9a7135d185284ff26b78200d07310aadd62e1bc1fa8cbe84bc722d6d38473d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49082102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:687606b2d55ff16cb50978edccd8d382ea33f852a2ca0c2cddca0d3a2b3277a1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 22:10:57 GMT
ADD file:370ebe08b480f9a216be10725cb8895be7820ab55fca469677f7247e7382edbd in / 
# Tue, 30 Mar 2021 22:10:58 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 22:11:04 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:213c8289b0d779ce6c722e21f96329e885d10fc611e42bf94ab60eec39baeec0`  
		Last Modified: Tue, 30 Mar 2021 22:18:21 GMT  
		Size: 49.1 MB (49081880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9dc8176fa8802d335159b8043ec4d1b8edf362dd3be598d9404d3b45a1631e1`  
		Last Modified: Tue, 30 Mar 2021 22:18:32 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:220a9caf4ac2e55a9c146a9081395a28351b17f5f4da78e3ec3fe245c6b21a89
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54180011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29d015a53373aa5a70b37b7275978ec41b92ec929f0941adb9660ec09c5af1af`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 22:37:10 GMT
ADD file:bc748596e223054d58dad5acb8964b67ef0d276d368803cbd5f5a0c424845076 in / 
# Tue, 30 Mar 2021 22:37:18 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 22:37:35 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:108c0b8eca0ec2ca6aee26c5bec2896ae6a328064dbe238bd58a2a8608489dad`  
		Last Modified: Tue, 30 Mar 2021 22:43:54 GMT  
		Size: 54.2 MB (54179785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c0211be0d4e7deb0a447fe92abc4e6fe3387e645125cc9e478a95f11fa87bf`  
		Last Modified: Tue, 30 Mar 2021 22:44:04 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:5b075b81710dc2106ec4b2814795b10bcbd58ed38e285573d9dde10ec40c8149
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49000693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:060d88ff547414901588df8fde53acd0ba5e92ac58d97482efdc85b3d8b101fb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:43:18 GMT
ADD file:b70215bdb74e45698fe819c9d4b01582051b77d523659639fc028a89a4f5e0c7 in / 
# Tue, 30 Mar 2021 21:43:21 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 21:43:26 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4959d7ae8d7311060164ca4be86892b52605ed786b85da59f17eebe056ac744b`  
		Last Modified: Tue, 30 Mar 2021 21:47:02 GMT  
		Size: 49.0 MB (49000468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46baa8e55a83df27f35e21cffb1bc7e50166a991cdeaa3aad1c76d6430a83f28`  
		Last Modified: Tue, 30 Mar 2021 21:47:08 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
