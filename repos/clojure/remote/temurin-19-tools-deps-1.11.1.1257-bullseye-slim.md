## `clojure:temurin-19-tools-deps-1.11.1.1257-bullseye-slim`

```console
$ docker pull clojure@sha256:6535b4343c69d69d177ef6e2d4fafe46d3b9b89b18badb2d930e7b3ef25fcbbb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-tools-deps-1.11.1.1257-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:b930f8dc53c64cbebe232d8fed9b6dc05dfdec04c7e882697cfdb33bbc32a0ec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.0 MB (294015054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:316944a984542b97ea9afa48aed4fff834f957b9c2687255880c0f6071c397d2`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:41:22 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Mar 2023 07:50:20 GMT
COPY dir:94cb5af8175285c10c94286222d8a35302f3f8c290e00011a75c67156659d6ab in /opt/java/openjdk 
# Wed, 01 Mar 2023 07:50:22 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 20:26:59 GMT
ENV CLOJURE_VERSION=1.11.1.1257
# Thu, 16 Mar 2023 20:26:59 GMT
WORKDIR /tmp
# Thu, 16 Mar 2023 20:27:15 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "be032cf21dc67ecf072f7254a01c3587d97aa311198f53cd1a1777ddfb3e9244 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 16 Mar 2023 20:27:16 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 16 Mar 2023 20:27:16 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Thu, 16 Mar 2023 20:27:16 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 16 Mar 2023 20:27:16 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b3ccae27fe03c16494d3c8f769e2249b243d16240726cb9587a989c25ac8d0`  
		Last Modified: Wed, 01 Mar 2023 08:01:12 GMT  
		Size: 201.1 MB (201112994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a979a3fa1f3e87e27c15810b8641d849cb755b0e32b25f2f4ad10fc043a5c5b`  
		Last Modified: Thu, 16 Mar 2023 20:37:41 GMT  
		Size: 61.5 MB (61489638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f31b997d200a66c52b8291eabe9fe7833b2a7eb4be2497a27fbc803b16730d1e`  
		Last Modified: Thu, 16 Mar 2023 20:37:34 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38ebcf9d6c427ece0de3262c99e82346e19dfef3086f0c1f5c4f6c1bbb88542`  
		Last Modified: Thu, 16 Mar 2023 20:37:34 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-tools-deps-1.11.1.1257-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:34a9d2994530648f2e0a1f76f6ba767ebf0b4074c33112c65e32ccbaa2d1b373
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.5 MB (291523691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edab81b4c8b9388f256b6112e279822c3d28b686d0046a0135f3113bcbf2546c`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:02:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Mar 2023 03:09:45 GMT
COPY dir:9a6a873ca11063f6f04e7f088397a1fce771e2b1aa8590b72eb07158cfac883f in /opt/java/openjdk 
# Wed, 01 Mar 2023 03:09:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 19:45:24 GMT
ENV CLOJURE_VERSION=1.11.1.1257
# Thu, 16 Mar 2023 19:45:24 GMT
WORKDIR /tmp
# Thu, 16 Mar 2023 19:45:38 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "be032cf21dc67ecf072f7254a01c3587d97aa311198f53cd1a1777ddfb3e9244 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 16 Mar 2023 19:45:38 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 16 Mar 2023 19:45:38 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Thu, 16 Mar 2023 19:45:38 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 16 Mar 2023 19:45:38 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee23dab4c9395b25d6fc9f10fb3db021a5fb12f2747057b25dfcd66add5df0fd`  
		Last Modified: Wed, 01 Mar 2023 03:19:32 GMT  
		Size: 199.9 MB (199855200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f0363c9460fe935b5effd223a4fd3871bcd0bcf9facb68481976290ec2fc98`  
		Last Modified: Thu, 16 Mar 2023 19:54:05 GMT  
		Size: 61.6 MB (61604659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96288411fed664f04a73679bdb601053d2519cba21ecfa486decf79333225d8e`  
		Last Modified: Thu, 16 Mar 2023 19:53:59 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec4625ac341971fd83f7c4924fff4b05ab6d7fd7babeb8c75db62e8988dc3ae`  
		Last Modified: Thu, 16 Mar 2023 19:53:59 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
