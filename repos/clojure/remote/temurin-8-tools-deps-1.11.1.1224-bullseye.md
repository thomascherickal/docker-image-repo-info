## `clojure:temurin-8-tools-deps-1.11.1.1224-bullseye`

```console
$ docker pull clojure@sha256:e15c26f45e46dd1366c457e4110ee215d7705c5add7ab8180a3b8e5f5e9901c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `clojure:temurin-8-tools-deps-1.11.1.1224-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:7919508d9f1957e3b2574470aad73b7c6ab37c0481cfe175b08f5b2e133a8f71
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.4 MB (179423491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:140a352deab4a50d90ea67d0e407403c9622b86dcd8cb66e945dcb27546c85a4`
-	Default Command: `["clj"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:29 GMT
ADD file:5cf2de182dac36d99ec41918889c9755f9c49c56fa0a8d0ca14040c1d8c04541 in / 
# Thu, 09 Feb 2023 03:58:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:17:51 GMT
COPY dir:b6d7e5613532d986930216de9e0fece0632e82564ce7a6a98baf63b4115f840d in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:17:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 13 Feb 2023 20:41:05 GMT
ENV CLOJURE_VERSION=1.11.1.1224
# Mon, 13 Feb 2023 20:41:06 GMT
WORKDIR /tmp
# Mon, 13 Feb 2023 20:41:27 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "3bbab4d253eda43e3122fd5705014a69c44944a6dee8ea4d7d567afe157eb4ef *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Mon, 13 Feb 2023 20:41:27 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Mon, 13 Feb 2023 20:41:28 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:80dae1b9d879348c210c40024c6e90ef92677ac3515456375fcbb70bdf07b104`  
		Last Modified: Thu, 09 Feb 2023 04:02:11 GMT  
		Size: 53.7 MB (53703368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77b7001deefab693beef32501685ba34c540df86923e1b9f608310809ebc1ce`  
		Last Modified: Thu, 09 Feb 2023 09:30:48 GMT  
		Size: 53.7 MB (53727942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2a2086b85d37ddef4ee3d3e4e0c4adb059ce21709db23d6db23b63e85b98e4`  
		Last Modified: Mon, 13 Feb 2023 20:50:16 GMT  
		Size: 72.0 MB (71991561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e7c0854d42812de7f31d23945061147fd2f1ca60a6ddb822fa7874b711f647`  
		Last Modified: Mon, 13 Feb 2023 20:50:09 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
