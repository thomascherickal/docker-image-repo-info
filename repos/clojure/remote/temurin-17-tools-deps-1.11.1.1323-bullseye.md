## `clojure:temurin-17-tools-deps-1.11.1.1323-bullseye`

```console
$ docker pull clojure@sha256:3bcfb305e57032ed7ebc7b73d7134cabfa598e7abca0007206dd853a2a5354c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `clojure:temurin-17-tools-deps-1.11.1.1323-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:927bb51eece1300a7d669299b715fd423ff455e8c418fc4ad07873a60d6fbe1f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.1 MB (317076134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9210d16f747ed7d17041a3341be96228a34c7abbe7ad9f6156ee3c36ba384e9`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 03 May 2023 00:22:41 GMT
ADD file:f930fdb659332a615b0042ca415d6d7feda9ba6b2f58222e3e5bbed326db4d40 in / 
# Wed, 03 May 2023 00:22:42 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:43:29 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 10:13:41 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Thu, 04 May 2023 10:13:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 19 May 2023 19:49:23 GMT
ENV CLOJURE_VERSION=1.11.1.1323
# Fri, 19 May 2023 19:49:23 GMT
WORKDIR /tmp
# Fri, 19 May 2023 19:49:36 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "c4666f0e2c2397b91554befd71ff6149b2e89acbf90400e1dcf557526cfb593d *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 19 May 2023 19:49:37 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 19 May 2023 19:49:37 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 19 May 2023 19:49:37 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 19 May 2023 19:49:37 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:d677c78be691f8dcbe9d44ce576b97ad205b3dd78557dc62794e59eb19553ee9`  
		Last Modified: Wed, 03 May 2023 00:25:31 GMT  
		Size: 53.7 MB (53692705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11090c6457d65efbe72f084b567111755856da82721e52490ffc8bec9b85abff`  
		Last Modified: Thu, 04 May 2023 10:22:02 GMT  
		Size: 191.4 MB (191387646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:163b8ca8ccd97c0154a6f87cb2bf8cdb0a297123b6ad65d9d52355cb16653339`  
		Last Modified: Fri, 19 May 2023 19:58:06 GMT  
		Size: 72.0 MB (71994767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f883199bc47e604bbe86ea515d2f9f9f018f978d9ac5990d679fc16256948b`  
		Last Modified: Fri, 19 May 2023 19:57:59 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90fb49b5011216d91a7fe5c50f714121f4e6d4a579557581ee7d98348fbfcacb`  
		Last Modified: Fri, 19 May 2023 19:57:59 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
