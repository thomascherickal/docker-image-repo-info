## `clojure:temurin-11-tools-deps-bullseye`

```console
$ docker pull clojure@sha256:dfb043225cefac2447c696fdb9cc4693953a09695e19dd247baf5eb512c56463
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-tools-deps-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:453d8e95af6180957c97ba6c7dd1f9a9e6dd2f5d55a8296b08ad5ed21e94a104
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.8 MB (300800997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9e5705125c659e9c518c26626639e7d8d15f52f88f9e0282bdf6df7eca0e8ba`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:41 GMT
ADD file:553d20b03d45305e58cde07e0c259421bba044155ac90b4559e5cc0b69093347 in / 
# Tue, 06 Dec 2022 01:20:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:48:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:36:17 GMT
COPY dir:a503569ef9354f7d11d0273f2ab0ff91f3e5c47f548dc54f07c58e44ff27a8a0 in /opt/java/openjdk 
# Fri, 09 Dec 2022 06:36:19 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Dec 2022 00:21:45 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Wed, 14 Dec 2022 00:21:45 GMT
WORKDIR /tmp
# Wed, 14 Dec 2022 00:22:02 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 14 Dec 2022 00:22:02 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 14 Dec 2022 00:22:03 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698`  
		Last Modified: Tue, 06 Dec 2022 01:24:48 GMT  
		Size: 55.0 MB (55041342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561532e76f8a67e2ac0114bf68c5fcb2c640ceb1eff7b0f331d366e73f673768`  
		Last Modified: Fri, 09 Dec 2022 06:53:29 GMT  
		Size: 198.5 MB (198454561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad34a0c44a5e6416fa23422a7d008036b39fd02141650df4ff714d8aa0675069`  
		Last Modified: Wed, 14 Dec 2022 00:29:31 GMT  
		Size: 47.3 MB (47304475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee510fb3ee0eebcb4cc54e7ef486804c9fff56ceec6e0f14226c1fd61c71118`  
		Last Modified: Wed, 14 Dec 2022 00:29:25 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-tools-deps-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:c2a656163e956654c61b664847e8dfcfd87a6b40ce9334c14c7f32cd4fc1695f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.2 MB (296197588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd8ebd8a1664d8f38a98b6db52360d186888e433481aeb75406cce0122d6ce9f`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:06 GMT
ADD file:b1e7652678bbfc9556636e77d79c947ff1436888e2929f9c5c3ddb42a50c1176 in / 
# Tue, 06 Dec 2022 01:40:07 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:15 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 05:03:32 GMT
COPY dir:e387a3b68139ff88bdac27d5ce097fc680f3cae9fdd88c28cdd91a06f9205180 in /opt/java/openjdk 
# Fri, 09 Dec 2022 05:03:36 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Dec 2022 00:40:53 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Wed, 14 Dec 2022 00:40:53 GMT
WORKDIR /tmp
# Wed, 14 Dec 2022 00:41:06 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 14 Dec 2022 00:41:06 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 14 Dec 2022 00:41:06 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:4948a51a9a3f176f30ac619014f4a2da453a943244eacb53096ee9742eb7cef1`  
		Last Modified: Tue, 06 Dec 2022 01:43:33 GMT  
		Size: 53.7 MB (53699146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1dc93c936f130a0b32765e5801ad37ff3679f9461520ae91ce9b6fa4d65888`  
		Last Modified: Fri, 09 Dec 2022 05:18:13 GMT  
		Size: 195.2 MB (195203416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96ce753eb9e3a5a4212d0f4b7bd52bac909190c8d3d201e330183f4c4cd0acf`  
		Last Modified: Wed, 14 Dec 2022 00:47:22 GMT  
		Size: 47.3 MB (47294408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139618d056b8830baff06e4a8b342b868e8d21668cc54c3526c2b8f86372120d`  
		Last Modified: Wed, 14 Dec 2022 00:47:17 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
