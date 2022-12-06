## `clojure:temurin-11-tools-deps-bullseye-slim`

```console
$ docker pull clojure@sha256:dfc5ba9a222acd2266f19b345d6a4a26b63da89a0f7391a4119aafba6db83635
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-tools-deps-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:ca5bf31542f0cc6be64e7dd1c28d43fd4e60e3215db97e92b2078b08603fe80d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.4 MB (291353951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4820bf36b613528adb5a8b6aa0863f5d87bd1b94810de0c5edccc840114fee00`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 06 Dec 2022 01:52:17 GMT
COPY dir:039751b2f6c905ea6e5bf7be1061a4abdf10c194a9bb43ba41c6aa90a55e71df in /opt/java/openjdk 
# Tue, 06 Dec 2022 01:52:19 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 01:54:09 GMT
ENV CLOJURE_VERSION=1.11.1.1200
# Tue, 06 Dec 2022 01:54:09 GMT
WORKDIR /tmp
# Tue, 06 Dec 2022 01:54:27 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "694381cb78d44f143bdcc38657507f012ebac4009bc57cec67abef1675447878 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 06 Dec 2022 01:54:27 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 06 Dec 2022 01:54:27 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b51844deb1462039b2a177cafb5f003ef0f5694191fab5310135e3307f2d3f`  
		Last Modified: Tue, 06 Dec 2022 02:05:31 GMT  
		Size: 198.5 MB (198455846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2896bd34102d577a14bbff7d37d40b31c768ce10a8d78df746ddb3c4072ae12`  
		Last Modified: Tue, 06 Dec 2022 02:06:29 GMT  
		Size: 61.5 MB (61484638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f3d9fd04097bd49f9e3519751021902f0c6f463192a013b371e33e4f018a51`  
		Last Modified: Tue, 06 Dec 2022 02:06:21 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-tools-deps-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:354adf3d1e6409cfac765216455360d9d78905d46f8d9c959c72ee350425a579
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.9 MB (286866256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaa7bc858f8b262a2353e2ffb509f91d72a19ebce9c258cb6ad3f4b11f705740`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 06 Dec 2022 02:20:18 GMT
COPY dir:5aa0292cc524fb250468b6c5a859d971d75bcb0dd4bed7cfb9f10423858de6d6 in /opt/java/openjdk 
# Tue, 06 Dec 2022 02:20:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 02:21:57 GMT
ENV CLOJURE_VERSION=1.11.1.1200
# Tue, 06 Dec 2022 02:21:57 GMT
WORKDIR /tmp
# Tue, 06 Dec 2022 02:22:10 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "694381cb78d44f143bdcc38657507f012ebac4009bc57cec67abef1675447878 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 06 Dec 2022 02:22:10 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 06 Dec 2022 02:22:11 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5ee26ba69cd8afd37462741fda4929d6658730baa6af64ace9a30c2c6aa3b9`  
		Last Modified: Tue, 06 Dec 2022 02:31:55 GMT  
		Size: 195.2 MB (195201090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c5294167391b6a7d3bdbc526994613cbfcb70a569cbbc9eacfb33d1a91edf5`  
		Last Modified: Tue, 06 Dec 2022 02:32:48 GMT  
		Size: 61.6 MB (61604228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33793806e1342a38e49caec6786ef5cecc753dd9fe73e22780ecf73035ffa31`  
		Last Modified: Tue, 06 Dec 2022 02:32:42 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
