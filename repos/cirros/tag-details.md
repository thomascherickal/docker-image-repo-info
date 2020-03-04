<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `cirros`

-	[`cirros:0`](#cirros0)
-	[`cirros:0.5`](#cirros05)
-	[`cirros:0.5.0`](#cirros050)
-	[`cirros:latest`](#cirroslatest)

## `cirros:0`

```console
$ docker pull cirros@sha256:477522da784f5b3c8e3d2c7cce37c6c00947f610be6ed5aa72e13dd95cdd68f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `cirros:0` - linux; amd64

```console
$ docker pull cirros@sha256:639af3aa2828aa4efa3e27b06857552fe2db74eed4bc107bedb23a6122493d21
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (5953477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8cf2b398779ae60d12d9372e5dbfb66c0ffaec0b0a246c697a266fffbf30a71`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Wed, 04 Mar 2020 03:19:36 GMT
ADD file:7dd645da025b829ce3a58eda283fd28cbb8ef5d018241a9e46d2f31702949d93 in / 
# Wed, 04 Mar 2020 03:19:37 GMT
RUN rm /etc/rc3.d/S40-network
# Wed, 04 Mar 2020 03:19:38 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Wed, 04 Mar 2020 03:19:38 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:3c4b29c44747d8ead42e1a03a594fa91e3950d2b3314e3ed2cf899ba13a38726`  
		Last Modified: Wed, 04 Mar 2020 03:19:48 GMT  
		Size: 6.0 MB (5952069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae1cdea52f92512f576ea638e421f7c9263d6134bea153fb8701a9ef6b6b7cc`  
		Last Modified: Wed, 04 Mar 2020 03:19:47 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bca7c60d756992600573a76c0459a7dbf42b6b3c293029de0d2d2b59732f2a5`  
		Last Modified: Wed, 04 Mar 2020 03:19:46 GMT  
		Size: 1.3 KB (1251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0` - linux; arm variant v5

```console
$ docker pull cirros@sha256:5613be73fa3d88979776d2e0f1ba9b90c3400f19002e419b4120cb06866403e3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.6 MB (5634381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e24ca8e4664d4bafb19195c2d34e52f6a8069ffe586269dcd2b0620aa75d6c4`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Wed, 04 Mar 2020 03:48:24 GMT
ADD file:f4f821b05b6cfb4f3fa31012adb331dd57c57d492fbe5a53a5deffa6026bfa0e in / 
# Wed, 04 Mar 2020 03:48:26 GMT
RUN rm /etc/rc3.d/S40-network
# Wed, 04 Mar 2020 03:48:27 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Wed, 04 Mar 2020 03:48:28 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:33e50245f4fc4104d55214e9b0362a821edebbb261134c9bb8d9b424a6f38011`  
		Last Modified: Wed, 04 Mar 2020 03:48:39 GMT  
		Size: 5.6 MB (5632972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ff859a9ab72f7109b6dac1af178c111e6be4fbe8ebc043748ab165d9c1e7a9`  
		Last Modified: Wed, 04 Mar 2020 03:48:37 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6cb0006ecdf0039402d90ec34055159dbb373fbaacfed3e02746f118f25e44`  
		Last Modified: Wed, 04 Mar 2020 03:48:37 GMT  
		Size: 1.3 KB (1252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0` - linux; arm64 variant v8

```console
$ docker pull cirros@sha256:9bb5da8a0a43f0cfefcf107c9d5cf5f1d0f01765d6dca0822e86a652ccf9f484
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5381496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49c2d66f9f12684a5bade65fd1049d9a899db7a53eb8a7da9447c3a8142cdd4f`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Wed, 04 Mar 2020 03:39:43 GMT
ADD file:a6d30e587ca56c660bf6dbf0257c89cedf5a89286ac825e93a0d1c459c54bf83 in / 
# Wed, 04 Mar 2020 03:39:45 GMT
RUN rm /etc/rc3.d/S40-network
# Wed, 04 Mar 2020 03:39:46 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Wed, 04 Mar 2020 03:39:47 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:35df11b12919a3b9827938de4a8b55176c7ddfb2e87cf559858764365c885446`  
		Last Modified: Wed, 04 Mar 2020 03:39:57 GMT  
		Size: 5.4 MB (5380086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dea8baa8412c21524088511648c32018f230c913308eedbc28a617c5dfdad67`  
		Last Modified: Wed, 04 Mar 2020 03:39:56 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5aba0358242a35568239b5061a318455594ac21042fd7d5d8da9b5f6801de9`  
		Last Modified: Wed, 04 Mar 2020 03:39:56 GMT  
		Size: 1.3 KB (1252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0` - linux; 386

```console
$ docker pull cirros@sha256:3c6e16d674e697a07f5bc4bf73f08d8e0a48b6e7ddc6e0f54c5d84fbeeb6b61c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5531739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:579b6baca511fd54c70e57c3656d94412fb4f47fe2bfa3c10a7d703ca9f8a3be`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Wed, 04 Mar 2020 03:38:26 GMT
ADD file:73657d1d105210371bedeae4e7dc0f6ab1249c8c42ad729ef767e6b3a7fe4949 in / 
# Wed, 04 Mar 2020 03:38:27 GMT
RUN rm /etc/rc3.d/S40-network
# Wed, 04 Mar 2020 03:38:27 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Wed, 04 Mar 2020 03:38:27 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:e7bd3e7f87713723923da5ab89ee97e7e847d04dd11972c048f3e0755e332c0e`  
		Last Modified: Wed, 04 Mar 2020 03:38:35 GMT  
		Size: 5.5 MB (5530337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c84906c79e8b33dc47bc7fa6602d1520f2e376dcc0fb0cf216713157dfd99c2`  
		Last Modified: Wed, 04 Mar 2020 03:38:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9068d613cfb0f637131254136e0465d4a21a0b7373f225c5566a5ef4c262e0c`  
		Last Modified: Wed, 04 Mar 2020 03:38:34 GMT  
		Size: 1.2 KB (1248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0` - linux; ppc64le

```console
$ docker pull cirros@sha256:83fe7decf7e2cc1f13aa9d216474c7d772bacbc50cba23c3af9e4519408f100f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 MB (5770658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b99c3db42160238bcaef14a19800216c78cf5c7ed7c0afcbd4470e5a4531aca1`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Wed, 04 Mar 2020 03:31:30 GMT
ADD file:867dd84e8959e9f1f3647b5391e6b4dce42ecc772c47119403f54db588944783 in / 
# Wed, 04 Mar 2020 03:31:35 GMT
RUN rm /etc/rc3.d/S40-network
# Wed, 04 Mar 2020 03:31:42 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Wed, 04 Mar 2020 03:31:44 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:81fa53a9c824a2d73ef844702e11d5377598b64257721313c21413efb753ce9f`  
		Last Modified: Wed, 04 Mar 2020 03:31:59 GMT  
		Size: 5.8 MB (5769250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b1a63bab9311d7cd0bbcb9c4e92bf1e37b9e64202b4788d566b272de7a7774`  
		Last Modified: Wed, 04 Mar 2020 03:31:58 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfaba3b952f0078fbb6a55f105e7bc6d2e6ff0566346a0b8f909843e4f7fff8`  
		Last Modified: Wed, 04 Mar 2020 03:31:58 GMT  
		Size: 1.3 KB (1251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `cirros:0.5`

```console
$ docker pull cirros@sha256:477522da784f5b3c8e3d2c7cce37c6c00947f610be6ed5aa72e13dd95cdd68f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `cirros:0.5` - linux; amd64

```console
$ docker pull cirros@sha256:639af3aa2828aa4efa3e27b06857552fe2db74eed4bc107bedb23a6122493d21
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (5953477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8cf2b398779ae60d12d9372e5dbfb66c0ffaec0b0a246c697a266fffbf30a71`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Wed, 04 Mar 2020 03:19:36 GMT
ADD file:7dd645da025b829ce3a58eda283fd28cbb8ef5d018241a9e46d2f31702949d93 in / 
# Wed, 04 Mar 2020 03:19:37 GMT
RUN rm /etc/rc3.d/S40-network
# Wed, 04 Mar 2020 03:19:38 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Wed, 04 Mar 2020 03:19:38 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:3c4b29c44747d8ead42e1a03a594fa91e3950d2b3314e3ed2cf899ba13a38726`  
		Last Modified: Wed, 04 Mar 2020 03:19:48 GMT  
		Size: 6.0 MB (5952069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae1cdea52f92512f576ea638e421f7c9263d6134bea153fb8701a9ef6b6b7cc`  
		Last Modified: Wed, 04 Mar 2020 03:19:47 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bca7c60d756992600573a76c0459a7dbf42b6b3c293029de0d2d2b59732f2a5`  
		Last Modified: Wed, 04 Mar 2020 03:19:46 GMT  
		Size: 1.3 KB (1251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0.5` - linux; arm variant v5

```console
$ docker pull cirros@sha256:5613be73fa3d88979776d2e0f1ba9b90c3400f19002e419b4120cb06866403e3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.6 MB (5634381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e24ca8e4664d4bafb19195c2d34e52f6a8069ffe586269dcd2b0620aa75d6c4`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Wed, 04 Mar 2020 03:48:24 GMT
ADD file:f4f821b05b6cfb4f3fa31012adb331dd57c57d492fbe5a53a5deffa6026bfa0e in / 
# Wed, 04 Mar 2020 03:48:26 GMT
RUN rm /etc/rc3.d/S40-network
# Wed, 04 Mar 2020 03:48:27 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Wed, 04 Mar 2020 03:48:28 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:33e50245f4fc4104d55214e9b0362a821edebbb261134c9bb8d9b424a6f38011`  
		Last Modified: Wed, 04 Mar 2020 03:48:39 GMT  
		Size: 5.6 MB (5632972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ff859a9ab72f7109b6dac1af178c111e6be4fbe8ebc043748ab165d9c1e7a9`  
		Last Modified: Wed, 04 Mar 2020 03:48:37 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6cb0006ecdf0039402d90ec34055159dbb373fbaacfed3e02746f118f25e44`  
		Last Modified: Wed, 04 Mar 2020 03:48:37 GMT  
		Size: 1.3 KB (1252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0.5` - linux; arm64 variant v8

```console
$ docker pull cirros@sha256:9bb5da8a0a43f0cfefcf107c9d5cf5f1d0f01765d6dca0822e86a652ccf9f484
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5381496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49c2d66f9f12684a5bade65fd1049d9a899db7a53eb8a7da9447c3a8142cdd4f`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Wed, 04 Mar 2020 03:39:43 GMT
ADD file:a6d30e587ca56c660bf6dbf0257c89cedf5a89286ac825e93a0d1c459c54bf83 in / 
# Wed, 04 Mar 2020 03:39:45 GMT
RUN rm /etc/rc3.d/S40-network
# Wed, 04 Mar 2020 03:39:46 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Wed, 04 Mar 2020 03:39:47 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:35df11b12919a3b9827938de4a8b55176c7ddfb2e87cf559858764365c885446`  
		Last Modified: Wed, 04 Mar 2020 03:39:57 GMT  
		Size: 5.4 MB (5380086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dea8baa8412c21524088511648c32018f230c913308eedbc28a617c5dfdad67`  
		Last Modified: Wed, 04 Mar 2020 03:39:56 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5aba0358242a35568239b5061a318455594ac21042fd7d5d8da9b5f6801de9`  
		Last Modified: Wed, 04 Mar 2020 03:39:56 GMT  
		Size: 1.3 KB (1252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0.5` - linux; 386

```console
$ docker pull cirros@sha256:3c6e16d674e697a07f5bc4bf73f08d8e0a48b6e7ddc6e0f54c5d84fbeeb6b61c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5531739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:579b6baca511fd54c70e57c3656d94412fb4f47fe2bfa3c10a7d703ca9f8a3be`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Wed, 04 Mar 2020 03:38:26 GMT
ADD file:73657d1d105210371bedeae4e7dc0f6ab1249c8c42ad729ef767e6b3a7fe4949 in / 
# Wed, 04 Mar 2020 03:38:27 GMT
RUN rm /etc/rc3.d/S40-network
# Wed, 04 Mar 2020 03:38:27 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Wed, 04 Mar 2020 03:38:27 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:e7bd3e7f87713723923da5ab89ee97e7e847d04dd11972c048f3e0755e332c0e`  
		Last Modified: Wed, 04 Mar 2020 03:38:35 GMT  
		Size: 5.5 MB (5530337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c84906c79e8b33dc47bc7fa6602d1520f2e376dcc0fb0cf216713157dfd99c2`  
		Last Modified: Wed, 04 Mar 2020 03:38:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9068d613cfb0f637131254136e0465d4a21a0b7373f225c5566a5ef4c262e0c`  
		Last Modified: Wed, 04 Mar 2020 03:38:34 GMT  
		Size: 1.2 KB (1248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0.5` - linux; ppc64le

```console
$ docker pull cirros@sha256:83fe7decf7e2cc1f13aa9d216474c7d772bacbc50cba23c3af9e4519408f100f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 MB (5770658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b99c3db42160238bcaef14a19800216c78cf5c7ed7c0afcbd4470e5a4531aca1`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Wed, 04 Mar 2020 03:31:30 GMT
ADD file:867dd84e8959e9f1f3647b5391e6b4dce42ecc772c47119403f54db588944783 in / 
# Wed, 04 Mar 2020 03:31:35 GMT
RUN rm /etc/rc3.d/S40-network
# Wed, 04 Mar 2020 03:31:42 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Wed, 04 Mar 2020 03:31:44 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:81fa53a9c824a2d73ef844702e11d5377598b64257721313c21413efb753ce9f`  
		Last Modified: Wed, 04 Mar 2020 03:31:59 GMT  
		Size: 5.8 MB (5769250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b1a63bab9311d7cd0bbcb9c4e92bf1e37b9e64202b4788d566b272de7a7774`  
		Last Modified: Wed, 04 Mar 2020 03:31:58 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfaba3b952f0078fbb6a55f105e7bc6d2e6ff0566346a0b8f909843e4f7fff8`  
		Last Modified: Wed, 04 Mar 2020 03:31:58 GMT  
		Size: 1.3 KB (1251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `cirros:0.5.0`

```console
$ docker pull cirros@sha256:477522da784f5b3c8e3d2c7cce37c6c00947f610be6ed5aa72e13dd95cdd68f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `cirros:0.5.0` - linux; amd64

```console
$ docker pull cirros@sha256:639af3aa2828aa4efa3e27b06857552fe2db74eed4bc107bedb23a6122493d21
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (5953477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8cf2b398779ae60d12d9372e5dbfb66c0ffaec0b0a246c697a266fffbf30a71`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Wed, 04 Mar 2020 03:19:36 GMT
ADD file:7dd645da025b829ce3a58eda283fd28cbb8ef5d018241a9e46d2f31702949d93 in / 
# Wed, 04 Mar 2020 03:19:37 GMT
RUN rm /etc/rc3.d/S40-network
# Wed, 04 Mar 2020 03:19:38 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Wed, 04 Mar 2020 03:19:38 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:3c4b29c44747d8ead42e1a03a594fa91e3950d2b3314e3ed2cf899ba13a38726`  
		Last Modified: Wed, 04 Mar 2020 03:19:48 GMT  
		Size: 6.0 MB (5952069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae1cdea52f92512f576ea638e421f7c9263d6134bea153fb8701a9ef6b6b7cc`  
		Last Modified: Wed, 04 Mar 2020 03:19:47 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bca7c60d756992600573a76c0459a7dbf42b6b3c293029de0d2d2b59732f2a5`  
		Last Modified: Wed, 04 Mar 2020 03:19:46 GMT  
		Size: 1.3 KB (1251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0.5.0` - linux; arm variant v5

```console
$ docker pull cirros@sha256:5613be73fa3d88979776d2e0f1ba9b90c3400f19002e419b4120cb06866403e3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.6 MB (5634381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e24ca8e4664d4bafb19195c2d34e52f6a8069ffe586269dcd2b0620aa75d6c4`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Wed, 04 Mar 2020 03:48:24 GMT
ADD file:f4f821b05b6cfb4f3fa31012adb331dd57c57d492fbe5a53a5deffa6026bfa0e in / 
# Wed, 04 Mar 2020 03:48:26 GMT
RUN rm /etc/rc3.d/S40-network
# Wed, 04 Mar 2020 03:48:27 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Wed, 04 Mar 2020 03:48:28 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:33e50245f4fc4104d55214e9b0362a821edebbb261134c9bb8d9b424a6f38011`  
		Last Modified: Wed, 04 Mar 2020 03:48:39 GMT  
		Size: 5.6 MB (5632972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ff859a9ab72f7109b6dac1af178c111e6be4fbe8ebc043748ab165d9c1e7a9`  
		Last Modified: Wed, 04 Mar 2020 03:48:37 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6cb0006ecdf0039402d90ec34055159dbb373fbaacfed3e02746f118f25e44`  
		Last Modified: Wed, 04 Mar 2020 03:48:37 GMT  
		Size: 1.3 KB (1252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0.5.0` - linux; arm64 variant v8

```console
$ docker pull cirros@sha256:9bb5da8a0a43f0cfefcf107c9d5cf5f1d0f01765d6dca0822e86a652ccf9f484
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5381496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49c2d66f9f12684a5bade65fd1049d9a899db7a53eb8a7da9447c3a8142cdd4f`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Wed, 04 Mar 2020 03:39:43 GMT
ADD file:a6d30e587ca56c660bf6dbf0257c89cedf5a89286ac825e93a0d1c459c54bf83 in / 
# Wed, 04 Mar 2020 03:39:45 GMT
RUN rm /etc/rc3.d/S40-network
# Wed, 04 Mar 2020 03:39:46 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Wed, 04 Mar 2020 03:39:47 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:35df11b12919a3b9827938de4a8b55176c7ddfb2e87cf559858764365c885446`  
		Last Modified: Wed, 04 Mar 2020 03:39:57 GMT  
		Size: 5.4 MB (5380086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dea8baa8412c21524088511648c32018f230c913308eedbc28a617c5dfdad67`  
		Last Modified: Wed, 04 Mar 2020 03:39:56 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5aba0358242a35568239b5061a318455594ac21042fd7d5d8da9b5f6801de9`  
		Last Modified: Wed, 04 Mar 2020 03:39:56 GMT  
		Size: 1.3 KB (1252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0.5.0` - linux; 386

```console
$ docker pull cirros@sha256:3c6e16d674e697a07f5bc4bf73f08d8e0a48b6e7ddc6e0f54c5d84fbeeb6b61c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5531739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:579b6baca511fd54c70e57c3656d94412fb4f47fe2bfa3c10a7d703ca9f8a3be`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Wed, 04 Mar 2020 03:38:26 GMT
ADD file:73657d1d105210371bedeae4e7dc0f6ab1249c8c42ad729ef767e6b3a7fe4949 in / 
# Wed, 04 Mar 2020 03:38:27 GMT
RUN rm /etc/rc3.d/S40-network
# Wed, 04 Mar 2020 03:38:27 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Wed, 04 Mar 2020 03:38:27 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:e7bd3e7f87713723923da5ab89ee97e7e847d04dd11972c048f3e0755e332c0e`  
		Last Modified: Wed, 04 Mar 2020 03:38:35 GMT  
		Size: 5.5 MB (5530337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c84906c79e8b33dc47bc7fa6602d1520f2e376dcc0fb0cf216713157dfd99c2`  
		Last Modified: Wed, 04 Mar 2020 03:38:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9068d613cfb0f637131254136e0465d4a21a0b7373f225c5566a5ef4c262e0c`  
		Last Modified: Wed, 04 Mar 2020 03:38:34 GMT  
		Size: 1.2 KB (1248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:0.5.0` - linux; ppc64le

```console
$ docker pull cirros@sha256:83fe7decf7e2cc1f13aa9d216474c7d772bacbc50cba23c3af9e4519408f100f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 MB (5770658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b99c3db42160238bcaef14a19800216c78cf5c7ed7c0afcbd4470e5a4531aca1`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Wed, 04 Mar 2020 03:31:30 GMT
ADD file:867dd84e8959e9f1f3647b5391e6b4dce42ecc772c47119403f54db588944783 in / 
# Wed, 04 Mar 2020 03:31:35 GMT
RUN rm /etc/rc3.d/S40-network
# Wed, 04 Mar 2020 03:31:42 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Wed, 04 Mar 2020 03:31:44 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:81fa53a9c824a2d73ef844702e11d5377598b64257721313c21413efb753ce9f`  
		Last Modified: Wed, 04 Mar 2020 03:31:59 GMT  
		Size: 5.8 MB (5769250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b1a63bab9311d7cd0bbcb9c4e92bf1e37b9e64202b4788d566b272de7a7774`  
		Last Modified: Wed, 04 Mar 2020 03:31:58 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfaba3b952f0078fbb6a55f105e7bc6d2e6ff0566346a0b8f909843e4f7fff8`  
		Last Modified: Wed, 04 Mar 2020 03:31:58 GMT  
		Size: 1.3 KB (1251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `cirros:latest`

```console
$ docker pull cirros@sha256:477522da784f5b3c8e3d2c7cce37c6c00947f610be6ed5aa72e13dd95cdd68f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `cirros:latest` - linux; amd64

```console
$ docker pull cirros@sha256:639af3aa2828aa4efa3e27b06857552fe2db74eed4bc107bedb23a6122493d21
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (5953477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8cf2b398779ae60d12d9372e5dbfb66c0ffaec0b0a246c697a266fffbf30a71`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Wed, 04 Mar 2020 03:19:36 GMT
ADD file:7dd645da025b829ce3a58eda283fd28cbb8ef5d018241a9e46d2f31702949d93 in / 
# Wed, 04 Mar 2020 03:19:37 GMT
RUN rm /etc/rc3.d/S40-network
# Wed, 04 Mar 2020 03:19:38 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Wed, 04 Mar 2020 03:19:38 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:3c4b29c44747d8ead42e1a03a594fa91e3950d2b3314e3ed2cf899ba13a38726`  
		Last Modified: Wed, 04 Mar 2020 03:19:48 GMT  
		Size: 6.0 MB (5952069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae1cdea52f92512f576ea638e421f7c9263d6134bea153fb8701a9ef6b6b7cc`  
		Last Modified: Wed, 04 Mar 2020 03:19:47 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bca7c60d756992600573a76c0459a7dbf42b6b3c293029de0d2d2b59732f2a5`  
		Last Modified: Wed, 04 Mar 2020 03:19:46 GMT  
		Size: 1.3 KB (1251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:latest` - linux; arm variant v5

```console
$ docker pull cirros@sha256:5613be73fa3d88979776d2e0f1ba9b90c3400f19002e419b4120cb06866403e3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.6 MB (5634381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e24ca8e4664d4bafb19195c2d34e52f6a8069ffe586269dcd2b0620aa75d6c4`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Wed, 04 Mar 2020 03:48:24 GMT
ADD file:f4f821b05b6cfb4f3fa31012adb331dd57c57d492fbe5a53a5deffa6026bfa0e in / 
# Wed, 04 Mar 2020 03:48:26 GMT
RUN rm /etc/rc3.d/S40-network
# Wed, 04 Mar 2020 03:48:27 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Wed, 04 Mar 2020 03:48:28 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:33e50245f4fc4104d55214e9b0362a821edebbb261134c9bb8d9b424a6f38011`  
		Last Modified: Wed, 04 Mar 2020 03:48:39 GMT  
		Size: 5.6 MB (5632972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ff859a9ab72f7109b6dac1af178c111e6be4fbe8ebc043748ab165d9c1e7a9`  
		Last Modified: Wed, 04 Mar 2020 03:48:37 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6cb0006ecdf0039402d90ec34055159dbb373fbaacfed3e02746f118f25e44`  
		Last Modified: Wed, 04 Mar 2020 03:48:37 GMT  
		Size: 1.3 KB (1252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:latest` - linux; arm64 variant v8

```console
$ docker pull cirros@sha256:9bb5da8a0a43f0cfefcf107c9d5cf5f1d0f01765d6dca0822e86a652ccf9f484
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5381496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49c2d66f9f12684a5bade65fd1049d9a899db7a53eb8a7da9447c3a8142cdd4f`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Wed, 04 Mar 2020 03:39:43 GMT
ADD file:a6d30e587ca56c660bf6dbf0257c89cedf5a89286ac825e93a0d1c459c54bf83 in / 
# Wed, 04 Mar 2020 03:39:45 GMT
RUN rm /etc/rc3.d/S40-network
# Wed, 04 Mar 2020 03:39:46 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Wed, 04 Mar 2020 03:39:47 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:35df11b12919a3b9827938de4a8b55176c7ddfb2e87cf559858764365c885446`  
		Last Modified: Wed, 04 Mar 2020 03:39:57 GMT  
		Size: 5.4 MB (5380086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dea8baa8412c21524088511648c32018f230c913308eedbc28a617c5dfdad67`  
		Last Modified: Wed, 04 Mar 2020 03:39:56 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5aba0358242a35568239b5061a318455594ac21042fd7d5d8da9b5f6801de9`  
		Last Modified: Wed, 04 Mar 2020 03:39:56 GMT  
		Size: 1.3 KB (1252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:latest` - linux; 386

```console
$ docker pull cirros@sha256:3c6e16d674e697a07f5bc4bf73f08d8e0a48b6e7ddc6e0f54c5d84fbeeb6b61c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5531739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:579b6baca511fd54c70e57c3656d94412fb4f47fe2bfa3c10a7d703ca9f8a3be`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Wed, 04 Mar 2020 03:38:26 GMT
ADD file:73657d1d105210371bedeae4e7dc0f6ab1249c8c42ad729ef767e6b3a7fe4949 in / 
# Wed, 04 Mar 2020 03:38:27 GMT
RUN rm /etc/rc3.d/S40-network
# Wed, 04 Mar 2020 03:38:27 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Wed, 04 Mar 2020 03:38:27 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:e7bd3e7f87713723923da5ab89ee97e7e847d04dd11972c048f3e0755e332c0e`  
		Last Modified: Wed, 04 Mar 2020 03:38:35 GMT  
		Size: 5.5 MB (5530337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c84906c79e8b33dc47bc7fa6602d1520f2e376dcc0fb0cf216713157dfd99c2`  
		Last Modified: Wed, 04 Mar 2020 03:38:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9068d613cfb0f637131254136e0465d4a21a0b7373f225c5566a5ef4c262e0c`  
		Last Modified: Wed, 04 Mar 2020 03:38:34 GMT  
		Size: 1.2 KB (1248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `cirros:latest` - linux; ppc64le

```console
$ docker pull cirros@sha256:83fe7decf7e2cc1f13aa9d216474c7d772bacbc50cba23c3af9e4519408f100f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 MB (5770658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b99c3db42160238bcaef14a19800216c78cf5c7ed7c0afcbd4470e5a4531aca1`
-	Default Command: `["\/sbin\/init"]`

```dockerfile
# Wed, 04 Mar 2020 03:31:30 GMT
ADD file:867dd84e8959e9f1f3647b5391e6b4dce42ecc772c47119403f54db588944783 in / 
# Wed, 04 Mar 2020 03:31:35 GMT
RUN rm /etc/rc3.d/S40-network
# Wed, 04 Mar 2020 03:31:42 GMT
RUN sed -i '/is_lxc && lxc_netdown/d' /etc/init.d/rc.sysinit
# Wed, 04 Mar 2020 03:31:44 GMT
CMD ["/sbin/init"]
```

-	Layers:
	-	`sha256:81fa53a9c824a2d73ef844702e11d5377598b64257721313c21413efb753ce9f`  
		Last Modified: Wed, 04 Mar 2020 03:31:59 GMT  
		Size: 5.8 MB (5769250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b1a63bab9311d7cd0bbcb9c4e92bf1e37b9e64202b4788d566b272de7a7774`  
		Last Modified: Wed, 04 Mar 2020 03:31:58 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfaba3b952f0078fbb6a55f105e7bc6d2e6ff0566346a0b8f909843e4f7fff8`  
		Last Modified: Wed, 04 Mar 2020 03:31:58 GMT  
		Size: 1.3 KB (1251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
