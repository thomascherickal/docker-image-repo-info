## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:c49fd49d868b56f1454f7734a3bfdc5b502cdd80963f669458251b146e4b4cd0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:1070545f3003036660f858836efcf7b089f5f33c9c3da98c664e5d6303957a50
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **476.8 MB (476758547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:712d2767ea76ecb265150bae981829b198c60d9ce3fbef60ef2fe247219c0ff3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Apr 2020 18:22:56 GMT
ADD file:c64a7d77d1e9f4364c8d2009059cb8668697d61f54f457215b6be6f0c9cded5b in / 
# Tue, 21 Apr 2020 18:22:56 GMT
CMD ["/bin/bash"]
# Tue, 21 Apr 2020 18:23:21 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-44ab891c498d922bb21e90b6006b12c7f05381ec7e67aba05bb535aae3b261b1.tar.gz"  && echo "a1b70378c6175331c9daa5bee79c8cb36dab14ed1fb0d02bfd33254652f0b846  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:a3f8e652bdc470bbea38766fe41f8f12b9e4d44e9ce4037eb502839754b06b9c`  
		Last Modified: Tue, 21 Apr 2020 18:23:48 GMT  
		Size: 61.6 MB (61619066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85b52563080715b3858df242f64ffaa92212a60bfd97b7e9e9bd506b80663b2`  
		Last Modified: Tue, 21 Apr 2020 18:24:16 GMT  
		Size: 415.1 MB (415139481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:with-sources` - linux; arm64 variant v8

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
