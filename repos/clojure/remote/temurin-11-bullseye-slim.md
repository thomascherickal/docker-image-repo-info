## `clojure:temurin-11-bullseye-slim`

```console
$ docker pull clojure@sha256:98f84ea5c52ed89f00e94880d3ac2ba01cfcf394e1c7047116f256454b9aea54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:e5082c2a72659f8d5ce6f9b76e83b4133cc4e448cd0442e2977750875462a0d3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.8 MB (237751055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a1f688c102d2feba8bf227ec8bff9c6b476b1671655e3d7a1bf21bce3cb65ba`
-	Default Command: `["clj"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:07 GMT
ADD file:3d726bf0abbc08d6dda026cc406cdfb529deb60071641d164de28fcd62d1c1c0 in / 
# Thu, 27 Jul 2023 23:25:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:22:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 08 Aug 2023 20:19:21 GMT
COPY dir:071e7267c24117f41caea93a03f9d7c7d8dc1c681571e9b8f2b8b433c86f9778 in /opt/java/openjdk 
# Tue, 08 Aug 2023 22:30:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 14 Aug 2023 23:23:01 GMT
ENV CLOJURE_VERSION=1.11.1.1386
# Mon, 14 Aug 2023 23:23:01 GMT
WORKDIR /tmp
# Mon, 14 Aug 2023 23:23:18 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "3a09e2df4d3abd89b5b1286af0133a36a525ff3acfe1432f98b5c24b170940e8 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Mon, 14 Aug 2023 23:23:18 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Mon, 14 Aug 2023 23:23:18 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:1d5252f66ea9b661aceca1027b3d7ca259a50608261a25b51148119ecf086932`  
		Last Modified: Thu, 27 Jul 2023 23:30:08 GMT  
		Size: 31.4 MB (31417602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906a67c0c0e120eaa60971623d0bcdd60c592fdaff036504dc7443ce6dac2118`  
		Last Modified: Tue, 08 Aug 2023 20:23:28 GMT  
		Size: 144.8 MB (144831527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef81ef91bec0fe233a5eeacdfa24006ab8838fb1b7b7b03ebb0b234a19f8a996`  
		Last Modified: Mon, 14 Aug 2023 23:31:06 GMT  
		Size: 61.5 MB (61501308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64baf974c8d6a328b8d83880977a8bcc8af23e4e5738f73c62487e8a5a519293`  
		Last Modified: Mon, 14 Aug 2023 23:30:59 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:ae7e7fcb8761fcf3956abf8eecd65fc21d74c0bb90caadfe38fede51a5b93d67
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.2 MB (233243745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6d2e15a232807fcb1855a6fe6c111af1bf3781010c731b8945db56bcfa5d609`
-	Default Command: `["clj"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:15 GMT
ADD file:085ecd2f941de953afe5513a41a37412d72cbafd982de581ebd2309b3772b51e in / 
# Thu, 27 Jul 2023 23:43:15 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 14:25:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 08 Aug 2023 20:21:30 GMT
COPY dir:ddfd64e7bd36f630cd100cf454a9685f9fd0f9483467dbf7a4c9a71ab0af7089 in /opt/java/openjdk 
# Tue, 08 Aug 2023 20:21:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 20:26:40 GMT
ENV CLOJURE_VERSION=1.11.1.1347
# Tue, 08 Aug 2023 20:26:40 GMT
WORKDIR /tmp
# Tue, 08 Aug 2023 20:26:53 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "d9158bf3a1d92fbf8551656e47a86f42e93d10f1db9defa2124bfee206ce8c8f *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 08 Aug 2023 20:26:54 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 08 Aug 2023 20:26:54 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:795b5d192ab1819e75375fead3f2f931bd86046e3308224944f16a5ec3b97424`  
		Last Modified: Thu, 27 Jul 2023 23:47:14 GMT  
		Size: 30.1 MB (30062831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4618d52dbf5263b6400122ab8ead6b84fd0a5fdd684ed03f8e4a606dff09c08e`  
		Last Modified: Tue, 08 Aug 2023 20:32:48 GMT  
		Size: 141.6 MB (141565379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646642520f881897dc3b0dd9c09966972646dbb2ce0429fc2bb6c42aceeea6bc`  
		Last Modified: Tue, 08 Aug 2023 20:34:35 GMT  
		Size: 61.6 MB (61614917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e834ab0f8b7521de0135b837480bb23422658bf6e3ae44d7feecfdebc0f9b446`  
		Last Modified: Tue, 08 Aug 2023 20:34:27 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
