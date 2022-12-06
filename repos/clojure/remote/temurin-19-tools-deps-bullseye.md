## `clojure:temurin-19-tools-deps-bullseye`

```console
$ docker pull clojure@sha256:4c9e027919648e20e04441b7a3baf6f4aa4898ded5161f0d9047709fe8f01971
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-tools-deps-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:22fbf08e02b09de603dd80cb017e1ad2ecddde6ae897a21d9cf3d4e8abbb1334
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.5 MB (303457203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b272feb6033fc3d019103ed04661472647af188b9fcc953f7a355f3c60d353b`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:41 GMT
ADD file:553d20b03d45305e58cde07e0c259421bba044155ac90b4559e5cc0b69093347 in / 
# Tue, 06 Dec 2022 01:20:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:48:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 06 Dec 2022 01:57:42 GMT
COPY dir:fef581854733ec7202f8c807463b9e1952aeb6c7a002719c7e54987e50ea4dcb in /opt/java/openjdk 
# Tue, 06 Dec 2022 01:57:44 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 01:59:47 GMT
ENV CLOJURE_VERSION=1.11.1.1200
# Tue, 06 Dec 2022 01:59:47 GMT
WORKDIR /tmp
# Tue, 06 Dec 2022 02:00:02 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "694381cb78d44f143bdcc38657507f012ebac4009bc57cec67abef1675447878 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 06 Dec 2022 02:00:03 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 06 Dec 2022 02:00:03 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 06 Dec 2022 02:00:03 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 06 Dec 2022 02:00:03 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698`  
		Last Modified: Tue, 06 Dec 2022 01:24:48 GMT  
		Size: 55.0 MB (55041342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5290555b9fd520933dc8e0c6563f92fd2a2cfc886a885094d2288c04a01ae4`  
		Last Modified: Tue, 06 Dec 2022 02:09:00 GMT  
		Size: 201.1 MB (201103430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6dac0356fbe5b2c087a0d9b9fe9e5aa4b124623e5bad3209bb36bde03366b3f`  
		Last Modified: Tue, 06 Dec 2022 02:10:11 GMT  
		Size: 47.3 MB (47311419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f3d10dc1ae3c5e8d0d3017f8c064eb2d382dc48996aea0c9193e088c63ddec`  
		Last Modified: Tue, 06 Dec 2022 02:10:05 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8654d859751d5f83591f0982c4b97e5f16443a6732077c1cd1e1137500a4d204`  
		Last Modified: Tue, 06 Dec 2022 02:10:05 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-tools-deps-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:265006ab6d8d6884dba91350f55f6f7f3dc4c0597c2e5674f44604a2659ff3ce
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.9 MB (300868638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6599e661a9470b2e13c5986c3e3688a497b765ad2208363c269c5123b9662d41`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:06 GMT
ADD file:b1e7652678bbfc9556636e77d79c947ff1436888e2929f9c5c3ddb42a50c1176 in / 
# Tue, 06 Dec 2022 01:40:07 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:15 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 06 Dec 2022 02:24:58 GMT
COPY dir:4138443eebfda1a2a245638d5bb568645bd34d79b66d39a3be31b5ac6b823d6d in /opt/java/openjdk 
# Tue, 06 Dec 2022 02:25:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 02:26:52 GMT
ENV CLOJURE_VERSION=1.11.1.1200
# Tue, 06 Dec 2022 02:26:52 GMT
WORKDIR /tmp
# Tue, 06 Dec 2022 02:27:03 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "694381cb78d44f143bdcc38657507f012ebac4009bc57cec67abef1675447878 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 06 Dec 2022 02:27:04 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 06 Dec 2022 02:27:04 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 06 Dec 2022 02:27:04 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 06 Dec 2022 02:27:04 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:4948a51a9a3f176f30ac619014f4a2da453a943244eacb53096ee9742eb7cef1`  
		Last Modified: Tue, 06 Dec 2022 01:43:33 GMT  
		Size: 53.7 MB (53699146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cabaaf976f2d5c56a302b35a76e1a18a5cb39245bb9fc93db9557a6e3e5f0b9`  
		Last Modified: Tue, 06 Dec 2022 02:35:02 GMT  
		Size: 199.9 MB (199864416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a63e23ff7f1e8f300785b7932b23603af682cbfe4e921e6412ab90715e24f75`  
		Last Modified: Tue, 06 Dec 2022 02:36:01 GMT  
		Size: 47.3 MB (47304061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9253e2142ebcdba373e42ae4bba72f7a655149638b68558e5f1c81c0e74bbcd`  
		Last Modified: Tue, 06 Dec 2022 02:35:56 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b1969594aef0cd820fc1780f5bed6ef4e3111c493c45cafb08bada50c0c9063`  
		Last Modified: Tue, 06 Dec 2022 02:35:56 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
