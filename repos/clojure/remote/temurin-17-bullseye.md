## `clojure:temurin-17-bullseye`

```console
$ docker pull clojure@sha256:937b21b59c089a20a50d414a1920309b9f920f23799565c8e10c78adcf64429e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:424afff4ccd605a50cfd95306ed4e6dd92e5e39f1bf3b8e431eb7b1c300b2f4b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.7 MB (271711292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12bebae98919ea052059ed1acd7a83eaa9340119ef713568b0a68d91b77a0753`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:57 GMT
ADD file:20f89ff93bfbd6c9fb1a97058a1f3de4485a8974e8a83892072c511fbd2e4134 in / 
# Wed, 16 Aug 2023 00:59:58 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:06 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 18:08:24 GMT
COPY dir:534dada44a8b7afe6fc6978f0ae46933b536905423b1ac2af86e550e59d392b1 in /opt/java/openjdk 
# Wed, 16 Aug 2023 18:08:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Aug 2023 20:26:39 GMT
ENV CLOJURE_VERSION=1.11.1.1405
# Wed, 23 Aug 2023 20:26:39 GMT
WORKDIR /tmp
# Wed, 23 Aug 2023 20:26:55 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "e02966d807e5fcee40d3aeee823196fd296cb97e91746f444ac8c6681731b354 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 23 Aug 2023 20:26:56 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 23 Aug 2023 20:26:56 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 23 Aug 2023 20:26:56 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 23 Aug 2023 20:26:56 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:6a70103cc499a199e10e379794c60aa524d9598587cc2bdfe2995642c2da8df7`  
		Last Modified: Wed, 16 Aug 2023 01:04:50 GMT  
		Size: 55.1 MB (55056621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4fbbfc9003ff6a7a7db701f4c4c225eecdff24e8d91f37e9d447417a6e458b2`  
		Last Modified: Wed, 16 Aug 2023 18:17:54 GMT  
		Size: 144.8 MB (144773721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:976f07f2221fa2ef515fc6407d0463ebd3ee28923d49ed221b4c4588dbb4db62`  
		Last Modified: Wed, 23 Aug 2023 20:34:36 GMT  
		Size: 71.9 MB (71879930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f22b39fe95daa353851ff63d72c018f7517fa0a7a915e39a4e4ff3cab41b22d`  
		Last Modified: Wed, 23 Aug 2023 20:34:28 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb64826340dddb194411a8a1a7ac148b3992ef8b9c03111b77a3ffdec188483`  
		Last Modified: Wed, 23 Aug 2023 20:34:28 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:d46e54e0ce14215e3aa6dcaf78cda8037e23d7e9ffbbf2af91ef6dd3ced58292
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.2 MB (269242296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32d50d174a0862cd5cd5f48e12a46e233d5607d0115485c14f89433108658f80`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:03 GMT
ADD file:8973cddb2d84a543b71001635599951bea6485a3526ae4ff916443b584864c83 in / 
# Tue, 15 Aug 2023 23:40:04 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:14 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:25:20 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Wed, 16 Aug 2023 17:25:24 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Aug 2023 19:45:11 GMT
ENV CLOJURE_VERSION=1.11.1.1405
# Wed, 23 Aug 2023 19:45:11 GMT
WORKDIR /tmp
# Wed, 23 Aug 2023 19:45:25 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "e02966d807e5fcee40d3aeee823196fd296cb97e91746f444ac8c6681731b354 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 23 Aug 2023 19:45:26 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 23 Aug 2023 19:45:26 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 23 Aug 2023 19:45:26 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 23 Aug 2023 19:45:26 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:e837d9f05c625de5b814b851adbc03559ba02ea7078f57c81a01e18fc65bf42b`  
		Last Modified: Tue, 15 Aug 2023 23:43:37 GMT  
		Size: 53.7 MB (53704779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407f1b0394be128a63af2359d89c3282164b67cd2fac29716c6f2f5e348ec07a`  
		Last Modified: Wed, 16 Aug 2023 17:34:01 GMT  
		Size: 143.5 MB (143538089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2605b6bc8efe8e1e61c321b912c0879b4257b7387a673be945a534a61d29edd1`  
		Last Modified: Wed, 23 Aug 2023 19:51:18 GMT  
		Size: 72.0 MB (71998412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed88bf81240fba07eec5a39ee2f2f091a2de78b6c687c7e7d3e3a8b6711936e`  
		Last Modified: Wed, 23 Aug 2023 19:51:11 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225e7cc68f932a23fbd936fce74ae5f9352ec3f6237536c2ca586617f7bb3931`  
		Last Modified: Wed, 23 Aug 2023 19:51:11 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
