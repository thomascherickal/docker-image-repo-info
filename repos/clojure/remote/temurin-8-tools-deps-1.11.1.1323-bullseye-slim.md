## `clojure:temurin-8-tools-deps-1.11.1.1323-bullseye-slim`

```console
$ docker pull clojure@sha256:0e6d1064f2c03350d55682ed16635c3582330a1bc967fceba10fac27f3c3a351
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `clojure:temurin-8-tools-deps-1.11.1.1323-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:b38bcf0f16e04738df3ca4b8ba7014dae93aae15e1aad6d5c28e78539c8b0834
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.4 MB (145404962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66733af646684c0d3e77c7ab068852dea467953ca481bf9e8d3d880d6feffcd3`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:44:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 03 May 2023 17:44:17 GMT
COPY dir:f6bbe63c81e220d954915791686219263d8c45918fd81b238f7c9f6b21f076f8 in /opt/java/openjdk 
# Wed, 03 May 2023 17:44:19 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 19 May 2023 19:44:43 GMT
ENV CLOJURE_VERSION=1.11.1.1323
# Fri, 19 May 2023 19:44:43 GMT
WORKDIR /tmp
# Fri, 19 May 2023 19:44:56 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "c4666f0e2c2397b91554befd71ff6149b2e89acbf90400e1dcf557526cfb593d *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 19 May 2023 19:44:57 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 19 May 2023 19:44:57 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45323ce94562764c60b759096664441c4fd32a723ce4c04882e7478c93e9b104`  
		Last Modified: Wed, 03 May 2023 17:53:34 GMT  
		Size: 53.7 MB (53742660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8336f417789486f1d3581cbf766644fb0c4a278d0b713998183d12658d87201`  
		Last Modified: Fri, 19 May 2023 19:54:31 GMT  
		Size: 61.6 MB (61608953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca83ee635c467aea534e1f06b2c7ed38f420073bfdb038a84c2d04f6748cea5b`  
		Last Modified: Fri, 19 May 2023 19:54:25 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
