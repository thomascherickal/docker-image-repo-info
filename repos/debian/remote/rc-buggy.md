## `debian:rc-buggy`

```console
$ docker pull debian@sha256:a29a061efe59e1f5175972684e56240ae3a597dc35b9a52b6b47671c0d074dd0
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

### `debian:rc-buggy` - linux; amd64

```console
$ docker pull debian@sha256:b878ce38bb4b70ab3b45920de342b00931c41e677e02d0e6fad38ba273397cd6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52488318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fec7128bee529054d2e1e1964c42bb1ddce228924e5248256aa31892340d2267`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 00:28:02 GMT
ADD file:d09d72986a18210fc325abfbe18d3d35fef6de8ede47304410bea7528e5ab5e6 in / 
# Thu, 10 Sep 2020 00:28:02 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:32:17 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:5da2bf34dd483faff62b98f29a31447619812af8afb0cdee07c188e866571393`  
		Last Modified: Thu, 10 Sep 2020 00:35:58 GMT  
		Size: 52.5 MB (52488092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251d7dbd2f5b88c7c8d0ad4a40b0cb187dd681db606e83eb00b93d67a3d28ae1`  
		Last Modified: Thu, 10 Sep 2020 00:38:53 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v5

```console
$ docker pull debian@sha256:fd16f9f794e8e296356364bc36c2115e8dfc1fc117228d85e22164609cb71b3c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50413770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ac11ec470495fe3768ec3c463c9a4acaa05048010c87ca7b02d25335496f013`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:56:41 GMT
ADD file:9c8616d4fabe6861a7f03ec7c1849957393374004adaf865fad27fc7e91057dc in / 
# Wed, 09 Sep 2020 23:56:44 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:00:41 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:dd8dd816178223393e19e5b2cd1f62df2d94bc6d5c9c393d8da9f901c96e3f93`  
		Last Modified: Thu, 10 Sep 2020 00:05:28 GMT  
		Size: 50.4 MB (50413542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be15ff42ba202309374f9e7705cd94247f0e764b799e078b44b8a1c6acb9ea7`  
		Last Modified: Thu, 10 Sep 2020 00:08:53 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v7

```console
$ docker pull debian@sha256:49084764c622b965baa3e41265438d7f3768f69e50deb60c7541e8d295558fad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48157046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1aa53c969d91f8863e117a7f8f8bf296a6c18a1c644c2f73371a6a489357d0a2`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 00:11:28 GMT
ADD file:23fbc90316c23c82a8b8da300c8a5623fc3db73c430d1cbdbfab09ab920a25cf in / 
# Thu, 10 Sep 2020 00:11:29 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:15:57 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:d4d2daf5b278e6cc19610d2a52a8745b441acb4d3e087f6cc35aff05d6ce2a0d`  
		Last Modified: Thu, 10 Sep 2020 00:20:05 GMT  
		Size: 48.2 MB (48156817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ed420092d135ff742d16d0ae21de55db35c23583fe65d4a1e14c848ea97d82`  
		Last Modified: Thu, 10 Sep 2020 00:23:01 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:c35971a3b734fb216dd85cd2194ce64fcd70d37bb26701050b24781cdf8f9aa9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.8 MB (50845481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1d199fe90dda4925b63371b7e98c0a66b762666d3d876d8dd1e355e6245f2b6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:52:18 GMT
ADD file:0b10d18375e8cd004468a07659e73e4afcd826f2808314dcc8fbb6b773c3ed6a in / 
# Wed, 09 Sep 2020 23:52:28 GMT
CMD ["bash"]
# Wed, 09 Sep 2020 23:57:14 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:21fc4451f3aee8da37deddc4046fa3dd8ea41b5a39481b93c43bc5dd385277d5`  
		Last Modified: Thu, 10 Sep 2020 00:00:09 GMT  
		Size: 50.8 MB (50845252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d450450b8e308c2280c3582e9be1a75428337030d6ce52ba4dfd4b7b04f091`  
		Last Modified: Thu, 10 Sep 2020 00:03:45 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; 386

```console
$ docker pull debian@sha256:b47fd49365b62339a0533dcdba017b2598659f5f8186e08f2306c6e6576e340b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53575195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16c0684e64fdc779330068e2cc414b110a812dc1a5bf3f15f66bd0d60bce1b59`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:42:20 GMT
ADD file:0f16119ad5399bd128cd02055185b1f534348a2ea02757438ace9e8b088822c2 in / 
# Wed, 09 Sep 2020 23:42:21 GMT
CMD ["bash"]
# Wed, 09 Sep 2020 23:45:09 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:9cf7fbf089a5c33a8981bcf78f935777e9a0e1340c0526fbe21a102ede6f5a74`  
		Last Modified: Wed, 09 Sep 2020 23:48:07 GMT  
		Size: 53.6 MB (53574966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ecae0a38c5122c89130f7bdcd5fb66bf04a800c4e928de364b0a28df8087ea`  
		Last Modified: Wed, 09 Sep 2020 23:50:12 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; mips64le

```console
$ docker pull debian@sha256:bc436eeeb181a922c8fafe8f9a0de2f969a4525a425347d78e19992860bc1750
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51146905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:659796ec33fc3cd68a4d9db8c32790d3e9cdaee6d849b01469f4483f202d3ac1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:42:49 GMT
ADD file:c8977e04a216367623fcae06b950449d648b73fe2ebfeea8ac4d43b825fd9072 in / 
# Tue, 04 Aug 2020 06:42:50 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 06:45:37 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:d1b4f7d45a45e5da796e6015b373bab6d97853967e128d506ed0b95683b889a2`  
		Last Modified: Tue, 04 Aug 2020 06:49:31 GMT  
		Size: 51.1 MB (51146678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d840d0452d6c3fc0df5c751aa43af285212dbc8a8ed03b77612dbe65b35ebb`  
		Last Modified: Tue, 04 Aug 2020 06:54:25 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; ppc64le

```console
$ docker pull debian@sha256:3c624e5174c7da7fb5468d1cb06a682b110bd771c9e914e47878a42638fab6cf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.3 MB (56336916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe959250f77550b2e6f691defd0aef025da11c3a6d181977012b3b31c158c3ef`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 01:06:51 GMT
ADD file:6525cb187fc85a4741e9d9de398149d93f43e196e99a20d48f165a25a1a8f36e in / 
# Thu, 10 Sep 2020 01:07:08 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 01:21:07 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:184155505be08ee96b6e64926098f03c472ad33bae3d34b8f683480960d7b5d6`  
		Last Modified: Thu, 10 Sep 2020 01:30:22 GMT  
		Size: 56.3 MB (56336687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17fca0efd2d3c8248e41756e7d4ade3e4ee6e3783300c914c3877dad6eb16293`  
		Last Modified: Thu, 10 Sep 2020 01:42:21 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; s390x

```console
$ docker pull debian@sha256:50afb61c85c16c5f78a1db731ef1dd6fa7952cc48e67e9659c99febd856bb13e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51061220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f831c91f36767846c23402afafbed0b3d78fb63b14aca1353a0ca197302eafa1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:42:52 GMT
ADD file:8cf459b787b06e517199d5538d4a79b845b7b7d72ccf10fffdee5a385c0895bd in / 
# Wed, 09 Sep 2020 23:42:57 GMT
CMD ["bash"]
# Wed, 09 Sep 2020 23:45:20 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:0777a1517003dde2e616b494a11a7867f55924ffac710d8d2c15b7b50fbeea1d`  
		Last Modified: Wed, 09 Sep 2020 23:46:42 GMT  
		Size: 51.1 MB (51060992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac77f806c52b3d09b7878243f35d7256b0e606b1f73648bc6f47fbff6f5fb82`  
		Last Modified: Wed, 09 Sep 2020 23:48:14 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
