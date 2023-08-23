## `clojure:temurin-17-tools-deps-1.11.1.1405-bullseye-slim`

```console
$ docker pull clojure@sha256:be13a35c0e1702c1632b2ed479488e38e9f433a2a675c0008e9b509f801c6033
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-tools-deps-1.11.1.1405-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:1d390c504d1402acb5af01204881153db453b29fdc65da41ec395869a7183693
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.7 MB (237687717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6931dd8240b8e95ea700cbc483deebe2f0b9b3e0cd0c0be4cc8570243316dd4e`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:01:12 GMT
COPY dir:534dada44a8b7afe6fc6978f0ae46933b536905423b1ac2af86e550e59d392b1 in /opt/java/openjdk 
# Wed, 16 Aug 2023 18:08:57 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Aug 2023 20:26:59 GMT
ENV CLOJURE_VERSION=1.11.1.1405
# Wed, 23 Aug 2023 20:27:00 GMT
WORKDIR /tmp
# Wed, 23 Aug 2023 20:27:16 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "e02966d807e5fcee40d3aeee823196fd296cb97e91746f444ac8c6681731b354 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 23 Aug 2023 20:27:16 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 23 Aug 2023 20:27:16 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 23 Aug 2023 20:27:17 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 23 Aug 2023 20:27:17 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f19d3c0c76607d38f469ea69cdeea9a0f589af42c6145f4530a3ae325eaef2`  
		Last Modified: Wed, 16 Aug 2023 17:03:52 GMT  
		Size: 144.8 MB (144773731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed06e3b5cf5ea142a0e9f041b20809af2f7f028f7655ada425dd4d589d9602f`  
		Last Modified: Wed, 23 Aug 2023 20:34:54 GMT  
		Size: 61.5 MB (61495291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d8a2798ae00fd4e474faaa3c613db02d881863a038edd967b5598e5a979e95`  
		Last Modified: Wed, 23 Aug 2023 20:34:47 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48257acdfe41c44e8cadd78ecfeec138d2e19e7e22a7482487be27bc3f0e7340`  
		Last Modified: Wed, 23 Aug 2023 20:34:47 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-tools-deps-1.11.1.1405-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:f4495b4bfdf5dafdd808805392916c315dc01f8d9ffdd424a7aa92d25a575f65
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.2 MB (235214627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:456976f1d43a9964c94c5a4c87eba9ce3cc80fe07c52d77fe22ef60e56458152`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:25:53 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Wed, 16 Aug 2023 17:25:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Aug 2023 19:45:30 GMT
ENV CLOJURE_VERSION=1.11.1.1405
# Wed, 23 Aug 2023 19:45:30 GMT
WORKDIR /tmp
# Wed, 23 Aug 2023 19:45:44 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "e02966d807e5fcee40d3aeee823196fd296cb97e91746f444ac8c6681731b354 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 23 Aug 2023 19:45:45 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 23 Aug 2023 19:45:45 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 23 Aug 2023 19:45:45 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 23 Aug 2023 19:45:45 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4e1713a1018eae13a831df1ed9b8fd5e8788a4ef59b3f122c903b9e1c2857b`  
		Last Modified: Wed, 16 Aug 2023 17:34:20 GMT  
		Size: 143.5 MB (143538106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053b6a2a46f3b82116936f8fec786f6258970a51051ce8e6d5a409bd5b988755`  
		Last Modified: Wed, 23 Aug 2023 19:51:34 GMT  
		Size: 61.6 MB (61612687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6f2413d185720e689ba26a6505987e591000bd0f0ff65e8c56b02ebc35eb89`  
		Last Modified: Wed, 23 Aug 2023 19:51:28 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431f372a085c5b77ffda2324efe8733eedf35a36a92fb9c54a821dc7ef404f76`  
		Last Modified: Wed, 23 Aug 2023 19:51:29 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
