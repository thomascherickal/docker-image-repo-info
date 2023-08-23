## `clojure:temurin-11-tools-deps-1.11.1.1405-bullseye`

```console
$ docker pull clojure@sha256:978765603e72e04e4e4316a0856d85b8fd433f5ba9296842b2f22f8310efb7cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-tools-deps-1.11.1.1405-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:8179ed8b38750cf2030e78ad6e30d94ada3755b51d85e9965786feea3f61caca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.8 MB (271768771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1365e9f49d50c373e0bde5c1240d5075664fbd22a3847d35b25a59e46c774953`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:57 GMT
ADD file:20f89ff93bfbd6c9fb1a97058a1f3de4485a8974e8a83892072c511fbd2e4134 in / 
# Wed, 16 Aug 2023 00:59:58 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:06 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 18:04:32 GMT
COPY dir:72d046f3e284b8eca8066a837ab8a68f91b4cf5355de7f6803a8ee9b7ce3d682 in /opt/java/openjdk 
# Wed, 16 Aug 2023 18:04:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Aug 2023 20:24:47 GMT
ENV CLOJURE_VERSION=1.11.1.1405
# Wed, 23 Aug 2023 20:24:47 GMT
WORKDIR /tmp
# Wed, 23 Aug 2023 20:25:04 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "e02966d807e5fcee40d3aeee823196fd296cb97e91746f444ac8c6681731b354 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 23 Aug 2023 20:25:04 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 23 Aug 2023 20:25:05 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:6a70103cc499a199e10e379794c60aa524d9598587cc2bdfe2995642c2da8df7`  
		Last Modified: Wed, 16 Aug 2023 01:04:50 GMT  
		Size: 55.1 MB (55056621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802f7c61301eef1eb08be64b58b246c8d0994f99e572b694d6cd34c52442c978`  
		Last Modified: Wed, 16 Aug 2023 18:15:30 GMT  
		Size: 144.8 MB (144831648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1703537694a75994c831536dddcb92249d4abfa7386ab8c7da6d475bf879a730`  
		Last Modified: Wed, 23 Aug 2023 20:32:48 GMT  
		Size: 71.9 MB (71879884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46d83c7bacac33cb4b68a5b72e7ae5b78d91714de6a49bc09a8aa126a8699013`  
		Last Modified: Wed, 23 Aug 2023 20:32:40 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-tools-deps-1.11.1.1405-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:6e2e3a748c80de741bffe29871d91fa0a5f2a7b02481b3d9a0edba1e8495d95e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.3 MB (267269346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:736e232a760da1839cbc8313873494fe4fb8b466d5ba6c698a4433dc1a7d0ef7`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:03 GMT
ADD file:8973cddb2d84a543b71001635599951bea6485a3526ae4ff916443b584864c83 in / 
# Tue, 15 Aug 2023 23:40:04 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:14 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:21:45 GMT
COPY dir:6acc55ac013a722a8db4af8f0ce8de9270cd9aeb372e6c734b449d15adcc5218 in /opt/java/openjdk 
# Wed, 16 Aug 2023 17:21:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Aug 2023 19:43:47 GMT
ENV CLOJURE_VERSION=1.11.1.1405
# Wed, 23 Aug 2023 19:43:47 GMT
WORKDIR /tmp
# Wed, 23 Aug 2023 19:44:01 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "e02966d807e5fcee40d3aeee823196fd296cb97e91746f444ac8c6681731b354 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 23 Aug 2023 19:44:02 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 23 Aug 2023 19:44:02 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:e837d9f05c625de5b814b851adbc03559ba02ea7078f57c81a01e18fc65bf42b`  
		Last Modified: Tue, 15 Aug 2023 23:43:37 GMT  
		Size: 53.7 MB (53704779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:175ec2cb09b3952032a7dbf0cdc9f641b1c5035ea846b712b44240d849a2979f`  
		Last Modified: Wed, 16 Aug 2023 17:31:34 GMT  
		Size: 141.6 MB (141565216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc46588f67c29ca7542a63ea3404dd624c31a50f12db2ca87b9b65766c2272d0`  
		Last Modified: Wed, 23 Aug 2023 19:49:58 GMT  
		Size: 72.0 MB (71998733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c967b2f42bdb136e49d71660db45e3bc93fab18462040bd74a9b05f9d8053a8f`  
		Last Modified: Wed, 23 Aug 2023 19:49:48 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
