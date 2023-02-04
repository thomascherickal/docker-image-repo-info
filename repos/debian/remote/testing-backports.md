## `debian:testing-backports`

```console
$ docker pull debian@sha256:4e665282354028cdff842621c34969d010c6230ab0b6a6a8417d4fa460a5275f
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
$ docker pull debian@sha256:24275d9e2ba720ef8812ad86f2c298c2ef977599138ef0b7a0356546bc03c5ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50106716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d99c9f63f2d5b2e294ab6a1760d14ef45edddf9b6617fec1a2a87782a2ac23a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:36:25 GMT
ADD file:22d1bfbf515d54cfb8cc550ff465c1c0cb9a4abf7a340310c25b479079210d01 in / 
# Wed, 11 Jan 2023 02:36:26 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 02:36:29 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:37f2817160f3b2632e4625bfb13687ea793d896785b941bf53c171a4f2951c49`  
		Last Modified: Wed, 11 Jan 2023 02:41:43 GMT  
		Size: 50.1 MB (50106493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69581142712563d1f4a4b629b26f87ad2c870811609a9fb37f577ae57c1ffae9`  
		Last Modified: Wed, 11 Jan 2023 02:41:52 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:4002f41284247f9c64990bcd89fc0ff034b73e63a931c9ab5535364f19387983
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.0 MB (47993471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7220ce7b48adcb510cffe423a1e94797ff3059a41a38c6aa8c82c458ff303f86`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 02:47:39 GMT
ADD file:98e47e6350976474e8c5ce450917a12c04e080ced6ab05eed9e04772c5728570 in / 
# Sat, 04 Feb 2023 02:47:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 02:47:47 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:01cdab3e0a4d64aa88c8c65852e4599d329659e9aa85a26d1ae3f1565db6ea9b`  
		Last Modified: Sat, 04 Feb 2023 02:53:31 GMT  
		Size: 48.0 MB (47993248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e542969ffccee238f8d18194c3c32fa7352b532da45e6ce9624db3718aa7a1b`  
		Last Modified: Sat, 04 Feb 2023 02:53:42 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:3380b4c029d9d23ae317710736da2f9727547d681075a81623a2e94da3dcb96a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46896414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56ed7a2ddb7b48058c50196c303bd8e0ce9ab21619db48e213332b8d6da0555f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 04:03:03 GMT
ADD file:e265776b6b62da8ec73c72802a5f45c56311664fad279e039488fea3e773baa3 in / 
# Wed, 11 Jan 2023 04:03:05 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 04:03:10 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:eb7363eac3e82dfa1a2e2a380dd18728860c5f00a9451d64956ea62d0a97aa61`  
		Last Modified: Wed, 11 Jan 2023 04:11:04 GMT  
		Size: 46.9 MB (46896191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a65d0f618d512228f2c37f5bae4b7dd0cde0e4722621896b42e504f4b7cc08`  
		Last Modified: Wed, 11 Jan 2023 04:11:15 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:3cd07d32cf922018823fedbc3d084dd431798bb57c6d77fb4c436da071fed0e7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50161839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03bbfbb9cb427d27dcb41bff76da44cbc3ea4796ab2a0a901d6ce5bc5b654077`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:58:45 GMT
ADD file:c23924e713ab52b9d332f43e0c153ad7676a8ebae8388a7b66e72a85167a3573 in / 
# Wed, 11 Jan 2023 02:58:46 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 02:58:48 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:df0aed7e9ae695c99ecd2ff90171c1fba9f80c00a6b0d37535d97eb1cc63c0cb`  
		Last Modified: Wed, 11 Jan 2023 03:03:50 GMT  
		Size: 50.2 MB (50161618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67153c3c50f70e92dc818da99b8171b63df39546a4ceb4c39be81457b88befe9`  
		Last Modified: Wed, 11 Jan 2023 03:03:59 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:ce5780f1c63a5c5777795b1229032f3bd227ac91478951d86b85ef7d99afe886
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51145242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73ea49ebc3017e5cc14b962db842e3952b4001101a4abdd34634af1f6be4c1d1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 03:18:06 GMT
ADD file:6844d4a2dc67679bd73a46761f113cb7f8966710bd5a9b2c6bb11aaa98558eae in / 
# Wed, 11 Jan 2023 03:18:07 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:18:13 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f8a2a12389e2c4a78c1b304491d95bc5cdfc352a48454885618037364b690bb1`  
		Last Modified: Wed, 11 Jan 2023 03:24:57 GMT  
		Size: 51.1 MB (51145018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f382fe9eb3f42c0537d0a37a3c28253532baf5d788966d123f63536467dfe8ae`  
		Last Modified: Wed, 11 Jan 2023 03:25:07 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; mips64le

```console
$ docker pull debian@sha256:8a782bebbc094edd5a2c3ad1e78b416ca89d9253c1f7135e6ad2f07e69cd117d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50120786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da1301657044c6d8b3321abb2d33fcb1cf2f929aedc3a2ed5d36a2327ad697c0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 16:37:45 GMT
ADD file:488d1e9efc2793cb7bbc0a24db90f3d4caedb4317378aa6bded81e7c95d23d4f in / 
# Wed, 11 Jan 2023 16:37:51 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 16:38:03 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:07add6c37fbd3dfd7f7e099832a7dfac7e83714a61b8b1dc5a824b3d6de56e79`  
		Last Modified: Wed, 11 Jan 2023 16:46:22 GMT  
		Size: 50.1 MB (50120561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26693889ecf7a4b3386617ea62a40a405b19683be8d3714df68d06f3340a57b7`  
		Last Modified: Wed, 11 Jan 2023 16:46:32 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:dd64c66212fa6c71b4f51b0ef826ba3973a7f2e43c5ced88d060916a3d88849b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.1 MB (54144138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d881f0032e812689381081155e842c744dcfbfdeae0caeb59c98da2f29ce2833`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 03:51:12 GMT
ADD file:f81974c52cc70632419a4bb9e1b0ebce34c50279cccdb80c4c55f25affd62354 in / 
# Wed, 11 Jan 2023 03:51:14 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:51:21 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5a076f88d4e3024706b03ea816ea1848f10b04e81272b548e79f552c7716938a`  
		Last Modified: Wed, 11 Jan 2023 03:57:35 GMT  
		Size: 54.1 MB (54143916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8645d03730215557c0d28075e647402154870ff46934875b407048bfd5147395`  
		Last Modified: Wed, 11 Jan 2023 03:57:46 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:8b316db32eb51d8b035aa9631cd8edd51421637daaf4e1dfde84019d4505df23
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47429925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:739da72d284bb05e62815eb38fa84fa807a5edbb7005a9ce9a2379822d1ca096`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 04:07:20 GMT
ADD file:bc5ff0fc30abad7ccd04b372b80a22ffd8fabd60c0b4ddfa367dc841415fbc8e in / 
# Sat, 04 Feb 2023 04:07:24 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 04:07:30 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b0d4d83e89902e21b3d9b4ff69c9a54c6af1968d9820327767ffd6c6f44e07dd`  
		Last Modified: Sat, 04 Feb 2023 04:11:30 GMT  
		Size: 47.4 MB (47429701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b77f205684f5ea27f72fab73a22d60fdd4edf9300ffc6d5a5f788b07e3e2400`  
		Last Modified: Sat, 04 Feb 2023 04:11:36 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
