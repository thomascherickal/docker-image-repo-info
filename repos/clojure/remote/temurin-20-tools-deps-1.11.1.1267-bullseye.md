## `clojure:temurin-20-tools-deps-1.11.1.1267-bullseye`

```console
$ docker pull clojure@sha256:ca6bc6c17e92fbc961af68d4d6466165189f6c32ee980877c0ad8e67a5b448cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-20-tools-deps-1.11.1.1267-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:be04e99032611f1d1051ea100a348a4789df70e636d55383e998ed53e166a77e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.7 MB (329734299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a5d465b683524810cc50884757af6c336ba356cf4df6a3c6498e641bc7373d4`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:10:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:18:50 GMT
COPY dir:0f9b663d61413099f20817ab55258941c09987290b8ce360d0fb2fab00ddddda in /opt/java/openjdk 
# Wed, 12 Apr 2023 08:18:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 08:19:41 GMT
ENV CLOJURE_VERSION=1.11.1.1267
# Wed, 12 Apr 2023 08:19:41 GMT
WORKDIR /tmp
# Wed, 12 Apr 2023 08:19:57 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "c949c9ba24ee46a2c57c6e6aeff262ebb0ff8112ee2367b3dbabd2f2df75380a *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 12 Apr 2023 08:19:57 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 12 Apr 2023 08:19:58 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 12 Apr 2023 08:19:58 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 12 Apr 2023 08:19:58 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb7d4bc5e99617b9205b6de7fb6d4899b028181001a97de7705ce560e55a602`  
		Last Modified: Wed, 12 Apr 2023 08:26:22 GMT  
		Size: 202.8 MB (202800557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a89fef89b2b74da90c130c425c5f34daeb4a8a774db4c623a17bf6aa6e3fe22`  
		Last Modified: Wed, 12 Apr 2023 08:27:02 GMT  
		Size: 71.9 MB (71879993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b88d5704848eb480b57ba98d56a5d01073d0770ebea22a180cde2126935745`  
		Last Modified: Wed, 12 Apr 2023 08:26:55 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c49a719f10a2a7dd96b909230a9495fd4a3092690bb7dbb98d6285a6cc877b2b`  
		Last Modified: Wed, 12 Apr 2023 08:26:54 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-20-tools-deps-1.11.1.1267-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:23f08b643d1c2b91f802561c885746b3d61f99084feae7f3ea5282a4af74de10
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.9 MB (326863382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69aba6931bca4d9c10f20127014807f3b46b7fc31d65c5b692d5556ab43333c9`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:25:31 GMT
COPY dir:66b65f1974fed4b5bc3675e6b378c93a3ba9feeabfec7eeabd6d1d0b07fd5fa4 in /opt/java/openjdk 
# Wed, 12 Apr 2023 01:25:36 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 01:26:24 GMT
ENV CLOJURE_VERSION=1.11.1.1267
# Wed, 12 Apr 2023 01:26:25 GMT
WORKDIR /tmp
# Wed, 12 Apr 2023 01:26:38 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "c949c9ba24ee46a2c57c6e6aeff262ebb0ff8112ee2367b3dbabd2f2df75380a *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 12 Apr 2023 01:26:39 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 12 Apr 2023 01:26:39 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 12 Apr 2023 01:26:39 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 12 Apr 2023 01:26:39 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9fc51dd626337cedfa8259e3da03cef96eece3f3118695f388ae26fd81e82bd`  
		Last Modified: Wed, 12 Apr 2023 01:32:34 GMT  
		Size: 201.2 MB (201160086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148e8e31aea1aeeea95da7fe0d3eaeaafc6d434fc12111027fbbb92da1e8fe67`  
		Last Modified: Wed, 12 Apr 2023 01:33:10 GMT  
		Size: 72.0 MB (71996755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947de9fd2bb8b869ad812a0323142f5099e9f3cc90dcf37adccaf3b90a7d8c16`  
		Last Modified: Wed, 12 Apr 2023 01:33:03 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420f18bb454dcedac7c33f4ebb076283441960d3a4eda4cd6d230c87c178220a`  
		Last Modified: Wed, 12 Apr 2023 01:33:03 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
