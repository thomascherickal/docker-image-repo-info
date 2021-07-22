## `debian:experimental-20210721`

```console
$ docker pull debian@sha256:72cc58b7447e72c28a67295353a1d1fa85b953053393ee8aa84a1fbb77d07260
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `debian:experimental-20210721` - linux; amd64

```console
$ docker pull debian@sha256:17e2aacf5e2c3257169c076a5ef5e73188dfff30dce051c67735a202d01e9de1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54909451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3d3b8822af2e26039eddd5638bf37e984af6e729aa2911c415a384612018c67`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:47:56 GMT
ADD file:72caaedee988b94c64ab78132092fb61535d1afe60e1ce6a6cc89af671204510 in / 
# Thu, 22 Jul 2021 00:47:57 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:48:12 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:384fb8afa5630c2860fbec8ef28c7001f980f4a54cf0db82bbe68ee7634d6005`  
		Last Modified: Thu, 22 Jul 2021 00:54:24 GMT  
		Size: 54.9 MB (54909230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3be2f8c4e56dc212e22639f90bdcc33b4e48c21be6bc1b13ec314fd219910f`  
		Last Modified: Thu, 22 Jul 2021 00:54:50 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20210721` - linux; arm variant v5

```console
$ docker pull debian@sha256:452a491f0cca558ccbbf9ecf578a3fee92cbc361ca68f4f0e98f2b15eaf62d6f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.4 MB (52446220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cfab69fa43a9c5c87f0dc74835a417e4475afa7a15368afb8d8c936b50fa29f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:54:58 GMT
ADD file:130a56cc4f62c5f99992b40717d91aee59653029881066d5d2f6aa90f3c534c2 in / 
# Thu, 22 Jul 2021 00:55:01 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:55:33 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:02fd227d65b202bd21ad9f318e3bd4c2fb7fdadef762296f692a14c87e4287eb`  
		Last Modified: Thu, 22 Jul 2021 01:09:14 GMT  
		Size: 52.4 MB (52445996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f120935126b6f6a1ef8ef39b08cb2d4a7b9fbbc2713d6740f87e50da689417c`  
		Last Modified: Thu, 22 Jul 2021 01:09:57 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20210721` - linux; arm variant v7

```console
$ docker pull debian@sha256:abaff37bdbcfadac2191c85bbef15b846e077a978e26863c8b9877e29bd38d32
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50112070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:135d1d4fc916136756d99355250e694ad1a7192f45a31d20a8a6e94d3502c88c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 02:08:55 GMT
ADD file:1b3b77d60136df3dd46ae0ea23986c26640584a24bfe5dac4d8082fb81cec664 in / 
# Thu, 22 Jul 2021 02:08:56 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 02:09:29 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:f75829fe215f0952fcc8ef08bca0bd5050b0fcf9e8474e54e9d8fea9965d044e`  
		Last Modified: Thu, 22 Jul 2021 02:23:18 GMT  
		Size: 50.1 MB (50111847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d924350570e995b7707a22fedebf98816aef7fa43458322e39d0c51ee0d410b4`  
		Last Modified: Thu, 22 Jul 2021 02:23:57 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20210721` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:bf5df7fff2370d245f794ad24afaa1c6ee83169ad0bc496d99a6fc3e2f74b88e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53593283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40c2d9302eef6e74d502264318425024a5b6be7c0158ac0f0fec86f5256113c0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:13 GMT
ADD file:5d2db16f160a8360a29d92801065a411eede3b29bf0cd69a6168c6a2a599a365 in / 
# Thu, 22 Jul 2021 00:42:14 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:42:28 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:e2205e97a09a5d09ac3d40cd922e7a35add0202c6862ae06197982a50246e61f`  
		Last Modified: Thu, 22 Jul 2021 00:50:01 GMT  
		Size: 53.6 MB (53593063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e134dfa7d3da97b9ea5ae4b0fcd94eadb2aecbf0d4dee00becee10466a34f68`  
		Last Modified: Thu, 22 Jul 2021 00:50:34 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20210721` - linux; 386

```console
$ docker pull debian@sha256:ae8c8b9f0d36ace05a511e7b10319361f3c5a51c2793029f314643f5a4955294
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.9 MB (55915435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7881e4df3ec60e6d4a149d75d70966ab0967846222462e572fe679919a1abe5`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:31 GMT
ADD file:9be8ea51c78319f68bd9dafa13311d032d06e6569c1ab5769d6d5515c79e63a5 in / 
# Thu, 22 Jul 2021 00:42:32 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:42:49 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:33efe91dae7ca8af00c12da471d2bf12430dcc92c5bb6d32a5d95013949d7270`  
		Last Modified: Thu, 22 Jul 2021 00:51:13 GMT  
		Size: 55.9 MB (55915216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a699d8592b672b626b9abf237bd3a1d5ccc826779a0da30d9f60444f16eb2624`  
		Last Modified: Thu, 22 Jul 2021 00:51:41 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20210721` - linux; mips64le

```console
$ docker pull debian@sha256:eeeb1c4b837b8fdd9d255c527b03621185ad1a3384d33f63eed3b6c8fd5c1b8f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53162258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e443b17afb1faa09c05ddcb4958c1bebe4f9fb265b25393f5b828b57fe09caab`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:12:32 GMT
ADD file:a4c6831bef1196d14300e45f0140aec5bd1d25178a98f7b08c649e409a7995c8 in / 
# Thu, 22 Jul 2021 00:12:33 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:12:57 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:808259531ead922b774f301a6378a5dfa29526dd387e81a5ad5158c4efb0fcf1`  
		Last Modified: Thu, 22 Jul 2021 00:20:49 GMT  
		Size: 53.2 MB (53162035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6fba1fbe4ac68b89f496039cd6bbc3487fb3d3e85394c012e80c2be0947621`  
		Last Modified: Thu, 22 Jul 2021 00:21:31 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20210721` - linux; ppc64le

```console
$ docker pull debian@sha256:1afb2ba983cb69252bd7dc7a7878d7b094f452c778ab1bead9d36c115ee9db9c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.8 MB (58810999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1491e4d84e4578a5045a63b6a08e67fe8f81941882f165234c43f8cb5e3cee85`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:22:30 GMT
ADD file:42719afae650d02663f605c5171f891a1fa9675c8f304c5e98573dbf8f82ee6d in / 
# Thu, 22 Jul 2021 00:22:43 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:23:19 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:d611f21aac479887eec681745ae379746661693e6d119806173bfff5f39ee0f1`  
		Last Modified: Thu, 22 Jul 2021 00:30:42 GMT  
		Size: 58.8 MB (58810778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ecc6a15a703df6a7c199fc8477427aeb02badd59f6067baee413e1552e9bd3e`  
		Last Modified: Thu, 22 Jul 2021 00:31:12 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20210721` - linux; riscv64

```console
$ docker pull debian@sha256:52f4ced84b7120e2593cf4313ce8c5dbb603a1a6b0adc7538485dc3278b0c273
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50397971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b71c7a884d9b02f98c0ec3c8da5d21edda17e2f71ddeb3c50f5d2427c1ac9208`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:35 GMT
ADD file:ab01cc13642b25f4108ecc46ee864da39800e744dc99a94d677ff6e5e09c048f in / 
# Thu, 22 Jul 2021 00:19:38 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:23:23 GMT
RUN echo 'deb http://deb.debian.org/debian-ports experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:39d5cc0ccaa154e3314690a929ab45e6959d5450db5dcb130c4bb57d06c61cbf`  
		Last Modified: Thu, 22 Jul 2021 00:38:35 GMT  
		Size: 50.4 MB (50397743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da1b88c53aba5af7999151118b0ced6be64b58b1de3931afb87995cf41ec5a9`  
		Last Modified: Thu, 22 Jul 2021 00:41:46 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20210721` - linux; s390x

```console
$ docker pull debian@sha256:5a986745584c0bc13489ff057d9a443590020a1228032c9a65798f500181fe74
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53187585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5ba4c892d3e3236efacec995fc847ce556b436021787095ca6bdc1e495448b4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:44:48 GMT
ADD file:d0e4eee5872ed1aed6b231a20dc224db3e46a36091ff28c7a901177da5a22dd9 in / 
# Thu, 22 Jul 2021 00:44:55 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:45:16 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:c1ee92b8f41eeaafca724a672297442ccb37919653d1adf4915109ec66e8b49f`  
		Last Modified: Thu, 22 Jul 2021 00:50:08 GMT  
		Size: 53.2 MB (53187365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cac7147b852ca2e0b273de88954d2403dc3674a07b20fc9d07949a501e608e`  
		Last Modified: Thu, 22 Jul 2021 00:50:29 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
