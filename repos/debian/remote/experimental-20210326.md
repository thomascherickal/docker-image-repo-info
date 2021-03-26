## `debian:experimental-20210326`

```console
$ docker pull debian@sha256:8ca57102cd10e96b6b5e3fd836d9fbdbd875702ebcbd1a45eec6566db7e53f5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v5
	-	linux; mips64le

### `debian:experimental-20210326` - linux; arm variant v5

```console
$ docker pull debian@sha256:e6a9dfb39feb4fd4dda653c0a314139016da9f96eb63ad81fb138789232b8869
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.4 MB (52402643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20ecf2885ec922297062365506f6d406c87094025e7d94466c6c9c135ed67dc8`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 07:57:13 GMT
ADD file:32612d584d6e838fda991bcee065f36db394c6848444220ab925641eed015030 in / 
# Fri, 26 Mar 2021 07:57:16 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 07:57:40 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:ea6af2ab5e68178d221322a9de282a1dc71dad081d87e92a0861e9cbd6b706cd`  
		Last Modified: Fri, 26 Mar 2021 08:05:41 GMT  
		Size: 52.4 MB (52402421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa483613c27c2a61b6db5546785369669d2578b1680819499ead7e37599ec18`  
		Last Modified: Fri, 26 Mar 2021 08:06:04 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20210326` - linux; mips64le

```console
$ docker pull debian@sha256:f8a69b4993283e7f37546958ca36a488ea80857d996f3f278dfb7676f2fa5feb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53127031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8367223de90e6e5ed6869860066c83594e0cf319b09af633fa8cb3bb30d322bb`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 08:12:45 GMT
ADD file:c79a17a0f871c489c33a2d475b8e5371996f90bbc7760e45557108da54e86545 in / 
# Fri, 26 Mar 2021 08:12:46 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 08:13:10 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:75c364cc452cddccfec518752d444a6600aed010f6c6fb415dd2924ecd097fa8`  
		Last Modified: Fri, 26 Mar 2021 08:21:20 GMT  
		Size: 53.1 MB (53126809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee942771ebd98062575efc7cc7107c8dc519eee1e1d12981ade8d08be4bc8a5`  
		Last Modified: Fri, 26 Mar 2021 08:22:01 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
