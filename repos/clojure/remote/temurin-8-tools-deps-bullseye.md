## `clojure:temurin-8-tools-deps-bullseye`

```console
$ docker pull clojure@sha256:bf40d386d0453babc79e93d88ff9c597d2f189a9c65f6d79dab451463bc6aac6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-tools-deps-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:3f3b108f316d2dee8bed04acc5aa3bfc565e417d19913b86b432b7123d0171f4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.9 MB (205861557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5007913419f292973c963ece4419214583ff89da2257d81ff380f5b4d821cce7`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:42 GMT
ADD file:26702ba2c3e94cb21cdb3c550cf01cf848823d160f3417b559116d4c718e5df0 in / 
# Tue, 25 Oct 2022 01:43:42 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:32:27 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 02:32:30 GMT
COPY dir:300027169ac55d8fb6f67a0995ca298d5de23ab51f3dc8e227f6e221abd3d2c3 in /opt/java/openjdk 
# Tue, 25 Oct 2022 02:32:31 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Oct 2022 20:33:53 GMT
ENV CLOJURE_VERSION=1.11.1.1182
# Fri, 28 Oct 2022 20:33:53 GMT
WORKDIR /tmp
# Fri, 28 Oct 2022 20:34:14 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "0e80041419bb91e142e2e8683e4dad6faf79958b603bb63b2a93bdd62c2a4f14 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 28 Oct 2022 20:34:15 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 28 Oct 2022 20:34:15 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:17c9e6141fdb3387e5a1c07d4f9b6a05ac1498e96029fa3ea55470d4504f7770`  
		Last Modified: Tue, 25 Oct 2022 01:47:28 GMT  
		Size: 55.0 MB (55046332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479a9f308d68e7fc10c050f0178ed5da63c43501be70a5e1990e6f5737383502`  
		Last Modified: Tue, 25 Oct 2022 02:48:07 GMT  
		Size: 103.5 MB (103513858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177f8451d04a562b50f29f0d837441681720241f62e46e43cbf983a5c5483104`  
		Last Modified: Fri, 28 Oct 2022 20:45:17 GMT  
		Size: 47.3 MB (47300748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38841b6b2eb76e80ed2e8d675a04e0c72087e6a997231914b9eeee50f6a00f80`  
		Last Modified: Fri, 28 Oct 2022 20:45:11 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-tools-deps-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:0f1c587ac9b04fbf024117ad3fc7355d8ac9277772b0017d4ab81bf04815aafd
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.6 MB (203609943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:873359fa0770d3e5857e5479e9855dc87aa74e111ddf0f5ddc613a78568e9db7`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 25 Oct 2022 05:45:55 GMT
ADD file:b16745ece8ef84c028d7e9ac4bf026ac64f885d4170bfcc9d435f237144a1b99 in / 
# Tue, 25 Oct 2022 05:45:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 23:53:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 23:53:18 GMT
COPY dir:7668b70c49687fddef57006c57f288afd02ec3ccd6cde9cbc5231ec8fb9225f1 in /opt/java/openjdk 
# Tue, 25 Oct 2022 23:53:20 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Oct 2022 20:26:17 GMT
ENV CLOJURE_VERSION=1.11.1.1182
# Fri, 28 Oct 2022 20:26:17 GMT
WORKDIR /tmp
# Fri, 28 Oct 2022 20:26:34 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "0e80041419bb91e142e2e8683e4dad6faf79958b603bb63b2a93bdd62c2a4f14 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 28 Oct 2022 20:26:34 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 28 Oct 2022 20:26:34 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:8e1d92e7d04d2a9a9880cb45dc3c32c2805912cd86abed96d0ada3ff28748205`  
		Last Modified: Tue, 25 Oct 2022 05:48:40 GMT  
		Size: 53.7 MB (53701966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49c6d9cfee667003a4370293363d578b2b73027ffe0326780e6686aebf34652`  
		Last Modified: Wed, 26 Oct 2022 00:13:32 GMT  
		Size: 102.6 MB (102613479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2868c510c2013f3704d5f6eb8f67f16e1c06439bbdab11004c4fa213069c4f`  
		Last Modified: Fri, 28 Oct 2022 20:34:53 GMT  
		Size: 47.3 MB (47293879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8e4bece48497600730c9982d0af35be261dad7850c8646fe6fb038f150fe2f`  
		Last Modified: Fri, 28 Oct 2022 20:34:48 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
