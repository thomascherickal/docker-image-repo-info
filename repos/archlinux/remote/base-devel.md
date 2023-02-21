## `archlinux:base-devel`

```console
$ docker pull archlinux@sha256:6aa7aa450a7bfa4f6777c990a67d2ff72f5fabd9b155ad7730b4728a3b4643fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `archlinux:base-devel` - linux; amd64

```console
$ docker pull archlinux@sha256:f2c6b88b2670f2fd3b5d665765a72d5983bf06779e22a68aec6f4c58d3789390
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.2 MB (245197784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eac87022dd6c9e34707dfab60e97d56e529c2c2bc98abee9e2553c5f6e508c10`
-	Default Command: `["\/usr\/bin\/bash"]`

```dockerfile
# Tue, 21 Feb 2023 20:21:31 GMT
COPY dir:aace1ea4a97e8cc063bcaa6af1959fd35456b8ddfcca27555554c9977068e144 in / 
# Tue, 21 Feb 2023 20:21:34 GMT
RUN ldconfig &&     sed -i '/BUILD_ID/a VERSION_ID=TEMPLATE_VERSION_ID' /etc/os-release
# Tue, 21 Feb 2023 20:21:34 GMT
ENV LANG=C.UTF-8
# Tue, 21 Feb 2023 20:21:34 GMT
CMD ["/usr/bin/bash"]
```

-	Layers:
	-	`sha256:c3dabff4be84df8174e4eac4a3a42d1642a96f0ff8301c049582a0e0138a7e2e`  
		Last Modified: Tue, 21 Feb 2023 20:22:59 GMT  
		Size: 245.2 MB (245189084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe54bbe0e9ebdd37438439cfc485ddc7a27dc0146e9b1202742e7e8a34afadb6`  
		Last Modified: Tue, 21 Feb 2023 20:22:26 GMT  
		Size: 8.7 KB (8700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
