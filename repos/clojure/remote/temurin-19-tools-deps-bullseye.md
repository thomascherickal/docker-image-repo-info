## `clojure:temurin-19-tools-deps-bullseye`

```console
$ docker pull clojure@sha256:6d6a791b1e9a20decaa5cee6223cd06a4a74141c35e5ba4ccd2904e7d4845150
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-tools-deps-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:f62f8d7af79f980ccf2c3ede62ac86116c75f1f4498a723a3671410a96aa6bb5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.5 MB (303451837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2535045e6fece4b0993738764c7b6899064054f1cd0c289ef77a51b37fcb45c7`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:42 GMT
ADD file:26702ba2c3e94cb21cdb3c550cf01cf848823d160f3417b559116d4c718e5df0 in / 
# Tue, 25 Oct 2022 01:43:42 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:32:27 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 08 Nov 2022 19:50:54 GMT
COPY dir:fef581854733ec7202f8c807463b9e1952aeb6c7a002719c7e54987e50ea4dcb in /opt/java/openjdk 
# Tue, 08 Nov 2022 19:50:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Nov 2022 19:54:56 GMT
ENV CLOJURE_VERSION=1.11.1.1189
# Tue, 08 Nov 2022 19:54:56 GMT
WORKDIR /tmp
# Tue, 08 Nov 2022 19:55:13 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "1afd91b165776615eca84cce2271e5fe5d5818c55dee0f082b1304bb1464b3e8 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 08 Nov 2022 19:55:13 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 08 Nov 2022 19:55:14 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 08 Nov 2022 19:55:14 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 08 Nov 2022 19:55:14 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:17c9e6141fdb3387e5a1c07d4f9b6a05ac1498e96029fa3ea55470d4504f7770`  
		Last Modified: Tue, 25 Oct 2022 01:47:28 GMT  
		Size: 55.0 MB (55046332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7234d89610b4a16d903abead0c04715b2957b47183fec8ab6f88c4f3538cff68`  
		Last Modified: Tue, 08 Nov 2022 20:00:47 GMT  
		Size: 201.1 MB (201103429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1521aba6650c4a43f3a78f2d25c80117bc9b4d2814981262ddd3127192e571`  
		Last Modified: Tue, 08 Nov 2022 20:03:25 GMT  
		Size: 47.3 MB (47301058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4141e8d50d076add58aa0243ab5081aadc250317b47127d0e9c6e903667f89db`  
		Last Modified: Tue, 08 Nov 2022 20:03:20 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cca4c145ceeca42adeac34c560f40f45a0bf96b9d4aa7347ac9f9d1a46b813c`  
		Last Modified: Tue, 08 Nov 2022 20:03:20 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-tools-deps-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:e14a096a60196e6fb222b003eabd0c881395d68cdf4ce5b46b1c53e1400cdfb5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.9 MB (300861950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:167243091a03ad0dcbd8497c24ce87964ccda739a977002d37685686765c51ad`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 25 Oct 2022 05:45:55 GMT
ADD file:b16745ece8ef84c028d7e9ac4bf026ac64f885d4170bfcc9d435f237144a1b99 in / 
# Tue, 25 Oct 2022 05:45:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 23:53:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 08 Nov 2022 22:41:06 GMT
COPY dir:4138443eebfda1a2a245638d5bb568645bd34d79b66d39a3be31b5ac6b823d6d in /opt/java/openjdk 
# Tue, 08 Nov 2022 22:41:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Nov 2022 22:44:51 GMT
ENV CLOJURE_VERSION=1.11.1.1189
# Tue, 08 Nov 2022 22:44:51 GMT
WORKDIR /tmp
# Tue, 08 Nov 2022 22:45:03 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "1afd91b165776615eca84cce2271e5fe5d5818c55dee0f082b1304bb1464b3e8 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 08 Nov 2022 22:45:03 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 08 Nov 2022 22:45:03 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 08 Nov 2022 22:45:03 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 08 Nov 2022 22:45:04 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:8e1d92e7d04d2a9a9880cb45dc3c32c2805912cd86abed96d0ada3ff28748205`  
		Last Modified: Tue, 25 Oct 2022 05:48:40 GMT  
		Size: 53.7 MB (53701966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92032ad253d7bb165f3b1ac644f2177d86d0bf0dd878bdd484c4c281ba1a1b0a`  
		Last Modified: Tue, 08 Nov 2022 22:49:49 GMT  
		Size: 199.9 MB (199864415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9370e4303b04502ffa38dfb08cba7738ce13e7be0a3f6229eb09f1b58b2f820c`  
		Last Modified: Tue, 08 Nov 2022 22:51:45 GMT  
		Size: 47.3 MB (47294550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092373e3b09ad0d1251f070201247995374dc5b1fa6c1bea175510c8c40e7e24`  
		Last Modified: Tue, 08 Nov 2022 22:51:41 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225021faf28585e4d293f2277beabeb419647ced587ae79630ee46fcfc295466`  
		Last Modified: Tue, 08 Nov 2022 22:51:40 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
