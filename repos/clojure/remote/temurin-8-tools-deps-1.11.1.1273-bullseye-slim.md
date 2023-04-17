## `clojure:temurin-8-tools-deps-1.11.1.1273-bullseye-slim`

```console
$ docker pull clojure@sha256:e1d5c77d0e74d0f59fa8541564945d8ba000f95e00451dab2d094db7369a1091
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-tools-deps-1.11.1.1273-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:f86826b3363c4dd0c65555468e74b24981095f742cae0e2f28944488cc354734
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.6 MB (147550312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f366aaf6a1caf39e3071fd72db887fa78e5e058dbdea76cf89e6750444290215`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:11:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:11:18 GMT
COPY dir:bbb84183d7ea38d81d8401f01e29d08935ee4c8bf6f90c6527579a1554c3bde1 in /opt/java/openjdk 
# Wed, 12 Apr 2023 08:11:19 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 17 Apr 2023 22:21:21 GMT
ENV CLOJURE_VERSION=1.11.1.1273
# Mon, 17 Apr 2023 22:21:21 GMT
WORKDIR /tmp
# Mon, 17 Apr 2023 22:21:38 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4938afe6c0690d2a6553141857742d94a7350c02b4fa57cd6a9c1b7cbe66492e *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Mon, 17 Apr 2023 22:21:39 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Mon, 17 Apr 2023 22:21:39 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f4a27a9e344c488df290d18697fb80bdb4bc2f7e4f2e7cb55c5f8b8c5b416b`  
		Last Modified: Wed, 12 Apr 2023 08:21:40 GMT  
		Size: 54.6 MB (54635556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4862d4781bc998874c213f3b5cd344d1c8361a9322cc0e9381eef92b9a6188f2`  
		Last Modified: Mon, 17 Apr 2023 22:29:24 GMT  
		Size: 61.5 MB (61495911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334f15d22b5a0fa30d9f050943062cdfbb18689716b7d43a49abb46e88afb41d`  
		Last Modified: Mon, 17 Apr 2023 22:29:16 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-tools-deps-1.11.1.1273-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:428c7d9de072cdae8b720c9ca1890874bb2a633264403bfdf63c0ef9e351c6cb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.4 MB (145403056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3a05bda6de3735ed19118450576307b20a22a03adb69fc378ca06069740e41e`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:18:46 GMT
COPY dir:b6d7e5613532d986930216de9e0fece0632e82564ce7a6a98baf63b4115f840d in /opt/java/openjdk 
# Wed, 12 Apr 2023 01:18:47 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 17 Apr 2023 21:40:53 GMT
ENV CLOJURE_VERSION=1.11.1.1273
# Mon, 17 Apr 2023 21:40:53 GMT
WORKDIR /tmp
# Mon, 17 Apr 2023 21:41:08 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4938afe6c0690d2a6553141857742d94a7350c02b4fa57cd6a9c1b7cbe66492e *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Mon, 17 Apr 2023 21:41:09 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Mon, 17 Apr 2023 21:41:09 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4beeaea1bb320b3b40a83a6b31783cdc7af5081dd6683ffd28ef3a3b39f888ff`  
		Last Modified: Wed, 12 Apr 2023 01:28:11 GMT  
		Size: 53.7 MB (53727937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34eabdfb1905117b7b1cb640e8aad3d4047b6109c325345c199688cf241b5d33`  
		Last Modified: Mon, 17 Apr 2023 21:47:18 GMT  
		Size: 61.6 MB (61610676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ffac64274d65e38f1d0609a5e5d00a1503d7f41f4e35c4e448901efe9147da2`  
		Last Modified: Mon, 17 Apr 2023 21:47:12 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
