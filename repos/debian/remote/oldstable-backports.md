## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:abb7ddeb021bbfdffa20652da466dd8600769931d7c479de0d0a432f362e8dd4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:oldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:0b9eae254f0260b41445b1eef4e0007acadceeb754764bd72cda816aa5745480
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50449105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7b690b953983462eb2f35ddc27c5a60aff34878c46377d16ebdbf7408e6f157`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:21:01 GMT
ADD file:1bea2b449a4ce132efd49fc55676c9345122a3e6bf2fd8d222973421e97cd543 in / 
# Wed, 21 Dec 2022 01:21:02 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:21:05 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4c345612f93e3101d36e5006b7f417ee9fb655c3fc10e30726108dcebc0b9c0d`  
		Last Modified: Wed, 21 Dec 2022 01:25:36 GMT  
		Size: 50.4 MB (50448879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc204c1ab4ce867ef76c493801ea75a00b95d5990d37f9a6217429ba64d17eb`  
		Last Modified: Wed, 21 Dec 2022 01:25:45 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:413fbc091720a8bb3a3a8c3266756470e993f4eacdd8c5860c33968d434abc87
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45915701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d40b62f7f83a156426fba5d4e8965e1c2348a9f376726034efca40834960bdcb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 00:59:42 GMT
ADD file:8fd8cda825c15d02c34973f7dfe0bafbea6ef65a0da663aca1b55045c69ccec2 in / 
# Tue, 06 Dec 2022 00:59:44 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 00:59:50 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:fd8e272c3a0dda2db4eee10dc4e8689e197689318a4b437c03fa2bd86320c10a`  
		Last Modified: Tue, 06 Dec 2022 01:07:20 GMT  
		Size: 45.9 MB (45915477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67cba2b746456dfbfbecc63c475978134a4a5bb9705630eeac2712ce9c8387c0`  
		Last Modified: Tue, 06 Dec 2022 01:07:31 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:bcf6b10cfcb1bbda0ebef66ac9790563a6bd6e996f11b7027f0c003b328c0424
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49233966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32f4da0d89a0630e00ddd50383ef126d54b15367febbc7021194824340c8e4af`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:42 GMT
ADD file:5aac487e8a98792f9d26b35326907f53704c9f811b66dd80ecda79bcf26e038e in / 
# Tue, 06 Dec 2022 01:40:42 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:40:45 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:85694686675a17bb196654e718ec16a7bf7e702ae4c2e71c29087c823c0b57cb`  
		Last Modified: Tue, 06 Dec 2022 01:44:50 GMT  
		Size: 49.2 MB (49233741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5666a58ef5eae2b3df72343925a6ce7285e716033fca3fe165e4f6d4a3e2e1d`  
		Last Modified: Tue, 06 Dec 2022 01:44:58 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:a4057a5884e1e45f63ed2515ed1e0a633daf02be229792ec5f181483ce1e81d2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51207927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ad723831e66a49a43462179012c55ea9753d6eed895e56da7272adaa14c6f17`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:35 GMT
ADD file:f50f5fb1adc41d77fc4e09c5fbdc62f13f6c9cd04fb456bddf5d566616c27435 in / 
# Tue, 06 Dec 2022 01:40:35 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:40:41 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:205b92520f738bc7f38ac65b79b80c7f5cdb162c0a5f98b53d284ebaa510b475`  
		Last Modified: Tue, 06 Dec 2022 01:46:48 GMT  
		Size: 51.2 MB (51207703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17ef8dc4d3afe64f286b4a525407db2519bff35c4a290a7e570f0edfc1f6b3d`  
		Last Modified: Tue, 06 Dec 2022 01:46:58 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
