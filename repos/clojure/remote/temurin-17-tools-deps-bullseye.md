## `clojure:temurin-17-tools-deps-bullseye`

```console
$ docker pull clojure@sha256:34cb140f0b3e40156597c6cd8e843cb811e15f0b098e403c28fb3ebae2984d90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-tools-deps-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:fb659e4665596c8ba96bc5968f9d5ff5ba9c250fbc96cf4b3a325624844f267e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.5 MB (319510606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b19d869122feb7e802d710faab739ad54395a39a052c05e9a376b72490a1cbee`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:09 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 14:58:53 GMT
COPY dir:05dd898ce921dff423e175db4bfabc77c7b70b060cfa18a18ee060c7533c567b in /opt/java/openjdk 
# Thu, 04 May 2023 14:58:53 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 15:01:17 GMT
ENV CLOJURE_VERSION=1.11.1.1273
# Thu, 04 May 2023 15:01:17 GMT
WORKDIR /tmp
# Thu, 04 May 2023 15:01:33 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4938afe6c0690d2a6553141857742d94a7350c02b4fa57cd6a9c1b7cbe66492e *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 04 May 2023 15:01:34 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 04 May 2023 15:01:34 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Thu, 04 May 2023 15:01:34 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 04 May 2023 15:01:34 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cbada72a4382332aa6aa78d824d0bdddefea4c233d0617f4e8924c1c87446c9`  
		Last Modified: Thu, 04 May 2023 15:09:12 GMT  
		Size: 192.6 MB (192580390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed29d12a05b1e47de9f144252cbbe4f6137c6ff18ca84b4b9bb626129e54c1a`  
		Last Modified: Thu, 04 May 2023 15:10:54 GMT  
		Size: 71.9 MB (71880135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4bfba0672406f26fe08f4898e906f6d1ffccf136a65ad55e1aee0aa5d6991a`  
		Last Modified: Thu, 04 May 2023 15:10:46 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bab39df7d311efd595f6cab9cfa468580ea69d6a9241a8a7d5966508ae5b9c8`  
		Last Modified: Thu, 04 May 2023 15:10:46 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-tools-deps-bullseye` - linux; arm64 variant v8

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
