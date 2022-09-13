## `debian:experimental-20220912`

```console
$ docker pull debian@sha256:b29f529256633725553e5c82a09a75ed9272789d481325920c1caa9b4b10865e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; s390x

### `debian:experimental-20220912` - linux; amd64

```console
$ docker pull debian@sha256:b543cd094edd0c9271c9b5fca680344af2fc418a057b0d63276b7e07cfa744f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.6 MB (52643827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8726d4a11d5a96a53b643c2295a1091d3ab5e77655e107f20885a1950835405a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:58:12 GMT
ADD file:6ddd5244833a0a8b71e79b85b68064bd5b09f430b1b0ed8db07d6855ad470c39 in / 
# Tue, 13 Sep 2022 00:58:12 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 00:58:23 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:d48fb30607a31176a332991b7110d4b196c3564594e7aab632b9662094ec885a`  
		Last Modified: Tue, 13 Sep 2022 01:03:54 GMT  
		Size: 52.6 MB (52643603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8feed5ae45c9f1637fd673679cd602a43eda6d5645f8656d5220cb52bd1cd905`  
		Last Modified: Tue, 13 Sep 2022 01:04:17 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20220912` - linux; arm variant v5

```console
$ docker pull debian@sha256:92cef5e5007a0834e3ff2301cad38e5fa5ffaa802f02bd29642f4170f15d3b66
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51786153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89292022e7fa88d2015b754dd03457cbe7a8b265b040d276bc7042b5b32623eb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:16 GMT
ADD file:e7ec9bef12457f73465a8b9b0d10d2ee3fdcf244d19625f58ba4ffc2fcab0a1d in / 
# Tue, 13 Sep 2022 00:56:17 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 00:56:42 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:2ea2e84f45a0dfa7c04aa60a28b638e9696ca74b5f08fff59842aa2fadadbc5e`  
		Last Modified: Tue, 13 Sep 2022 01:04:36 GMT  
		Size: 51.8 MB (51785933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e1d1040164c9b35fe18a10cf8b6b71419e3fad3fb828ca0d3e407b584c0818`  
		Last Modified: Tue, 13 Sep 2022 01:05:10 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20220912` - linux; s390x

```console
$ docker pull debian@sha256:5be8b87514dd868479dc2731fda809a9f08f777df173fcb0af703500e4eb3f5c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51537223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f517eb61c1d8e9b97f0c76d87e074b3f23f21666d093fd138daffee9db97d66b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:49:41 GMT
ADD file:218a929c0b84eeef4dd935bbc23ec1a4c9fc02f06cf5c86ca6c8e94e78c5f927 in / 
# Tue, 13 Sep 2022 00:49:44 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 00:50:04 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:ee6e329c518cbd235ab8d38fbd5ffb98ffe45bfb2874fa69e7084eb6ecd09ca1`  
		Last Modified: Tue, 13 Sep 2022 00:54:17 GMT  
		Size: 51.5 MB (51537001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e60677fa0219710676fe7d6c382b68d19f4d901be63afc7e617ba536f3dea5`  
		Last Modified: Tue, 13 Sep 2022 00:54:34 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
