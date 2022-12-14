## `clojure:temurin-19-tools-deps-bullseye`

```console
$ docker pull clojure@sha256:b758838248758793b5810e731ce4aa901ed48f240192110b7694ef52249ff332
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-tools-deps-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:038a83cdbcee043764d178171aee651a066754ba98f0b1465208002188e74dba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.5 MB (303450209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9a89efcefb2b15a18379d6bb774f19245f530f5485fb72b4d5c65f64c24e446`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:41 GMT
ADD file:553d20b03d45305e58cde07e0c259421bba044155ac90b4559e5cc0b69093347 in / 
# Tue, 06 Dec 2022 01:20:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:48:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 06 Dec 2022 01:57:42 GMT
COPY dir:fef581854733ec7202f8c807463b9e1952aeb6c7a002719c7e54987e50ea4dcb in /opt/java/openjdk 
# Tue, 06 Dec 2022 01:57:44 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Dec 2022 00:24:31 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Wed, 14 Dec 2022 00:24:31 GMT
WORKDIR /tmp
# Wed, 14 Dec 2022 00:24:47 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 14 Dec 2022 00:24:48 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 14 Dec 2022 00:24:48 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 14 Dec 2022 00:24:48 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 14 Dec 2022 00:24:48 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698`  
		Last Modified: Tue, 06 Dec 2022 01:24:48 GMT  
		Size: 55.0 MB (55041342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5290555b9fd520933dc8e0c6563f92fd2a2cfc886a885094d2288c04a01ae4`  
		Last Modified: Tue, 06 Dec 2022 02:09:00 GMT  
		Size: 201.1 MB (201103430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf23c9033c575cecabaf5b70020ce6a3221f83d0b77bd142e6edc98cf5fa3ff`  
		Last Modified: Wed, 14 Dec 2022 00:31:53 GMT  
		Size: 47.3 MB (47304419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f7c09d376723b7207294ac25ebfc46a70a15035db1e2e9359f81255c4dd944`  
		Last Modified: Wed, 14 Dec 2022 00:31:47 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c6bff253c13e0bab3fcee323a7203c20bbf94163060efe0c68e4edcdf24f8d`  
		Last Modified: Wed, 14 Dec 2022 00:31:47 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-tools-deps-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:9d260336222b804768b4f36fe3b19d95d2cd066f8a71bb10e9d76f77a4aae8e9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.9 MB (300858940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8f81e30eef492775911b54063a4b2291108ad3647e85adf9dfd70cbfaf3d0c4`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:06 GMT
ADD file:b1e7652678bbfc9556636e77d79c947ff1436888e2929f9c5c3ddb42a50c1176 in / 
# Tue, 06 Dec 2022 01:40:07 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:15 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 06 Dec 2022 02:24:58 GMT
COPY dir:4138443eebfda1a2a245638d5bb568645bd34d79b66d39a3be31b5ac6b823d6d in /opt/java/openjdk 
# Tue, 06 Dec 2022 02:25:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Dec 2022 00:43:06 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Wed, 14 Dec 2022 00:43:06 GMT
WORKDIR /tmp
# Wed, 14 Dec 2022 00:43:18 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 14 Dec 2022 00:43:18 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 14 Dec 2022 00:43:18 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 14 Dec 2022 00:43:18 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 14 Dec 2022 00:43:19 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:4948a51a9a3f176f30ac619014f4a2da453a943244eacb53096ee9742eb7cef1`  
		Last Modified: Tue, 06 Dec 2022 01:43:33 GMT  
		Size: 53.7 MB (53699146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cabaaf976f2d5c56a302b35a76e1a18a5cb39245bb9fc93db9557a6e3e5f0b9`  
		Last Modified: Tue, 06 Dec 2022 02:35:02 GMT  
		Size: 199.9 MB (199864416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae6f5a3124fa0a1308a35390edf912765881abd3b0b3f4e32fdeee6cc3dfc9b6`  
		Last Modified: Wed, 14 Dec 2022 00:49:27 GMT  
		Size: 47.3 MB (47294361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ac69824e5ccefe794377bab9308df7f99d5b2e85ca78dd61e61dedf1f8790a`  
		Last Modified: Wed, 14 Dec 2022 00:49:21 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06cb6738d85c41ce9531b048aef61a6c2455b255ff3f0fb4387dc4c89de9bfc0`  
		Last Modified: Wed, 14 Dec 2022 00:49:21 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
