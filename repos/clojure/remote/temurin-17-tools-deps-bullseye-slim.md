## `clojure:temurin-17-tools-deps-bullseye-slim`

```console
$ docker pull clojure@sha256:fc6e8f236e9fd3c189ad7608873732bb6b534c86462178b5e0e1b3504a76d405
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-tools-deps-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:2f0c383a6f6becaccdfd65c5a39639df4991ab250c794f0458b8175bd4b7f183
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.3 MB (285340188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c776c2de1d5bcc88a3203c3c0a89e386f483b12902774923109dac5f48f5da5`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:17:46 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:23:11 GMT
COPY dir:d90c8d6564183f8aad11f93ecfb2f7e0eeff18588ff2b62d7ca3d8d30672bc2c in /opt/java/openjdk 
# Thu, 23 Mar 2023 06:23:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:24:51 GMT
ENV CLOJURE_VERSION=1.11.1.1257
# Thu, 23 Mar 2023 06:24:51 GMT
WORKDIR /tmp
# Thu, 23 Mar 2023 06:25:07 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "be032cf21dc67ecf072f7254a01c3587d97aa311198f53cd1a1777ddfb3e9244 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 23 Mar 2023 06:25:07 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 23 Mar 2023 06:25:07 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Thu, 23 Mar 2023 06:25:07 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 23 Mar 2023 06:25:07 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f5c96fe943f36d4d8aa8ab4df9c0bd26f8cd6280632e002706fc7d61a975aa`  
		Last Modified: Thu, 23 Mar 2023 06:32:52 GMT  
		Size: 192.4 MB (192438234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab68d4a1297e7d66e4ca67182374f290ab7693f9f034e3583ed51e9cbfdca4c`  
		Last Modified: Thu, 23 Mar 2023 06:33:48 GMT  
		Size: 61.5 MB (61489533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8062f0de12248ecca2353f09d24718c1df4edb2f720bc69994e49502bb4ba9`  
		Last Modified: Thu, 23 Mar 2023 06:33:41 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753b6d6e8b2a1cde96642b681e5ad19af33d80816f82a2b3f640ba226d21ae78`  
		Last Modified: Thu, 23 Mar 2023 06:33:40 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-tools-deps-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:f0ba8ce80f8575c5a178e6f27ebe7dd10acf55f52e1c985906f6b0cbf24c2fdf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.9 MB (282928878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4e74c88192d3bb34ae728a2540af1542413f347928058824fdac71322beb2c6`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:52:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:57:23 GMT
COPY dir:44544f5117ae50af040f98b1979efcc18f4c9f0c7257bfc4a37b80697337361a in /opt/java/openjdk 
# Thu, 23 Mar 2023 06:57:27 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:58:48 GMT
ENV CLOJURE_VERSION=1.11.1.1257
# Thu, 23 Mar 2023 06:58:48 GMT
WORKDIR /tmp
# Thu, 23 Mar 2023 06:59:01 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "be032cf21dc67ecf072f7254a01c3587d97aa311198f53cd1a1777ddfb3e9244 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 23 Mar 2023 06:59:01 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 23 Mar 2023 06:59:02 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Thu, 23 Mar 2023 06:59:02 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 23 Mar 2023 06:59:02 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce46c3fded23542cb5a993d929bb8b2dfc32a31d4c9928588d2da3bc91d84fec`  
		Last Modified: Thu, 23 Mar 2023 07:06:00 GMT  
		Size: 191.3 MB (191260416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42549767c773d6583f01aa7c12f3409d884fe05b1dfbebeea356715652156d0b`  
		Last Modified: Thu, 23 Mar 2023 07:06:55 GMT  
		Size: 61.6 MB (61604749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2422b9bce223758f46a00137145f0ad2e27a958c04f090ca062e6292f5ce5b7f`  
		Last Modified: Thu, 23 Mar 2023 07:06:50 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f345b897a08d1414daaf07cbb819b7214611be0af32f14128faf0cde289bbff`  
		Last Modified: Thu, 23 Mar 2023 07:06:50 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
