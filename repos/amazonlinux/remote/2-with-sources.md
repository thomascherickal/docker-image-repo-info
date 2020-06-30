## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:fdf45395e6e6ee2e6fc5cd412c489015a8b9b29df656858b326f3c66f2230671
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:420d5d3cfb86d4e124377ab32bc6f9e1504a07d63c0fff4282c49aa7c436c9ec
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **476.9 MB (476922148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d80a4bcf0ffd4b139a9c3d2390bb8b6aa5e6b6aeecef63d6934d908bcde98229`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Jun 2020 20:20:04 GMT
ADD file:788af9048b1c163347d7a8349f8ecf5721b4d8b63395ec8c6ca6d0732f57acdd in / 
# Tue, 30 Jun 2020 20:20:05 GMT
CMD ["/bin/bash"]
# Tue, 30 Jun 2020 20:20:29 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-9af89b3a0cae0f976ef3a0f7b0a0568f88bb8a6a99cb0b19d4c75a7af24fdd7d.tar.gz"  && echo "3d1d16d828b58c8855a5899401da4cbf47e3096cbf2bd798d9a690b9021e2326  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:3d24604292f287c31563b1f563e83307e7915909506659401fb07c1c3e6e164c`  
		Last Modified: Tue, 30 Jun 2020 20:21:31 GMT  
		Size: 61.7 MB (61684682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b36c1db94ea96b1c9c9ff14be0be653f85063ac10bae9324bc5545309ee7fd`  
		Last Modified: Tue, 30 Jun 2020 20:22:34 GMT  
		Size: 415.2 MB (415237466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:4cbc0732124bed6fdb615eaf60c2d4bb7cc134d957d1f9674dc0066a438ce1bc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **478.2 MB (478219309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aca4e24672d702283a87cbf97240f20bed3724d62ff8f8dcfb9a0baed82da19a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Apr 2020 18:58:16 GMT
ADD file:85fc0908f460f80c41755d2b5ab9ff6a025bb2726628ccc4edceb21d2e3f8edf in / 
# Tue, 21 Apr 2020 18:58:18 GMT
CMD ["/bin/bash"]
# Tue, 21 Apr 2020 18:59:09 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-44ab891c498d922bb21e90b6006b12c7f05381ec7e67aba05bb535aae3b261b1.tar.gz"  && echo "a1b70378c6175331c9daa5bee79c8cb36dab14ed1fb0d02bfd33254652f0b846  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:0a37a5cd26f245ce54aff575389ef7765520d37d3ea7c437144c936c6adffc8a`  
		Last Modified: Tue, 21 Apr 2020 18:59:54 GMT  
		Size: 63.1 MB (63079760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4f9d710835018ff01a17ccc9e3b4ce18e9cf9f81a0dc1cf8d455472d9a1d29`  
		Last Modified: Tue, 21 Apr 2020 19:00:52 GMT  
		Size: 415.1 MB (415139549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
