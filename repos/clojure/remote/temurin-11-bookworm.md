## `clojure:temurin-11-bookworm`

```console
$ docker pull clojure@sha256:500d619e584ef95250538a3d2073bb27374c6cb3c12663b661449fed8e845eae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-bookworm` - linux; amd64

```console
$ docker pull clojure@sha256:b967a18068459353f01c526bd693c934d7af0c42c21895b63cce54769936d028
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.8 MB (277774252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1895b72ad3bc801315d36bf3df8ce1799a10d090d68033a378eee3e65b065271`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:37 GMT
ADD file:1e4dd5dab602337b5d5ef8d84b8dbe8b1ac62225f077b29b27d045842486d8e2 in / 
# Wed, 11 Oct 2023 18:34:37 GMT
CMD ["bash"]
# Fri, 13 Oct 2023 01:26:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 12:43:54 GMT
COPY dir:2526dfaf6aedccef54b8de2f87890e86c6d3fe8431985d8e74dcfc29195b01ed in /opt/java/openjdk 
# Fri, 13 Oct 2023 12:43:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 12:49:35 GMT
ENV CLOJURE_VERSION=1.11.1.1413
# Fri, 13 Oct 2023 12:49:35 GMT
WORKDIR /tmp
# Fri, 13 Oct 2023 12:49:58 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "ad9aa1e99c59a4f7eb66450914fbec543337d9fada60dd9d34eec7fe18ae4965 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 13 Oct 2023 12:49:58 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 13 Oct 2023 12:49:58 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:0a9573503463fd3166b5b1f34a7720dac28609e98d731e50e7068f92e79b8545`  
		Last Modified: Wed, 11 Oct 2023 18:39:10 GMT  
		Size: 49.6 MB (49582224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:312f54f99658b0b7990d26fe3799c0af7d535f77af55acd1d748d19013cad478`  
		Last Modified: Fri, 13 Oct 2023 13:04:52 GMT  
		Size: 144.8 MB (144826232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfacf647629ef0408692ca20bfd3b00c93794658a9c49343a706668c0de7f790`  
		Last Modified: Fri, 13 Oct 2023 13:07:52 GMT  
		Size: 83.4 MB (83365179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39af33eeb80ea50f3f3a957232fb91594d6109f967eaf2bfc867d844b7e7b5af`  
		Last Modified: Fri, 13 Oct 2023 13:07:42 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-bookworm` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:df0f91341c4eb68b4c05c556ce911128140257db85e37576adb38f48e52fb323
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.3 MB (274301885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30134398ef69eb3ab3074079a8907935bcb85ae4b139808c29417b72b0917333`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:43 GMT
ADD file:bf4264671bd91eb30c67d512144ebcf7f5c55a3e490ebe7876fa9b20d433bf7b in / 
# Wed, 11 Oct 2023 18:24:44 GMT
CMD ["bash"]
# Fri, 13 Oct 2023 00:57:54 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 10:12:02 GMT
COPY dir:b4903e9e1c2782550c5bca9cb7b0f840b4fdb810848e07ca44af328ac9dd84f6 in /opt/java/openjdk 
# Fri, 13 Oct 2023 10:12:05 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 10:16:44 GMT
ENV CLOJURE_VERSION=1.11.1.1413
# Fri, 13 Oct 2023 10:16:44 GMT
WORKDIR /tmp
# Fri, 13 Oct 2023 10:17:05 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "ad9aa1e99c59a4f7eb66450914fbec543337d9fada60dd9d34eec7fe18ae4965 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 13 Oct 2023 10:17:05 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 13 Oct 2023 10:17:05 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:e720f94321d63ecb6efa873b294dce7eaa1c3a5ddcd5bf7daddf375b955669a4`  
		Last Modified: Wed, 11 Oct 2023 18:28:04 GMT  
		Size: 49.6 MB (49612578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bf03c8b0dce1ee3013ef26db39e3fea7b1e7c57443f42116088217a57392c8`  
		Last Modified: Fri, 13 Oct 2023 10:29:26 GMT  
		Size: 141.6 MB (141570586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7218b518f04ee66faeeaa5ac428caab169d6e7a4d9defca6b669139f7bb9a6`  
		Last Modified: Fri, 13 Oct 2023 10:32:07 GMT  
		Size: 83.1 MB (83118104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bac2f02140dc880dd33823d42e76771b091a1519eebb84a36cf0bfd0b832104`  
		Last Modified: Fri, 13 Oct 2023 10:31:59 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
