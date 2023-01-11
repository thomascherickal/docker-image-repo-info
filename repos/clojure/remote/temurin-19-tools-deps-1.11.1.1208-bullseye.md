## `clojure:temurin-19-tools-deps-1.11.1.1208-bullseye`

```console
$ docker pull clojure@sha256:e5016116cc352022acbcfa5d78972c5197951715746c547193f7676ed44933fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-tools-deps-1.11.1.1208-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:559a74898291cd69d742d4f2d0b999dfae65c85dedcfd80bcaae244adad2e473
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.0 MB (327987954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:994396a88ce403b1a46331a30e281cca968ca1ff3bb407e4c7cf55de3877d7ba`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:29 GMT
ADD file:917750a82b29f8f7f88a121017bd9dfeb0fbcc8f0697a009f08b6b58246eff4b in / 
# Wed, 11 Jan 2023 02:34:30 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:18:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 11 Jan 2023 03:28:45 GMT
COPY dir:fef581854733ec7202f8c807463b9e1952aeb6c7a002719c7e54987e50ea4dcb in /opt/java/openjdk 
# Wed, 11 Jan 2023 03:28:46 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 03:30:57 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Wed, 11 Jan 2023 03:30:58 GMT
WORKDIR /tmp
# Wed, 11 Jan 2023 03:31:16 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 11 Jan 2023 03:31:16 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 11 Jan 2023 03:31:16 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 11 Jan 2023 03:31:16 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 11 Jan 2023 03:31:17 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:bbeef03cda1f5d6c9e20c310c1c91382a6b0a1a2501c3436b28152f13896f082`  
		Last Modified: Wed, 11 Jan 2023 02:38:42 GMT  
		Size: 55.0 MB (55025206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4098b1c8c484b772797e0f47e372b00d98eca8d709362a704bbcfe078971a4`  
		Last Modified: Wed, 11 Jan 2023 03:40:21 GMT  
		Size: 201.1 MB (201103372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc2f04b6009b33f1ed0300f79430f39c50f46f1bb27fcb40288838912326abd`  
		Last Modified: Wed, 11 Jan 2023 03:41:27 GMT  
		Size: 71.9 MB (71858359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf8b2bc89fd428e2f1089fe61c76f47a04cdf35d7fca748f9deb2b2ea713bd4`  
		Last Modified: Wed, 11 Jan 2023 03:41:18 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17682fc968af3dcc018d96e2183a598c2ffd432cadcd246c7b8f90f0f4189345`  
		Last Modified: Wed, 11 Jan 2023 03:41:18 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-tools-deps-1.11.1.1208-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:5083ffaf230bda89823fbc932f0bb686a22dc2fcd0200b8cc5586bb09d5deaa0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.5 MB (325526378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:385f919c9f9e9b0e35ab93f98eeb83eb4a0e7c7ebad7d8b0a015ba785ee41fb4`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:24 GMT
ADD file:9e185c2d9ca8a231a39ee2b1761fcdff75065252d25a65a207acb7a319c1cf23 in / 
# Wed, 11 Jan 2023 02:57:25 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:14 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 11 Jan 2023 03:45:54 GMT
COPY dir:4138443eebfda1a2a245638d5bb568645bd34d79b66d39a3be31b5ac6b823d6d in /opt/java/openjdk 
# Wed, 11 Jan 2023 03:45:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 03:47:49 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Wed, 11 Jan 2023 03:47:49 GMT
WORKDIR /tmp
# Wed, 11 Jan 2023 03:48:03 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 11 Jan 2023 03:48:04 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 11 Jan 2023 03:48:04 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 11 Jan 2023 03:48:04 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 11 Jan 2023 03:48:04 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:c345c9e441f5f49235768af74b8ab37743652d38958afaa000edd56d7b2f0540`  
		Last Modified: Wed, 11 Jan 2023 03:00:56 GMT  
		Size: 53.7 MB (53681859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a772f0e37f556b3ef1a18a30aff7106c88d94b6e9d9a1ac12a245942bb7995b5`  
		Last Modified: Wed, 11 Jan 2023 03:56:03 GMT  
		Size: 199.9 MB (199864459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba22c0511989b14a06911876ec0f10f443f859d14a09fa87a188199d9ebf0f9`  
		Last Modified: Wed, 11 Jan 2023 03:57:03 GMT  
		Size: 72.0 MB (71979043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16e742aff546f2b4ce377f47d90d5514fcf3c9b74d1a711f5fb82f49467edf84`  
		Last Modified: Wed, 11 Jan 2023 03:56:56 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb7c3c2185095c0c89ab9e0b30c67284dc0acb56f3b493eeaf21ca9e0ef3748`  
		Last Modified: Wed, 11 Jan 2023 03:56:56 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
