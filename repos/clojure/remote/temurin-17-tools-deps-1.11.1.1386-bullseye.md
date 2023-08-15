## `clojure:temurin-17-tools-deps-1.11.1.1386-bullseye`

```console
$ docker pull clojure@sha256:45ce66574bf881638fe162ac6d5cba16aa248101c4dc68235b370db7b25ba089
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-17-tools-deps-1.11.1.1386-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:02fbccf9a2b8f05cb789e092b1d8b19d71c13fae172ee52a17499462a67d43cb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.7 MB (271724944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:057f4e044eb3c5a2441fe2db2b2bf1003401350666b91cbb5cff67b6199d5da1`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:13:47 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 08 Aug 2023 22:36:59 GMT
COPY dir:8ea3eea47bd8b9d37ce2403b2d64b2cdc0fec836a119c10ec3e4ff0bcca8bb4d in /opt/java/openjdk 
# Tue, 08 Aug 2023 22:37:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 14 Aug 2023 23:24:28 GMT
ENV CLOJURE_VERSION=1.11.1.1386
# Mon, 14 Aug 2023 23:24:28 GMT
WORKDIR /tmp
# Mon, 14 Aug 2023 23:24:44 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "3a09e2df4d3abd89b5b1286af0133a36a525ff3acfe1432f98b5c24b170940e8 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Mon, 14 Aug 2023 23:24:44 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Mon, 14 Aug 2023 23:24:44 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Mon, 14 Aug 2023 23:24:45 GMT
ENTRYPOINT ["entrypoint"]
# Mon, 14 Aug 2023 23:24:45 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ad5f652aa0a9735f05b6a5d86369751c117fe48131a7c9ff7427b064b3036c`  
		Last Modified: Tue, 08 Aug 2023 22:49:32 GMT  
		Size: 144.8 MB (144773784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915a2e9cb869dfb8aa6ed2c28d78535c0716d42cf84581346f9aef650366774c`  
		Last Modified: Mon, 14 Aug 2023 23:32:33 GMT  
		Size: 71.9 MB (71894571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb7f36cbbb16c4af6ad5e4328c43cc8f6293a2a8dc67231537532ce7d73a4ba`  
		Last Modified: Mon, 14 Aug 2023 23:32:25 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9e75fd2b1405346e57081dec134aa4461deaa95b977ad88a3559286d44c351`  
		Last Modified: Mon, 14 Aug 2023 23:32:25 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
