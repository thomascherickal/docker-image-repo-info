## `clojure:temurin-17-tools-deps-bullseye`

```console
$ docker pull clojure@sha256:280728676099dd56b4bc7f8f19a1a97efea63f7ee38c22591b15cc5232a9e80a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-tools-deps-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:0cb6ce0599e5a07ffe1c441098f68fca32233ff9a9447097c7329fe4a47b7f3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.7 MB (271711382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:544c51b9ca754fab4ac212cd4962b384bab0baa0f91c2136416440c0c1bf9f98`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:57 GMT
ADD file:20f89ff93bfbd6c9fb1a97058a1f3de4485a8974e8a83892072c511fbd2e4134 in / 
# Wed, 16 Aug 2023 00:59:58 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:06 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 31 Aug 2023 23:31:16 GMT
COPY dir:6777d1f77166c2ecdd8f4eb23f5fd82574aa8a90fd65d6dff981fbb31778a3d1 in /opt/java/openjdk 
# Thu, 31 Aug 2023 23:31:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 31 Aug 2023 23:37:43 GMT
ENV CLOJURE_VERSION=1.11.1.1413
# Thu, 31 Aug 2023 23:37:43 GMT
WORKDIR /tmp
# Thu, 31 Aug 2023 23:37:59 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "ad9aa1e99c59a4f7eb66450914fbec543337d9fada60dd9d34eec7fe18ae4965 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 31 Aug 2023 23:38:00 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 31 Aug 2023 23:38:00 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Thu, 31 Aug 2023 23:38:00 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 31 Aug 2023 23:38:00 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:6a70103cc499a199e10e379794c60aa524d9598587cc2bdfe2995642c2da8df7`  
		Last Modified: Wed, 16 Aug 2023 01:04:50 GMT  
		Size: 55.1 MB (55056621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a114598ad33aed6a505f38365243af34f1e10fad82e78b36362b08851483a7`  
		Last Modified: Thu, 31 Aug 2023 23:44:21 GMT  
		Size: 144.8 MB (144775748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a018a230f79b13e9a1d8fdf80a29103537b88dd6637e03c6f3ff10c4c928a24d`  
		Last Modified: Thu, 31 Aug 2023 23:46:51 GMT  
		Size: 71.9 MB (71878000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ae22f6782b54b8dc2eb9861d28f69e5f2292ec08fbde2b4009452b04e6346d`  
		Last Modified: Thu, 31 Aug 2023 23:46:43 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3f9fe43738210b7847cebf74f6fc2b809b7c6a045651ecf22bf0aa41839c75`  
		Last Modified: Thu, 31 Aug 2023 23:46:43 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-tools-deps-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:6febc48d78ffbff7bab49b17ab82ae0fb59b183e33eec8aa86315da3fbbaad4b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.2 MB (269247053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbca2de04615f196b099515fab55d25ee1219144560ff9d0a56974184d3607ca`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:03 GMT
ADD file:8973cddb2d84a543b71001635599951bea6485a3526ae4ff916443b584864c83 in / 
# Tue, 15 Aug 2023 23:40:04 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:14 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Sep 2023 01:47:28 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Sat, 02 Sep 2023 01:47:31 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Sep 2023 01:49:37 GMT
ENV CLOJURE_VERSION=1.11.1.1413
# Sat, 02 Sep 2023 01:49:37 GMT
WORKDIR /tmp
# Sat, 02 Sep 2023 01:49:51 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "ad9aa1e99c59a4f7eb66450914fbec543337d9fada60dd9d34eec7fe18ae4965 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Sat, 02 Sep 2023 01:49:52 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Sat, 02 Sep 2023 01:49:52 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Sat, 02 Sep 2023 01:49:52 GMT
ENTRYPOINT ["entrypoint"]
# Sat, 02 Sep 2023 01:49:52 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:e837d9f05c625de5b814b851adbc03559ba02ea7078f57c81a01e18fc65bf42b`  
		Last Modified: Tue, 15 Aug 2023 23:43:37 GMT  
		Size: 53.7 MB (53704779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c782a1c2165dbdac384abd088ebc99d9f013b55fa39e22661861b6b10083b60`  
		Last Modified: Sat, 02 Sep 2023 01:55:28 GMT  
		Size: 143.5 MB (143543490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f0abc7e257ecccb3255aeeff9edab7864b279263e5a15948e422bcd62b4c2a`  
		Last Modified: Sat, 02 Sep 2023 01:57:02 GMT  
		Size: 72.0 MB (71997768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd76f79d0cf59e6f65f1df3fc198bd95267efd4dc6285cc91ef21edb3ad4c68a`  
		Last Modified: Sat, 02 Sep 2023 01:56:55 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147ecffdccfd1fc5156e85e078b02dea0dc3c48b6d0d52f081d2b9fdb4dd3ad0`  
		Last Modified: Sat, 02 Sep 2023 01:56:55 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
