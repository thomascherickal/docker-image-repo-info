## `debian:experimental`

```console
$ docker pull debian@sha256:e76c20ce1b7f1263f671ed80b5101ff4c373de1573634b8cc8075713bfe508a1
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

### `debian:experimental` - linux; amd64

```console
$ docker pull debian@sha256:352051d681ceadf97fda9f9d95d03273b7522a15f534208f786504b151dd0e82
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49534527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9e455eb468ef746580f05539e41a128c47a970c731129e31433759cfab77599`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:23:54 GMT
ADD file:9c058e7ea601a027f92fff816e442f2e38bf7d787fb9224fbf223c8726b1fbdd in / 
# Wed, 01 Nov 2023 00:23:54 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:24:07 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:1e0f4722d93288d1e13763cb35b29e239dc5bce0ab1ebdf97561a23e2b86aba1`  
		Last Modified: Wed, 01 Nov 2023 00:30:45 GMT  
		Size: 49.5 MB (49534306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2856fb3f9f1fba8a260be036dfc5ef7f198d086c0860d95780a45dd5477b62`  
		Last Modified: Wed, 01 Nov 2023 00:31:08 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v5

```console
$ docker pull debian@sha256:34361f3de6cbf5ca82e1848678972f10bb1c9fe5588e9f5c082cad98906b9b6b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47196924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07ae663ed2bde65d64b427e9f06b69bf1aeac44b673ac2df6c9c37792d3614d2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:02:40 GMT
ADD file:bceec73b119ad7995eaf06905d19884e80e91642f6509846be45522fac26171e in / 
# Tue, 21 Nov 2023 05:02:41 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:02:50 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:dc1f441734dab214a26a2bcdc1c43bd72e1154d95a7024417f3ed87e150585ee`  
		Last Modified: Tue, 21 Nov 2023 05:07:50 GMT  
		Size: 47.2 MB (47196700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b652161ee3d87951ee63ed20907b48a1fccad159968947d0515e0f5a1998b73a`  
		Last Modified: Tue, 21 Nov 2023 05:08:12 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v7

```console
$ docker pull debian@sha256:6cc2df07be03c77387ffc0c3326c5638fbbd9c0d4c49e8543619c29867a3a428
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.8 MB (44844227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54b48e13819400565bd72d93bc3069ac76c065dc3f0f0605b02a6348f5aa1cfa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:00:15 GMT
ADD file:8e091f00e04d8cb85cfce52bbabcbac6c260e95c3f3a00752186e465f583b2ca in / 
# Tue, 21 Nov 2023 04:00:15 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 04:00:27 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:bc7b160f4eb0bdcb6d980297d91f215375ca0669f74456162ed2c3a6534ceddc`  
		Last Modified: Tue, 21 Nov 2023 04:07:09 GMT  
		Size: 44.8 MB (44844006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a69e60ef4d54cab41871e2cb5a7bec428aea9ce83d55e58fff0dee9198f58e0`  
		Last Modified: Tue, 21 Nov 2023 04:07:32 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:6f31cb7e697fca1d46aa4b1ce420d8af30eeffa678a57dd7c1005dc55b25f337
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49553063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48aa735468bab4419939071c705745750d0e78d69a7ccbbc3d1a317bb394d9d3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:41 GMT
ADD file:73ccf1f3ada3f6531f17430ebaf790ee664bf9968fcf3e9b537a58abcc64a0a2 in / 
# Wed, 01 Nov 2023 00:41:42 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:41:50 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:7aa4384568145e6ec8cdfa393fdb3efd1d2484cdac27d767b07d54e923c12a7e`  
		Last Modified: Wed, 01 Nov 2023 00:47:46 GMT  
		Size: 49.6 MB (49552839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3163c71a522d116199408ce2155c29438879029e3727b94e446b3da9e3f540`  
		Last Modified: Wed, 01 Nov 2023 00:48:08 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; 386

```console
$ docker pull debian@sha256:4c0eb0477226a18e7b867aafa2c94efa40068489cbdf6497c54341234b27fb24
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50514053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f94fe66d580fd3c85a291cb7f9b121dc66595b1c6574768497d8a9de867d30e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:42:56 GMT
ADD file:b98d36844697f1344eb11bfd40332d2eb9217bc8007e97ed74592a9bb31c7570 in / 
# Tue, 21 Nov 2023 04:42:57 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 04:43:08 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:147ceb094c0a68c71e76e31ee257dc07454a713d5eba2a55351d05bee2fe53c1`  
		Last Modified: Tue, 21 Nov 2023 04:50:26 GMT  
		Size: 50.5 MB (50513834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6e39d2effc6b1d09e346a98e7057a66957de6fb0b3029f96b9d14a5b5e1686`  
		Last Modified: Tue, 21 Nov 2023 04:50:49 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; mips64le

```console
$ docker pull debian@sha256:ac3424f8285aee17a00a654ec7dde3bea039e6c5ebc497b154bff00be19800ef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49342071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0d1e922c701c25bf651d83210ea4fe69259140b9ad07101bb3eb0ab2af93972`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:17:31 GMT
ADD file:32388f25898c590557e184be8d1a25de1c8d0d46118ef57a0a76b0c893108d41 in / 
# Tue, 21 Nov 2023 04:17:36 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 04:18:13 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:e3dc12456ffa080d32be43a02cb6024e94ce186c09ce60151090c1296700a438`  
		Last Modified: Tue, 21 Nov 2023 04:28:44 GMT  
		Size: 49.3 MB (49341850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce08a81bc78ed1a698eb461ccfcbed917c55142347a46fce41f97411329887c`  
		Last Modified: Tue, 21 Nov 2023 04:29:22 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; ppc64le

```console
$ docker pull debian@sha256:1db54ee1e83d43cad2dae9800ffac99670508f250cc99589cb7cdd915677e666
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.4 MB (53424065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a87b75540e156f72104f61ced5aac643b5376dcb23531be262f87e4199a5103`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:27:15 GMT
ADD file:36d1b65e70c748f81fa571c211784bd684a44b6bf1688cf224e0b40112f948b2 in / 
# Tue, 21 Nov 2023 04:27:18 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 04:27:32 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:50bc207358121ecad8d7b3904464fab6cd43d21b4ba1e393141dac06112bcf0d`  
		Last Modified: Tue, 21 Nov 2023 04:33:20 GMT  
		Size: 53.4 MB (53423844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70861f95595d64ca996f53da650b213556b8dbf2f41208262b8facfec2b82f7b`  
		Last Modified: Tue, 21 Nov 2023 04:33:45 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; riscv64

```console
$ docker pull debian@sha256:1e72d63906b9a8c4d0a64ed1e98c02cf05a02268f3e6fe285b8ca0a325aab6dd
```

-	Docker Version: 20.10.25
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48206923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:013871bd9721543bf4ec97e375d9c2223b75834ecf613fa142e2035ea46d9b5b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:10:08 GMT
ADD file:f926dc89ba0815e0a23356d88037340957f7a57bea917a3aaed678d1decf7b22 in / 
# Tue, 21 Nov 2023 04:10:10 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 04:10:48 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b1fcc4091b722aae5f7f102ced62233745368e2095d318f03282cc819757f97e`  
		Last Modified: Tue, 21 Nov 2023 04:13:22 GMT  
		Size: 48.2 MB (48206699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60afd7f2b0f8844688b4d838bb33218c480848fcdfac7245abf07bd96e9286dc`  
		Last Modified: Tue, 21 Nov 2023 04:14:09 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; s390x

```console
$ docker pull debian@sha256:7fb04fcc004b2b9c218005ccec82aeb7d4a9b8178fdcbb0d7c7159b3af9387ef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49228338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f470556357128ad18ad8cac61e898906cf789b9b0d591c061368d426b1b37b03`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:08:40 GMT
ADD file:73ec4f9d8dbf70a36e53e50c5979f76de546ac747d7e6dfff7ad8a79154f30bc in / 
# Tue, 21 Nov 2023 05:08:49 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:09:10 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:01d2df6372c00ac73e4d879e803d41b949f8c149d760bfb8d5496b7d242aab0a`  
		Last Modified: Tue, 21 Nov 2023 05:12:48 GMT  
		Size: 49.2 MB (49228114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1606ec173f0fedc7fc85930963cec85cc58f229d2c6b8537e2cc5283ff5120`  
		Last Modified: Tue, 21 Nov 2023 05:13:02 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
