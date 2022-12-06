## `clojure:temurin-17-tools-deps-bullseye`

```console
$ docker pull clojure@sha256:4302294db655e83e309b1ab80facdc653631ab855d1852ebe666234d2bd7785e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-tools-deps-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:71db6f0a0376f578be9762f1431a6b21b209ff12a36b3f41e53f5a392bae5605
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.8 MB (294785109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d6a70c7ea02983ae72568f42aa6e866970d4640b6b1e4287b698f8b41c567d9`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:41 GMT
ADD file:553d20b03d45305e58cde07e0c259421bba044155ac90b4559e5cc0b69093347 in / 
# Tue, 06 Dec 2022 01:20:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:48:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 06 Dec 2022 01:54:43 GMT
COPY dir:fa15c3254735d08fe4cb4c940d6fc08efc9755ff0499a6eb8e51c961cea48d5c in /opt/java/openjdk 
# Tue, 06 Dec 2022 01:54:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 01:56:51 GMT
ENV CLOJURE_VERSION=1.11.1.1200
# Tue, 06 Dec 2022 01:56:51 GMT
WORKDIR /tmp
# Tue, 06 Dec 2022 01:57:06 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "694381cb78d44f143bdcc38657507f012ebac4009bc57cec67abef1675447878 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 06 Dec 2022 01:57:06 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 06 Dec 2022 01:57:06 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 06 Dec 2022 01:57:06 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 06 Dec 2022 01:57:07 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698`  
		Last Modified: Tue, 06 Dec 2022 01:24:48 GMT  
		Size: 55.0 MB (55041342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c44c11d030ccad72929755f22eeb76adeb4e273253c295bb22aa0cd941361f3`  
		Last Modified: Tue, 06 Dec 2022 02:06:58 GMT  
		Size: 192.4 MB (192431239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e7a664c9717961b6d33fc78ef4cd189d36872ff630a57319bec9773861e455`  
		Last Modified: Tue, 06 Dec 2022 02:08:09 GMT  
		Size: 47.3 MB (47311511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ac9260b331a43003896682f7218e34be2e8d93738c2f4fc39112d41c3de0e8`  
		Last Modified: Tue, 06 Dec 2022 02:08:03 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34662477d229bc2cc8ceb1bb9d08e06b0993623db9fd68efda42630ffb11ccb`  
		Last Modified: Tue, 06 Dec 2022 02:08:03 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-tools-deps-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:fe311e83886ca74654ed63bb339ddd06ee001b281af5e33594796898bb4e20ad
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.2 MB (292219511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34149d9af0998116116b7f3ab18b3f43f27f29244089935805654b918bf54893`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:06 GMT
ADD file:b1e7652678bbfc9556636e77d79c947ff1436888e2929f9c5c3ddb42a50c1176 in / 
# Tue, 06 Dec 2022 01:40:07 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:15 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 06 Dec 2022 02:22:20 GMT
COPY dir:36850aee002fdc5445f17d75b8266c48f8e705973ece815c3b53d28b6656ac3e in /opt/java/openjdk 
# Tue, 06 Dec 2022 02:22:24 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 02:24:16 GMT
ENV CLOJURE_VERSION=1.11.1.1200
# Tue, 06 Dec 2022 02:24:16 GMT
WORKDIR /tmp
# Tue, 06 Dec 2022 02:24:28 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "694381cb78d44f143bdcc38657507f012ebac4009bc57cec67abef1675447878 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 06 Dec 2022 02:24:28 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 06 Dec 2022 02:24:28 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 06 Dec 2022 02:24:28 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 06 Dec 2022 02:24:28 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:4948a51a9a3f176f30ac619014f4a2da453a943244eacb53096ee9742eb7cef1`  
		Last Modified: Tue, 06 Dec 2022 01:43:33 GMT  
		Size: 53.7 MB (53699146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e740ce804b4f2a8b5a6fbc891e6b48bdae55634c8831862b9b2bcc60b87ad1`  
		Last Modified: Tue, 06 Dec 2022 02:33:14 GMT  
		Size: 191.2 MB (191215247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bfd25ca561b2c31a16c4106eff5d72ae8bd4f999d2933bef9ad53a232d55f6b`  
		Last Modified: Tue, 06 Dec 2022 02:34:16 GMT  
		Size: 47.3 MB (47304103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9927b29cef968167c1f0e08532cef29414ac5c9e1be5f6079f32bb67f1b0c4db`  
		Last Modified: Tue, 06 Dec 2022 02:34:12 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbfb49fb1fa93f1ba40a5b7b7a32014b5b9de57922c56596ec2f6dced4b2e33`  
		Last Modified: Tue, 06 Dec 2022 02:34:12 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
