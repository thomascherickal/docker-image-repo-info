## `clojure:temurin-17-bullseye`

```console
$ docker pull clojure@sha256:6130f5b6c52d45071db348680eb09e9370e6393647b8c9222532c384bd3be567
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:2b5ce2c7816ce51103e6e211bece3912e60de73b1c696e64df9eec4d612cd2b1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.5 MB (294485877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f910fa157dca8866895990b90764aec67a9b31f51002d04e90bb22de9c700751`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:42 GMT
ADD file:26702ba2c3e94cb21cdb3c550cf01cf848823d160f3417b559116d4c718e5df0 in / 
# Tue, 25 Oct 2022 01:43:42 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:32:27 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Oct 2022 21:54:43 GMT
COPY dir:b50a87fd6710a805ef25d6c1dd2c5f7aa37ef63d04ab1c00c91801848dae94f0 in /opt/java/openjdk 
# Wed, 26 Oct 2022 21:54:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Oct 2022 20:38:16 GMT
ENV CLOJURE_VERSION=1.11.1.1182
# Fri, 28 Oct 2022 20:38:16 GMT
WORKDIR /tmp
# Fri, 28 Oct 2022 20:38:33 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "0e80041419bb91e142e2e8683e4dad6faf79958b603bb63b2a93bdd62c2a4f14 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 28 Oct 2022 20:38:34 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 28 Oct 2022 20:38:34 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 28 Oct 2022 20:38:34 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 28 Oct 2022 20:38:34 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:17c9e6141fdb3387e5a1c07d4f9b6a05ac1498e96029fa3ea55470d4504f7770`  
		Last Modified: Tue, 25 Oct 2022 01:47:28 GMT  
		Size: 55.0 MB (55046332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c779c71ed965efeafbd0884b3b2abdcb54913a73b69c6be2a18253fd1af00a5`  
		Last Modified: Wed, 26 Oct 2022 22:10:37 GMT  
		Size: 192.1 MB (192137566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04dca9db30484c7636e1fb6cb300a2dfeffca32c3b97c45fa7960db73b4c7c4c`  
		Last Modified: Fri, 28 Oct 2022 20:49:10 GMT  
		Size: 47.3 MB (47300958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55484d41e3b7c7aa8918e9b80bb241f72fd984824b4f3ed6d3a64f4cd9b967d0`  
		Last Modified: Fri, 28 Oct 2022 20:49:04 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff90db43a29b7dee843acb004259c99513957f6eca3ec390f3bc75ef9d4a41a7`  
		Last Modified: Fri, 28 Oct 2022 20:49:04 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:3da0e9d1f30f294ddc7c0eb70d6bf69222c7842a2f2ee794fa84093218ee558a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291900910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ba34bb18fdcd296b5ed2e2ea78cb68f9435d17750eed13af13b4b718fb31305`
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
# Fri, 28 Oct 2022 20:29:38 GMT
ENV CLOJURE_VERSION=1.11.1.1182
# Fri, 28 Oct 2022 20:29:38 GMT
WORKDIR /tmp
# Fri, 28 Oct 2022 20:29:50 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "0e80041419bb91e142e2e8683e4dad6faf79958b603bb63b2a93bdd62c2a4f14 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 28 Oct 2022 20:29:50 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 28 Oct 2022 20:29:50 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 28 Oct 2022 20:29:50 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 28 Oct 2022 20:29:50 GMT
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
	-	`sha256:34a5744e2743b7302a96d9ca3c8520feb1c6c1292bbc732f5b0e322bcdb0b8da`  
		Last Modified: Fri, 28 Oct 2022 20:37:50 GMT  
		Size: 47.3 MB (47293849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468f670c4187b083b1e4dbee7b8ab76390105496932c7e939765319c113585a7`  
		Last Modified: Fri, 28 Oct 2022 20:37:45 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce36e55ce5bb9fd5e5b1806797ec009c95231368aa2219e53244c764c61e5ab4`  
		Last Modified: Fri, 28 Oct 2022 20:37:45 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
