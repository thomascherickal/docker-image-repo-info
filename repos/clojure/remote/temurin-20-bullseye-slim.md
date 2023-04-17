## `clojure:temurin-20-bullseye-slim`

```console
$ docker pull clojure@sha256:baccb3b3dab429e85d4d1e8597c847396f9085fb3ca8ef4eff06f610b7e874c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-20-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:14c0f1be4981fc858d0b65e144189090d123770d70fe61510ceb581d7422dc47
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.7 MB (295715480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0a56f859410d2e01a9466ef977862df5846d51e9205950c8504b3204adc662d`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:11:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:19:17 GMT
COPY dir:0f9b663d61413099f20817ab55258941c09987290b8ce360d0fb2fab00ddddda in /opt/java/openjdk 
# Wed, 12 Apr 2023 08:19:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 17 Apr 2023 22:26:44 GMT
ENV CLOJURE_VERSION=1.11.1.1273
# Mon, 17 Apr 2023 22:26:44 GMT
WORKDIR /tmp
# Mon, 17 Apr 2023 22:27:00 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4938afe6c0690d2a6553141857742d94a7350c02b4fa57cd6a9c1b7cbe66492e *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Mon, 17 Apr 2023 22:27:01 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Mon, 17 Apr 2023 22:27:01 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Mon, 17 Apr 2023 22:27:01 GMT
ENTRYPOINT ["entrypoint"]
# Mon, 17 Apr 2023 22:27:01 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b32b49a5ad9ee1b838c8a414680cfb573b6bf63d15cefb9f67402b317700b6`  
		Last Modified: Wed, 12 Apr 2023 08:26:44 GMT  
		Size: 202.8 MB (202800600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b360969e680031dde41de55157e6ff33a1b250993a049d03f97a8b716c6ce56`  
		Last Modified: Mon, 17 Apr 2023 22:34:21 GMT  
		Size: 61.5 MB (61495636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b0804fa8ce20ea6ea3905c8e53bd22abd572a0c0266e5efeef56d3f2660523`  
		Last Modified: Mon, 17 Apr 2023 22:34:14 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb08096dacd97f561c6930f6aa8f5d862adf846900deb43a600cce4c561f74b6`  
		Last Modified: Mon, 17 Apr 2023 22:34:14 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-20-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:9df30f203beac2157ec97098ccc08d4cf89e4e1c45f7685a01786cae04aff5d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.8 MB (292835760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:783f4d25f413c624741936fc28e960b0d6cdf5630d8308f412eb113c9a04165b`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:25:57 GMT
COPY dir:66b65f1974fed4b5bc3675e6b378c93a3ba9feeabfec7eeabd6d1d0b07fd5fa4 in /opt/java/openjdk 
# Wed, 12 Apr 2023 01:26:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 17 Apr 2023 21:45:15 GMT
ENV CLOJURE_VERSION=1.11.1.1273
# Mon, 17 Apr 2023 21:45:15 GMT
WORKDIR /tmp
# Mon, 17 Apr 2023 21:45:28 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4938afe6c0690d2a6553141857742d94a7350c02b4fa57cd6a9c1b7cbe66492e *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Mon, 17 Apr 2023 21:45:29 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Mon, 17 Apr 2023 21:45:29 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Mon, 17 Apr 2023 21:45:29 GMT
ENTRYPOINT ["entrypoint"]
# Mon, 17 Apr 2023 21:45:29 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ac14b41f3aaaeba0605fc04f599b4365bfd232c1b3f11a8c1c5c7c4cceaa9b`  
		Last Modified: Wed, 12 Apr 2023 01:32:54 GMT  
		Size: 201.2 MB (201160129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a25bb2234e7b1a9bfddda468f9df53c60e46a63b2520c46e600be2ee2f0e7b2`  
		Last Modified: Mon, 17 Apr 2023 21:51:17 GMT  
		Size: 61.6 MB (61610788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85052b58601c0bf101a51079f769c9ef32d432047b35595f255973cff2ddc3bf`  
		Last Modified: Mon, 17 Apr 2023 21:51:11 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ec05735cd5ce4a175f1211468f46f784fbf18726c5739d378dde2b49cebd32`  
		Last Modified: Mon, 17 Apr 2023 21:51:11 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
