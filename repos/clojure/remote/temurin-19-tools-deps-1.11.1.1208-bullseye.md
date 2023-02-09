## `clojure:temurin-19-tools-deps-1.11.1.1208-bullseye`

```console
$ docker pull clojure@sha256:1fdd1cd18a09bb9dbe1d5e641248b3a34bd8d4cbae49693ee7c3986bfd0c524c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-tools-deps-1.11.1.1208-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:df8c4a081f77e449e97bdb9949e897927744ce2754f8caca6c5c57efc6d03116
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.0 MB (328028737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73b2367f650da512459817a6f92a0f5a82908e24434918051738665aa500c6b5`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:05 GMT
ADD file:b03d13d345c29f69557f410c8504e748226756d1f48e5abdb63cd40179b2640c in / 
# Thu, 09 Feb 2023 03:20:05 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:31:09 GMT
COPY dir:94cb5af8175285c10c94286222d8a35302f3f8c290e00011a75c67156659d6ab in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:31:11 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:33:13 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Thu, 09 Feb 2023 09:33:13 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:33:31 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 09 Feb 2023 09:33:32 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 09 Feb 2023 09:33:32 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Thu, 09 Feb 2023 09:33:32 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 09 Feb 2023 09:33:32 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:1e4aec178e0864db93a6f97a20bde3445871a4562c1801185eca1238d3a0e80d`  
		Last Modified: Thu, 09 Feb 2023 03:24:47 GMT  
		Size: 55.0 MB (55046771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441046777b829253c9900fed7834e1437d44d485f4ec90904dc51bc5aac05148`  
		Last Modified: Thu, 09 Feb 2023 09:42:23 GMT  
		Size: 201.1 MB (201112949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f17b40531948f8e90bbb2f9de577f8455e4d2092a69eabf56f5dbdea4901f0a`  
		Last Modified: Thu, 09 Feb 2023 09:43:28 GMT  
		Size: 71.9 MB (71867999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1edc7b3cb9e4a6ecebf6675b180264700420c92eeb9a5c9ed424068913abefc6`  
		Last Modified: Thu, 09 Feb 2023 09:43:20 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2265a47a7cbcaf1801adae73a92623ea4ffb616784cbbd7f6952ea6690fa3f6e`  
		Last Modified: Thu, 09 Feb 2023 09:43:20 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-tools-deps-1.11.1.1208-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:dcf1188fd948da8cb9cbaa79ad437da5d1c3698fb72c10d0c909858a86616f88
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.5 MB (325545465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f41c7eedeae919242cb1f440e97ecaf0a1a410f0177f4dcaee91a2b0f6fe56e`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:29 GMT
ADD file:5cf2de182dac36d99ec41918889c9755f9c49c56fa0a8d0ca14040c1d8c04541 in / 
# Thu, 09 Feb 2023 03:58:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:25:55 GMT
COPY dir:9a6a873ca11063f6f04e7f088397a1fce771e2b1aa8590b72eb07158cfac883f in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:26:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:27:42 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Thu, 09 Feb 2023 09:27:42 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:27:56 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 09 Feb 2023 09:27:56 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 09 Feb 2023 09:27:57 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Thu, 09 Feb 2023 09:27:57 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 09 Feb 2023 09:27:57 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:80dae1b9d879348c210c40024c6e90ef92677ac3515456375fcbb70bdf07b104`  
		Last Modified: Thu, 09 Feb 2023 04:02:11 GMT  
		Size: 53.7 MB (53703368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04575e4d68cefe99b7db24f9eba8de51503dbe724ee7b0b0862498a73eeefbf3`  
		Last Modified: Thu, 09 Feb 2023 09:36:01 GMT  
		Size: 199.9 MB (199855167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84fb7c3354faa1e763671879db30d621c814b00289f8bf5f8644aad97dc66898`  
		Last Modified: Thu, 09 Feb 2023 09:37:02 GMT  
		Size: 72.0 MB (71985910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9531726c80b7427dc80bd80b24c551b8af663d379b8a4c9d32f9541428ec7c2f`  
		Last Modified: Thu, 09 Feb 2023 09:36:55 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6991a87ad25bbba4f606ad2adedd01162aa52546afc7a1d9a26dfb5904f10ca6`  
		Last Modified: Thu, 09 Feb 2023 09:36:55 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
