## `clojure:temurin-19-tools-deps-bullseye`

```console
$ docker pull clojure@sha256:b32a7390c4645f7a593265d9da6aa48ff2e34582e16c494b05c1fc81828ba995
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-tools-deps-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:4f3f6ab30376c0f2f373dcdf64cef2799393f6b407659cfae2dce436a87f236f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.4 MB (303433136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0960727b2e9759599a4e250220504a8e6e0b6a826e737a523556b389458c7afb`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:21 GMT
ADD file:c13b430c8699df107ffd9ea5230b92238bc037a8e1cbbe35d6ab664941d575da in / 
# Wed, 21 Dec 2022 01:20:22 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:50:07 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 21 Dec 2022 01:59:28 GMT
COPY dir:fef581854733ec7202f8c807463b9e1952aeb6c7a002719c7e54987e50ea4dcb in /opt/java/openjdk 
# Wed, 21 Dec 2022 01:59:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Dec 2022 02:01:36 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Wed, 21 Dec 2022 02:01:36 GMT
WORKDIR /tmp
# Wed, 21 Dec 2022 02:01:52 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 21 Dec 2022 02:01:53 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 21 Dec 2022 02:01:53 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 21 Dec 2022 02:01:53 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 21 Dec 2022 02:01:53 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:32de3c850997ce03b6ff4ae8fb00b34b9d7d7f9a35bfcdb8538e22cc7b77c29d`  
		Last Modified: Wed, 21 Dec 2022 01:24:10 GMT  
		Size: 55.0 MB (55025166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d80e226f52e65f91550fee64cdd6a467c4da00bac7bed86c44aa550b443f1d`  
		Last Modified: Wed, 21 Dec 2022 02:10:56 GMT  
		Size: 201.1 MB (201103393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d0b2b6d2f70459f24eb1d5fe8ffae03fc4a246672a15a89fe19e671f2a3d3e`  
		Last Modified: Wed, 21 Dec 2022 02:12:02 GMT  
		Size: 47.3 MB (47303562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4313d098cc233b5253bce3556a2f39c6ad80b7a5702ca6469984ac8ab56b7581`  
		Last Modified: Wed, 21 Dec 2022 02:11:56 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a5b6407a65a42010f0acf18db1907a274b610d6e50e62e71b15eed9aa61050`  
		Last Modified: Wed, 21 Dec 2022 02:11:56 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-tools-deps-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:c93fee3903cc9ec907d09e70e2060298db87a5f674def9843f1a513cf4e17e12
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.8 MB (300840194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca36b71fd363b116b5076675a36a43d7c471b801c7afbe4fbd550e963d26a6b9`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:40 GMT
ADD file:5bbdc914ec8ed60ac85293e88ee1aafc3f0290762e320fc86dc9d79fa201834e in / 
# Wed, 21 Dec 2022 01:39:41 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:18:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 21 Dec 2022 02:25:44 GMT
COPY dir:4138443eebfda1a2a245638d5bb568645bd34d79b66d39a3be31b5ac6b823d6d in /opt/java/openjdk 
# Wed, 21 Dec 2022 02:25:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Dec 2022 02:27:36 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Wed, 21 Dec 2022 02:27:36 GMT
WORKDIR /tmp
# Wed, 21 Dec 2022 02:27:48 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 21 Dec 2022 02:27:49 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 21 Dec 2022 02:27:49 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 21 Dec 2022 02:27:49 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 21 Dec 2022 02:27:49 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:c3e6129b48b69d14c5e7a5605e2b94003fb71aac82eac46b8689f5b8007af2c5`  
		Last Modified: Wed, 21 Dec 2022 01:42:49 GMT  
		Size: 53.7 MB (53681797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5504f1730ed4e1dc3a15ab910d7a54c44be3b7eaa38521d40d2d6396a25c2b74`  
		Last Modified: Wed, 21 Dec 2022 02:35:43 GMT  
		Size: 199.9 MB (199864404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc3c9808437a7a92178b9e0ecfec4c3b2e3c2a15c47716756b79c775075fffe`  
		Last Modified: Wed, 21 Dec 2022 02:36:41 GMT  
		Size: 47.3 MB (47292977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd067b3d587ddce2ed5a1d67eb94266b2be9e64daa8381d9192d4a3891435b2`  
		Last Modified: Wed, 21 Dec 2022 02:36:36 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05237ceda3b3ca3a419ff427c3e28665283d073463e63d56bb17ec0098fc5be8`  
		Last Modified: Wed, 21 Dec 2022 02:36:36 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
