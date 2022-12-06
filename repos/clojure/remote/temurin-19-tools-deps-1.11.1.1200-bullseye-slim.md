## `clojure:temurin-19-tools-deps-1.11.1.1200-bullseye-slim`

```console
$ docker pull clojure@sha256:adf88e057fac8f98890d92d20918c6ead16ec6ee0b08b9c03c30531d184607d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-tools-deps-1.11.1.1200-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:7057d6f4de40560589503b0e77cd3da8ca819985a29c63173b917372cf23ce0d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.0 MB (294001790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c90ca38d78bd010769b2cbd871eb037b877a7f5f79f1004cf5b18f4e9fe4fecc`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 06 Dec 2022 01:58:15 GMT
COPY dir:fef581854733ec7202f8c807463b9e1952aeb6c7a002719c7e54987e50ea4dcb in /opt/java/openjdk 
# Tue, 06 Dec 2022 01:58:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 02:00:07 GMT
ENV CLOJURE_VERSION=1.11.1.1200
# Tue, 06 Dec 2022 02:00:07 GMT
WORKDIR /tmp
# Tue, 06 Dec 2022 02:00:25 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "694381cb78d44f143bdcc38657507f012ebac4009bc57cec67abef1675447878 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 06 Dec 2022 02:00:25 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 06 Dec 2022 02:00:25 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 06 Dec 2022 02:00:25 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 06 Dec 2022 02:00:26 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f07ccb399757ca2eb22ecfbed8b8e0fe753148c9c99205f4b73d03bcc43ef0d`  
		Last Modified: Tue, 06 Dec 2022 02:09:27 GMT  
		Size: 201.1 MB (201103429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bed576360463471088c3f4644b767efa6eb3ece30b41ef961fe287342640be`  
		Last Modified: Tue, 06 Dec 2022 02:10:29 GMT  
		Size: 61.5 MB (61484493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b09f235d89ce14c567f7c2792ad60734c47309e8138888fe76b863228df1baeb`  
		Last Modified: Tue, 06 Dec 2022 02:10:21 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a9021b93c9a67ad5aa69ca86ad3dad42de65e3f3f020a481311b1c584cd1981`  
		Last Modified: Tue, 06 Dec 2022 02:10:21 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-tools-deps-1.11.1.1200-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:b9775e419253dab12221b4149acff3a267b1bb2358167a43594062dac15d142a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.5 MB (291529161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47346761de42b5edfe70db915cd4a9c18619e9046dea68cfdb46a2e0e3bc2ab5`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 06 Dec 2022 02:25:30 GMT
COPY dir:4138443eebfda1a2a245638d5bb568645bd34d79b66d39a3be31b5ac6b823d6d in /opt/java/openjdk 
# Tue, 06 Dec 2022 02:25:35 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 02:27:09 GMT
ENV CLOJURE_VERSION=1.11.1.1200
# Tue, 06 Dec 2022 02:27:09 GMT
WORKDIR /tmp
# Tue, 06 Dec 2022 02:27:22 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "694381cb78d44f143bdcc38657507f012ebac4009bc57cec67abef1675447878 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 06 Dec 2022 02:27:22 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 06 Dec 2022 02:27:22 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 06 Dec 2022 02:27:22 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 06 Dec 2022 02:27:23 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41824f9c81730654da632df65bb8c2a4392976f97f4a938f885db8e2cb6804c2`  
		Last Modified: Tue, 06 Dec 2022 02:35:24 GMT  
		Size: 199.9 MB (199864417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7026b8f64c58c435a46d95e1df52f0fea1ac25e81e512e06cb76a9151f9c0ec1`  
		Last Modified: Tue, 06 Dec 2022 02:36:18 GMT  
		Size: 61.6 MB (61603408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70a46e9e6e330dbee6dd2d0498764b3306e29d057bde98cc9f03b3a133fcfa0`  
		Last Modified: Tue, 06 Dec 2022 02:36:11 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92deac62234750f35dc5d408b54f16e37d0d4a9007e500417db286a5e7882f3`  
		Last Modified: Tue, 06 Dec 2022 02:36:11 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
