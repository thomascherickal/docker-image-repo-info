## `clojure:temurin-11-tools-deps-bullseye`

```console
$ docker pull clojure@sha256:bc81b7d2ea2fa957e35decf4f5db5615d8ddf8551fcbe20551c0c9bcad3ebd2f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-tools-deps-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:be6441e67d8abc76f3fbf5eeb4a91ac1316e84a2646ec08f8248a91035a5d791
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.4 MB (325409665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42e6a7bc6df7d610690d264a4a5a17892d9f355c42f83084d186ef4aae94e337`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:10:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:13:28 GMT
COPY dir:e649a995635d4b28f1458e8ccc09f5f71440b52479cfda5ea11e99ab14d0ce82 in /opt/java/openjdk 
# Wed, 12 Apr 2023 08:13:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 17 Apr 2023 22:23:13 GMT
ENV CLOJURE_VERSION=1.11.1.1273
# Mon, 17 Apr 2023 22:23:13 GMT
WORKDIR /tmp
# Mon, 17 Apr 2023 22:23:30 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4938afe6c0690d2a6553141857742d94a7350c02b4fa57cd6a9c1b7cbe66492e *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Mon, 17 Apr 2023 22:23:30 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Mon, 17 Apr 2023 22:23:30 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc28d33e44b328c3a33e1c0717d82dcbea604364ba89e1ab1b64f3d3a2f165a`  
		Last Modified: Wed, 12 Apr 2023 08:22:57 GMT  
		Size: 198.5 MB (198476040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f49bcb7f5e3af33fe7f4279e1765caf762f1c169ae5802e970a40f9d97ea2f5`  
		Last Modified: Mon, 17 Apr 2023 22:30:41 GMT  
		Size: 71.9 MB (71880272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d7fd313ce28fbd6f175e26b2c6fde473071afb7716a5fa7887d982b6e0db83`  
		Last Modified: Mon, 17 Apr 2023 22:30:33 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-tools-deps-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:66d1c7db016d02fd5ce73b77c1239835a31e8dabb8ae6550ffaeb9af92794ba0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.9 MB (320945653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6da47ba97bafd4a03512e9962328950388ce8061b2b9cfc85d915c0e4bb2867`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:20:38 GMT
COPY dir:d446509417048b798354227404c222c2c6031477a91cb1b64eded33f5e598adf in /opt/java/openjdk 
# Wed, 12 Apr 2023 01:20:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 17 Apr 2023 21:42:35 GMT
ENV CLOJURE_VERSION=1.11.1.1273
# Mon, 17 Apr 2023 21:42:35 GMT
WORKDIR /tmp
# Mon, 17 Apr 2023 21:42:49 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4938afe6c0690d2a6553141857742d94a7350c02b4fa57cd6a9c1b7cbe66492e *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Mon, 17 Apr 2023 21:42:50 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Mon, 17 Apr 2023 21:42:50 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e34d229c4186d9e7e7ce0aee26abda131ebcee8bee99be5af11bfc1bf391db`  
		Last Modified: Wed, 12 Apr 2023 01:29:24 GMT  
		Size: 195.2 MB (195242537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adec3e609be6c29e6b135c5a17876ae6f67e1580d4b1607596d841c36e7fc0a`  
		Last Modified: Mon, 17 Apr 2023 21:48:16 GMT  
		Size: 72.0 MB (71996969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142c74f9ecacee6f761d963b77d2dd55ca79f6d56ecd6a185c4102046fd5b090`  
		Last Modified: Mon, 17 Apr 2023 21:48:10 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
