## `clojure:temurin-11-tools-deps-1.11.1.1347-bullseye-slim`

```console
$ docker pull clojure@sha256:3b7be7e350145fc206534c1c556d61e12b5c77baeab5bb6ae0f82d6637ca6433
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-tools-deps-1.11.1.1347-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:3a8313b2483a03fdecf9ded7d01ca1f1f764c8ebebfb164686585a4d3c46892d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.5 MB (291463495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1158fc3c2d615ae000c703db06e543473dbd48d813593b8ec9ad6be17cb1e0a7`
-	Default Command: `["clj"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:44:37 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 03:47:29 GMT
COPY dir:99fc054d8f67589023f9478fc6ae691114aff76e696d34d4988a30c767727d32 in /opt/java/openjdk 
# Tue, 13 Jun 2023 03:47:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 03:49:15 GMT
ENV CLOJURE_VERSION=1.11.1.1347
# Tue, 13 Jun 2023 03:49:15 GMT
WORKDIR /tmp
# Tue, 13 Jun 2023 03:49:31 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "d9158bf3a1d92fbf8551656e47a86f42e93d10f1db9defa2124bfee206ce8c8f *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 13 Jun 2023 03:49:31 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 13 Jun 2023 03:49:31 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c93dc0976ab0e1cedf14e59a533cbc8c624427cdfc4ff4080297f31ee3a366`  
		Last Modified: Tue, 13 Jun 2023 03:57:23 GMT  
		Size: 198.5 MB (198549694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0ac7f426cd91130857a0f6027c9b1224168094b119db59b5b647d6ceb3e016`  
		Last Modified: Tue, 13 Jun 2023 03:58:18 GMT  
		Size: 61.5 MB (61495777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a1d8c57e76a1b43f6e02f4e171d8b39d6e8d030be081b822e80ec8c923ba9f`  
		Last Modified: Tue, 13 Jun 2023 03:58:11 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-tools-deps-1.11.1.1347-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:e5839198ab9307bafa5d12f7291d4a7f9e430d40eb386c970fe3db6df09ac142
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.0 MB (286999173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8888b55f1eeb2daa0e5eec271d5e2de1f8bb590821a153c945489be1f6c9d08b`
-	Default Command: `["clj"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:28:47 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 04:42:21 GMT
COPY dir:e9846f499a157c7a78a7ddb1d6b9ebc67065c65b65eb611ad6978501e8452ab7 in /opt/java/openjdk 
# Fri, 16 Jun 2023 04:42:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 04:45:37 GMT
ENV CLOJURE_VERSION=1.11.1.1347
# Fri, 16 Jun 2023 04:45:37 GMT
WORKDIR /tmp
# Fri, 16 Jun 2023 04:45:51 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "d9158bf3a1d92fbf8551656e47a86f42e93d10f1db9defa2124bfee206ce8c8f *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 16 Jun 2023 04:45:52 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 16 Jun 2023 04:45:52 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f561dc152f6d05a1820783d780247855889a7f67c10ad93e662c845bc4e04b7`  
		Last Modified: Fri, 16 Jun 2023 04:54:22 GMT  
		Size: 195.3 MB (195324188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a3d89f0ec7ff7f0b0030f7fc2085f131ead3836e6c10b1ab5c395e729858b9`  
		Last Modified: Fri, 16 Jun 2023 04:56:03 GMT  
		Size: 61.6 MB (61611536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb2b949a3a8470588ceb527c4b1c91634282336f8544739c895d1b8095c23f3`  
		Last Modified: Fri, 16 Jun 2023 04:55:56 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
