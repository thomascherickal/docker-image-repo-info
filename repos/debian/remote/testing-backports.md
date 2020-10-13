## `debian:testing-backports`

```console
$ docker pull debian@sha256:1f03509a5adb81323e29e98e32d9322fbd4b8ead853f59e85c4e2ab751d30027
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

### `debian:testing-backports` - linux; amd64

```console
$ docker pull debian@sha256:297b8d2e17af542076a23bf76fa712832ce003da3f256fb6634c71764d1499cb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.6 MB (52579900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0453cd0f1382803b2dafabcdcfc349a7a5d43fbb6584e2ac31aa88ae68d82455`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:45:13 GMT
ADD file:58fd470c136e9fdd11c90e919ec97ba87bee364229cef3458b708f163f24f756 in / 
# Tue, 13 Oct 2020 01:45:14 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 01:45:20 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:57d5d8b09e9170c45af4cbad03f9fc30044c0116f4049d363f0254515cef5fe0`  
		Last Modified: Tue, 13 Oct 2020 01:51:19 GMT  
		Size: 52.6 MB (52579675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12725c53d9d93f1ce4f0f819a3dca29f19c7a7658682c9a9e79f20c659228762`  
		Last Modified: Tue, 13 Oct 2020 01:51:25 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:e077f061d4f613735b1ce9b34c3fea760420fed042ae2a84b078978ad0196e8e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50502310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e5e7b8ea54c67c5d2bf7ff477ad6fb1106158389ea5bb9a973dc7b4d5c9143b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:57:50 GMT
ADD file:f9831e4e34c6258ee0a83d118b641ac4d20eef4877156950a9e7c2be49a1d4e4 in / 
# Tue, 13 Oct 2020 01:57:52 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 01:58:05 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e090a1a37e716917d9a15b2a388b6a20c42facd0af2a586e087cef484742dfac`  
		Last Modified: Tue, 13 Oct 2020 02:06:03 GMT  
		Size: 50.5 MB (50502084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f615b558e0b16f4a375a1de56daead11c5ef407eee846b0b9236f1734b0249c`  
		Last Modified: Tue, 13 Oct 2020 02:06:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:59847a917bc82db20ff0df08b239d9487f45666b0011e5cde2d0080b4a7febd1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48236917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbd1c8e6bb2e5bfb5f5087ec3702357843f5f4066f5f79ee0d2691d99fdc9e67`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:04:54 GMT
ADD file:0824d3a0f4937ed3bdb74054868c75851f95be6fa0a8350f7472e61ff6896362 in / 
# Tue, 13 Oct 2020 01:04:55 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 01:05:04 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:33007ecbdf4367f09e5eb2141084c0a3decedd2fcafe392652110316ca7ed8f3`  
		Last Modified: Tue, 13 Oct 2020 01:13:25 GMT  
		Size: 48.2 MB (48236692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80842940da343342f2c8e2feb7a3d51278f344a1c310502b41290fbeb2e5037e`  
		Last Modified: Tue, 13 Oct 2020 01:13:33 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:7147e1b76410ae3202411689cdce6f7ce8385c3fc7e0c3f9b0c37cb3f292977c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51484510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1a095ebcc7130b750d4157c1560d35e95a0efdd49e4028f9f64a3525e0bf0e4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:43 GMT
ADD file:e1dc4f74cca26ba51ab2b0514641801b22d0f0a2eb7e8f2b4c54cc36a75494d4 in / 
# Tue, 13 Oct 2020 01:44:45 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 01:44:56 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c2b4ce940f2a9cdf9744b56e1bc9d370237dff1f0040d6944415cf7d5f7fb20d`  
		Last Modified: Tue, 13 Oct 2020 01:51:35 GMT  
		Size: 51.5 MB (51484285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2907ebc950de5298e85688e61a05d1fda779e1971f4ea32f7ab2bcdcc17826a`  
		Last Modified: Tue, 13 Oct 2020 01:51:42 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:7ff03847245836a0adc2a19ec5b63448cd9e3257db36c63791f6cdcac467da88
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53627956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:085cb9fdd78cf0f405c931e547f253227448a29b6a03c4ee55ec727b8663cf6f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:45:54 GMT
ADD file:5a48f78b466449c034ced1ef433fe150827e1c2152893e4160a313bf34b1d402 in / 
# Tue, 13 Oct 2020 01:45:55 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 01:46:02 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:158cac692856a9120e207509a79276f198348dacf6cb0bdde8dddb06e1bacafa`  
		Last Modified: Tue, 13 Oct 2020 01:52:31 GMT  
		Size: 53.6 MB (53627730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca43cc05cf0543cf2971fa4ba4fd0be556b3c87d9bdae939e04dc0abc6cf909f`  
		Last Modified: Tue, 13 Oct 2020 01:52:35 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; mips64le

```console
$ docker pull debian@sha256:bd4bb841ab3bda0cb592b5a396aa8ec7aee15e3643307384ed183386c556f1d3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.3 MB (51280117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c937dfe78598d7b211e6c24833956c113230831be153d5b7ea0aa7d759f2c5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:12:05 GMT
ADD file:a8aa71ba87caf382b1145d79c8efbea003f3a15a72db2a4da321cd13388ce1d2 in / 
# Tue, 13 Oct 2020 01:12:06 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 01:12:11 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e9d306d81d1898f3f44b8144eb502816eee59e45fda34aa46e4883de4c4b2fb7`  
		Last Modified: Tue, 13 Oct 2020 01:19:55 GMT  
		Size: 51.3 MB (51279895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:545f88f36d80a6807a767859b40f9c76daa175211c77f7c5ea9a493615e80842`  
		Last Modified: Tue, 13 Oct 2020 01:20:11 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:f636ed67a15d22d4049cd139de2dcc7a9567cba95aa978571412221f3e2ac868
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.5 MB (56486625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d91c1e448630d25e83b4575e847ec37e92ec13ec099868ff42713f91d848eb3f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:36 GMT
ADD file:391f7beabdff070d3417ca142cf9cd5a48f50f2d865401f3fc0cafa2cd0ee9b2 in / 
# Tue, 13 Oct 2020 01:41:43 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 01:42:09 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a3755d6e5159d63f7070ee41c1dc98d6ba8aa63edf93e38cb36d2dff626b94b5`  
		Last Modified: Tue, 13 Oct 2020 01:55:40 GMT  
		Size: 56.5 MB (56486400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac8275bdd258680205995e24cdf0472aab8a6c089e351e5a71e32ec68ecf4ce`  
		Last Modified: Tue, 13 Oct 2020 01:55:54 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:ebdcae93f93ed5da80bf9d7d5bac7982f1cd38387aa7011160c2134d042f302c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51119047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f530ba7c88260aeba8224600000aa29f13d536a2f0bad0a13b6cd0e9ab2a3825`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:43:39 GMT
ADD file:69ade3c1c4b493157a23f41edcc1da760398f8a1cec81602e72ee7b8b26b4a76 in / 
# Tue, 13 Oct 2020 01:43:41 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 01:43:47 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6f09154c5e80b4d12e4c72691bb2d8d8c39a7a2e45ccbf3b79576a2b54601b38`  
		Last Modified: Tue, 13 Oct 2020 01:46:58 GMT  
		Size: 51.1 MB (51118825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d071913cc6df2969533dd6a7ecf909b597362e03a5c2076d7b7d16b30214fe32`  
		Last Modified: Tue, 13 Oct 2020 01:47:06 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
