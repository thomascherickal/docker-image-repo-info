## `clojure:temurin-17-tools-deps-1.11.1.1224-bullseye-slim`

```console
$ docker pull clojure@sha256:5699da0dc9a4df6b2357d578ebaee28354d0b70ba4a54d2bd4933cee4b5c49a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `clojure:temurin-17-tools-deps-1.11.1.1224-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:e8836138ad872d7369df68cb9167cb001480de103b753b5cf2eb9992fb1aa8ac
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.9 MB (282922859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d55da8fb31c16dc1a6614217e405496f93bfa0b2efe7de0681bcf3e6596dfa3`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:18:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:23:59 GMT
COPY dir:a1bd99c3d82513db94430c73467e1e5c69ea4624d0489571d594afe503e15dc5 in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:24:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 13 Feb 2023 20:45:07 GMT
ENV CLOJURE_VERSION=1.11.1.1224
# Mon, 13 Feb 2023 20:45:07 GMT
WORKDIR /tmp
# Mon, 13 Feb 2023 20:45:21 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "3bbab4d253eda43e3122fd5705014a69c44944a6dee8ea4d7d567afe157eb4ef *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Mon, 13 Feb 2023 20:45:21 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Mon, 13 Feb 2023 20:45:21 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Mon, 13 Feb 2023 20:45:21 GMT
ENTRYPOINT ["entrypoint"]
# Mon, 13 Feb 2023 20:45:21 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7586f864daee85da340c78373323940ea5aadab0913592ab630744b3a8d6605`  
		Last Modified: Thu, 09 Feb 2023 09:34:26 GMT  
		Size: 191.3 MB (191260427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d0f6f256881027ec6b64f552696f3956273d7664bee45d722dfd3bd3ed5853`  
		Last Modified: Mon, 13 Feb 2023 20:53:25 GMT  
		Size: 61.6 MB (61598904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe288eac18280c08e39658b8835de07ef5968aef0bb29ab50cb3b3f9a0fcf19`  
		Last Modified: Mon, 13 Feb 2023 20:53:19 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fcbf9db9944d7da64ae8566980a41991f54d8891f77919c5ff67037667aa57c`  
		Last Modified: Mon, 13 Feb 2023 20:53:19 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
