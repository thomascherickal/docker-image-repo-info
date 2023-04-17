## `clojure:temurin-20-bullseye`

```console
$ docker pull clojure@sha256:5897a344430356f0af3c578e3897907a3e27d0fd0512a948747d4dfa226a0b90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-20-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:af0a1b2d5fb26a95fe6f8de5afffc57b89f649517bded44ef8f4b9b60887dac2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.7 MB (329734853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6db8acc4dbf3add8846b0120ec920cb458e35d37264b3a67fbbe5e5b035babb`
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
# Mon, 17 Apr 2023 22:26:24 GMT
ENV CLOJURE_VERSION=1.11.1.1273
# Mon, 17 Apr 2023 22:26:24 GMT
WORKDIR /tmp
# Mon, 17 Apr 2023 22:26:41 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4938afe6c0690d2a6553141857742d94a7350c02b4fa57cd6a9c1b7cbe66492e *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Mon, 17 Apr 2023 22:26:42 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Mon, 17 Apr 2023 22:26:42 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Mon, 17 Apr 2023 22:26:42 GMT
ENTRYPOINT ["entrypoint"]
# Mon, 17 Apr 2023 22:26:42 GMT
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
	-	`sha256:cb717469c71388ec39ed6cafb95bc98d0d8c78a2b3dd2d648b55564a2b09c7a7`  
		Last Modified: Mon, 17 Apr 2023 22:34:04 GMT  
		Size: 71.9 MB (71880545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160a517632ea4b3d6b46cd1ff8e80d25c4324141e63f4806be45f8b644141688`  
		Last Modified: Mon, 17 Apr 2023 22:33:53 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dead781c45fc77d11155574cbb65b19dd96d46e6e10bfa8ab0199f1fcd8033b8`  
		Last Modified: Mon, 17 Apr 2023 22:33:53 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-20-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:379587d888edbfb83187345f907d8d0c604aec2ec9af42eba15baa47fdf40602
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.9 MB (326863424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50a4f6718bd786c89af0370f734572fe78a03b3f43042340695762c8e6ea18ce`
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
# Mon, 17 Apr 2023 21:44:59 GMT
ENV CLOJURE_VERSION=1.11.1.1273
# Mon, 17 Apr 2023 21:44:59 GMT
WORKDIR /tmp
# Mon, 17 Apr 2023 21:45:13 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4938afe6c0690d2a6553141857742d94a7350c02b4fa57cd6a9c1b7cbe66492e *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Mon, 17 Apr 2023 21:45:13 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Mon, 17 Apr 2023 21:45:13 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Mon, 17 Apr 2023 21:45:14 GMT
ENTRYPOINT ["entrypoint"]
# Mon, 17 Apr 2023 21:45:14 GMT
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
	-	`sha256:219e364039e4f218a8ed3a8c6105541f9689f1bf10f4440ee270f1fa757a0822`  
		Last Modified: Mon, 17 Apr 2023 21:51:00 GMT  
		Size: 72.0 MB (71996792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ee612655403c0217ab047cc021eef0bb6ff19ccffaed757c4375427b9c5460`  
		Last Modified: Mon, 17 Apr 2023 21:50:54 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd039425ae08a3ab53254c1e045f1a6149294623ad50bd8b554b6dd1832c81da`  
		Last Modified: Mon, 17 Apr 2023 21:50:54 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
