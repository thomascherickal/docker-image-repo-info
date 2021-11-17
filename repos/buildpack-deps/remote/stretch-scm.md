## `buildpack-deps:stretch-scm`

```console
$ docker pull buildpack-deps@sha256:248d31934f42c9e18a18cc666a6eed8783f69f0ad7ddbb94e101d9a1f7c1ff3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:stretch-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:b0f76319830edb0ebac43cd1e76a4c2a5d34e847b9bb3f7371bbfebe57eb205f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.8 MB (110786547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cea98b6e932cedec41f17989129c68a1bd3d343c834ab1c992efb3bc8544888`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:28 GMT
ADD file:d7365dd9cf34b10ca189f85c95c21a0c33e44092f85ffb5884d5e737fb0b9be1 in / 
# Wed, 17 Nov 2021 02:22:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:19:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:19:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:19:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:200cae5c9d88bb9cf1dd3fcfb831d671403f078d2310416fa3b304337d8279c0`  
		Last Modified: Wed, 17 Nov 2021 02:29:09 GMT  
		Size: 45.4 MB (45380444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047156b8adafd241846cd5539cebd45e6e28fe1bd818cd654a0124cef61d4cb2`  
		Last Modified: Wed, 17 Nov 2021 03:27:27 GMT  
		Size: 11.3 MB (11301447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cbf304dd51feb48b321b93ae5b8a5a6ca55c23b51a8dc0d9642c3c3b5081a7`  
		Last Modified: Wed, 17 Nov 2021 03:27:26 GMT  
		Size: 4.3 MB (4342326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6e9db633dd66ac91ed2df32c5900c5a1ae82b58cc9261fd240913743d283ca`  
		Last Modified: Wed, 17 Nov 2021 03:27:45 GMT  
		Size: 49.8 MB (49762330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:3b6dcef1865cc1d9df51cfcede2b22a42810d59e1ed7f2dd6f1a2afdab2da382
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.6 MB (106589552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f1b47c4fc7cd09da1eadb373e1b3639dd3ea6f0d0a7f277a6f9a3a1badf1916`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:55:37 GMT
ADD file:eb65cc31f82e76c4ea5a8f21e4cad1372399517ee41a759740ff91d1d23b9e44 in / 
# Tue, 12 Oct 2021 00:55:38 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:54:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:54:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 05:55:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d2f67fd5897d122073fc9ad347c1fb9faec31555c47b3ee6ff64ca2b553034ed`  
		Last Modified: Tue, 12 Oct 2021 01:13:31 GMT  
		Size: 44.1 MB (44091932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b4f8f4eb65e840d4778dd2e77e7cc6d546cbd55ed717e53e017c853e7c07d1`  
		Last Modified: Tue, 12 Oct 2021 06:12:15 GMT  
		Size: 10.4 MB (10351740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec0c01cd7d7e35fbb8d775a4bca6166749569cbf3c1bc4b9a5aee530bff8978`  
		Last Modified: Tue, 12 Oct 2021 06:12:12 GMT  
		Size: 4.2 MB (4161429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb3ac8456e186fb75e7aaf1c21260430344e8cf1d6cd6fdaec9bfb9ab5a0741`  
		Last Modified: Tue, 12 Oct 2021 06:12:58 GMT  
		Size: 48.0 MB (47984451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:06b12ba3a191d0ec83b7588cd9cb7e94e5206746fe70cef1b57974f1c21f5097
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102120397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c01627a3706745a8b4f9600a77ff4453ce771391c424dff9199dbdfbec858c24`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:04:57 GMT
ADD file:61da3fcef3aea99b4927189cfcb823a65b0e911a3f4436e44ea84a57a7919ff3 in / 
# Wed, 17 Nov 2021 02:04:58 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:54:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:54:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 02:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4d54b576c2fcdd259e57bac14c4e1a2623f6e5dc9a0b1facaed7fe59d891e86`  
		Last Modified: Wed, 17 Nov 2021 02:22:03 GMT  
		Size: 42.1 MB (42116868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf04dd2447fcded30a4c9a8d7a054ccb2e4c4db4118989ea05bf2e56d60a8924`  
		Last Modified: Wed, 17 Nov 2021 03:14:24 GMT  
		Size: 10.0 MB (9956153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b37c8e78d6ca4f8e5467e0ec7ef61eef6101e99c8154472df98aa34159f5974`  
		Last Modified: Wed, 17 Nov 2021 03:14:21 GMT  
		Size: 3.9 MB (3921214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fcf28009119cc468ce87b98d583e8c51d3703937d10d502a704f1032bc2b26`  
		Last Modified: Wed, 17 Nov 2021 03:15:08 GMT  
		Size: 46.1 MB (46126162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:03b045b323b4d1f4cede5be2b001396f538505d8fdf27e9ea5d17476c965adad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105000402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:125f44db114ce9de480b682857aee2528e9db2f73f69805d347221b0accaa8ce`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:43:16 GMT
ADD file:33c2886dff8a69edd550eb69499bf01658d58e2eff405d4b5d4cd5d5be535faa in / 
# Tue, 12 Oct 2021 01:43:16 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:03:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:03:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 03:03:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd2a530f50c2591d61de58d0e9cf724f6c5a2e1112456f38562e289732464c0c`  
		Last Modified: Tue, 12 Oct 2021 01:52:05 GMT  
		Size: 43.2 MB (43176697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607051b9b8b0e248adc1dbae78b910c62d134181c4945e4df5e165ba533f7dea`  
		Last Modified: Sat, 16 Oct 2021 03:18:13 GMT  
		Size: 10.2 MB (10216060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c91f590ca18c241c146cf6ad6fb66517634bedc0681afcc69d37ee25828046`  
		Last Modified: Sat, 16 Oct 2021 03:18:12 GMT  
		Size: 3.9 MB (3873851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e454b57055514895812b6c056855e692fa41c1c6c1ba7f0cf0a57c78e9a0b8c`  
		Last Modified: Sat, 16 Oct 2021 03:18:31 GMT  
		Size: 47.7 MB (47733794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:3dd7dfec75397dae002735d04557b86aaaf641dbf609cd11f267f7740392d841
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.3 MB (113285816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10424f2f9fa56c237f5a1cb67f32e5286a03841b408bf07e8c6d4f87b5757030`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:42:19 GMT
ADD file:5a6f08cc731f24357c3702231256fb05eb0a97733779b2ace406ba3c9bf64baa in / 
# Tue, 12 Oct 2021 01:42:19 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:42:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:42:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 04:43:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d2ef4e90cca7406b4907a34e3571153fc56e3ecc9b2b5fdbb7787f22877cfec5`  
		Last Modified: Tue, 12 Oct 2021 01:51:58 GMT  
		Size: 46.1 MB (46097164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9020db84c7cf31b7929c21a2b6fe2123900e91c7391ad6f4ee5560a934f382`  
		Last Modified: Tue, 12 Oct 2021 04:52:49 GMT  
		Size: 11.4 MB (11358857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8cbe9196a8b6bd3825445c718bc5a248b7c295b4d9f45756819e8bf27cb72b`  
		Last Modified: Tue, 12 Oct 2021 04:52:47 GMT  
		Size: 4.6 MB (4565012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7454f0fe0ebf5d024897d682d46181ab978a980f7f40caa2492a83cc39f75ec`  
		Last Modified: Tue, 12 Oct 2021 04:53:20 GMT  
		Size: 51.3 MB (51264783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
