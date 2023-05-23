## `clojure:temurin-17-tools-deps-1.11.1.1323-bullseye-slim`

```console
$ docker pull clojure@sha256:2ca49b3fee7c836ecd0fecd34f8939a0eae1ddd71541ae084c1859a3b2850dfd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-tools-deps-1.11.1.1323-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:b99f755e014f0c90fb6577d91f30f60b79f0e93dd2309b1359f9e0d9f633e760
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.5 MB (285480065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47e9cebabed149e9cb7f55af471e4022f17e7e9fd328a6ef0dbb4bcd6e88c290`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 14:59:25 GMT
COPY dir:05dd898ce921dff423e175db4bfabc77c7b70b060cfa18a18ee060c7533c567b in /opt/java/openjdk 
# Thu, 04 May 2023 14:59:27 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 19 May 2023 20:31:54 GMT
ENV CLOJURE_VERSION=1.11.1.1323
# Fri, 19 May 2023 20:31:54 GMT
WORKDIR /tmp
# Fri, 19 May 2023 20:32:10 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "c4666f0e2c2397b91554befd71ff6149b2e89acbf90400e1dcf557526cfb593d *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 19 May 2023 20:32:10 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 19 May 2023 20:32:10 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 19 May 2023 20:32:11 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 19 May 2023 20:32:11 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21fd2caa057611d1671449088801d8f3e11973cc523e65f79f2b73f9189938c0`  
		Last Modified: Thu, 04 May 2023 15:09:34 GMT  
		Size: 192.6 MB (192580382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1df3a6614badf5f3d9fe4f6d657e25880e1bcc23d951163b6d5d611d9d7351f`  
		Last Modified: Fri, 19 May 2023 20:42:47 GMT  
		Size: 61.5 MB (61495152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d974c611bd88df3bbfc5735e219e16aba4920271ee0730822d50dc5dcaa292`  
		Last Modified: Fri, 19 May 2023 20:42:40 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b912aeaedfbf110e6d189ccd05266f0877d41621dbdfa00f86dea53149bfa78`  
		Last Modified: Fri, 19 May 2023 20:42:40 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-tools-deps-1.11.1.1323-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:420a6d80d3c0ee4d30de9b2c5346314ac316f4d42ffe2c418d1d0dc7bf2abcf4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.0 MB (283049841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:365e3fb519b46da7cd829927cf3cb89bd7818392ca47117c4c87b662a0379245`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:24:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 23 May 2023 01:29:51 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Tue, 23 May 2023 01:29:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 01:31:22 GMT
ENV CLOJURE_VERSION=1.11.1.1323
# Tue, 23 May 2023 01:31:22 GMT
WORKDIR /tmp
# Tue, 23 May 2023 01:31:35 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "c4666f0e2c2397b91554befd71ff6149b2e89acbf90400e1dcf557526cfb593d *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 23 May 2023 01:31:36 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 23 May 2023 01:31:36 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 23 May 2023 01:31:36 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 23 May 2023 01:31:36 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04300dd851e66af00281d635f3fa075517249f6b42bf7ebe21fbbe2828ef53bd`  
		Last Modified: Tue, 23 May 2023 01:37:21 GMT  
		Size: 191.4 MB (191387691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e37e5e0d92be928063c51204a3eb6662d1a99fcfe1f89d1f0409640bc7ace70`  
		Last Modified: Tue, 23 May 2023 01:38:17 GMT  
		Size: 61.6 MB (61608386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d1bdb461cb63a2333306a7f8cb3c734772e9eddba3d8e585c1aa98e9b1f226`  
		Last Modified: Tue, 23 May 2023 01:38:11 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38db61b82804e9cb7899efbef3f4f378eb7c5b49ccaf2e6b839f32cf0efa48b`  
		Last Modified: Tue, 23 May 2023 01:38:11 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
