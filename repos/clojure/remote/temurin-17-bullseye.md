## `clojure:temurin-17-bullseye`

```console
$ docker pull clojure@sha256:8015672747edef087b6ea6b4a6d0706aa22848217987a6e858eda2651589aef9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:1283ed466f7a5b19e041483db189ee56097e170b12adea1cd86f671beb9f42cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.5 MB (294483164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7b5fde87c4e0a8355a21584dfa427696be3c1bd577d0114a1923a44567382be`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:42 GMT
ADD file:26702ba2c3e94cb21cdb3c550cf01cf848823d160f3417b559116d4c718e5df0 in / 
# Tue, 25 Oct 2022 01:43:42 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:32:27 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 02:39:23 GMT
COPY dir:09afbf947759009c57336c17f70cd71239c5d8b0170793151aec66483cdd0976 in /opt/java/openjdk 
# Tue, 25 Oct 2022 02:39:24 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 02:41:36 GMT
ENV CLOJURE_VERSION=1.11.1.1165
# Tue, 25 Oct 2022 02:41:36 GMT
WORKDIR /tmp
# Tue, 25 Oct 2022 02:41:52 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "72d662bdc99b79037f9e34996272384de35e01e0416d8eb79cc940ee0f0fc808 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 25 Oct 2022 02:41:53 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 25 Oct 2022 02:41:53 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 25 Oct 2022 02:41:53 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 25 Oct 2022 02:41:53 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:17c9e6141fdb3387e5a1c07d4f9b6a05ac1498e96029fa3ea55470d4504f7770`  
		Last Modified: Tue, 25 Oct 2022 01:47:28 GMT  
		Size: 55.0 MB (55046332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac76dde2c2f13d28db088f654035acb0c8244b4c9447b8e9b0cfdb280fee3c55`  
		Last Modified: Tue, 25 Oct 2022 02:52:04 GMT  
		Size: 192.1 MB (192137591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:004cc23120c27da37276b78d82a5479038e81a13a5cab0e1fbd8fc990e77d8e9`  
		Last Modified: Tue, 25 Oct 2022 02:53:17 GMT  
		Size: 47.3 MB (47298226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329e0eeb36dff9bc95bb0e54ab718b717457d9772cb4785cdf0406564a602d49`  
		Last Modified: Tue, 25 Oct 2022 02:53:12 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adb7ae45231a0bbc76456e64d94035e57d5e7925c5d2b04a7fdd7ab872a499f`  
		Last Modified: Tue, 25 Oct 2022 02:53:12 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:f1c33b85f71ed8e19b18187fbe24f3d83cd8b40de8d7e5934a03ffe93d78c2ec
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291900131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9dc49f142f1e75670123d13111434d2de4bebf57efa710ed35c8239a7479cf2`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 25 Oct 2022 05:45:55 GMT
ADD file:b16745ece8ef84c028d7e9ac4bf026ac64f885d4170bfcc9d435f237144a1b99 in / 
# Tue, 25 Oct 2022 05:45:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 23:53:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Oct 2022 15:44:50 GMT
COPY dir:580c509aa131da1d31de9db8eed968c1f0ef93ad270f258b0b43d9d7d72bba84 in /opt/java/openjdk 
# Wed, 26 Oct 2022 15:44:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 15:47:45 GMT
ENV CLOJURE_VERSION=1.11.1.1165
# Wed, 26 Oct 2022 15:47:45 GMT
WORKDIR /tmp
# Wed, 26 Oct 2022 15:47:57 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "72d662bdc99b79037f9e34996272384de35e01e0416d8eb79cc940ee0f0fc808 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 26 Oct 2022 15:47:57 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 26 Oct 2022 15:47:57 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 26 Oct 2022 15:47:57 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 26 Oct 2022 15:47:57 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:8e1d92e7d04d2a9a9880cb45dc3c32c2805912cd86abed96d0ada3ff28748205`  
		Last Modified: Tue, 25 Oct 2022 05:48:40 GMT  
		Size: 53.7 MB (53701966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28dae7f1170ef9a47cb310629f09131dfb5a10ce4efd89d8f7e2a1aad189bb61`  
		Last Modified: Wed, 26 Oct 2022 16:01:02 GMT  
		Size: 190.9 MB (190904077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dabc244504f823ee05b66062dc4c5798873da88dc3a4767bb072b4ae213ef0a5`  
		Last Modified: Wed, 26 Oct 2022 16:03:26 GMT  
		Size: 47.3 MB (47293069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0b6a0ad39ea72c2a1af7e3c8f11241dd1f256fae0e8e0bc1c47b27167d1b9a`  
		Last Modified: Wed, 26 Oct 2022 16:03:21 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51239cba327f32e6c338c1b5a3c037dd5d8fc45ab82dce58223e42ff2e0676eb`  
		Last Modified: Wed, 26 Oct 2022 16:03:21 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
