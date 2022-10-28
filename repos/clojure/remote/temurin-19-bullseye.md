## `clojure:temurin-19-bullseye`

```console
$ docker pull clojure@sha256:9aad786513668e10d38f68651de0b378ea8655de183270bb8f60d2420deba98e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:9a3fb8e056f6dce2fab23dea8f365f5c0fcac64fde340b9b2740bb257b465f6b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.2 MB (303191814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:028a5257eaf39c86c1fcb2ad4ce2b425c978ca1b78399b066535fbd5016c38f8`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:42 GMT
ADD file:26702ba2c3e94cb21cdb3c550cf01cf848823d160f3417b559116d4c718e5df0 in / 
# Tue, 25 Oct 2022 01:43:42 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:32:27 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 02:42:31 GMT
COPY dir:49a4548ab030e4d26793e92b4d74537cf530961ce7b4083b8d383585c96415d5 in /opt/java/openjdk 
# Tue, 25 Oct 2022 02:42:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Oct 2022 20:40:21 GMT
ENV CLOJURE_VERSION=1.11.1.1182
# Fri, 28 Oct 2022 20:40:21 GMT
WORKDIR /tmp
# Fri, 28 Oct 2022 20:40:38 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "0e80041419bb91e142e2e8683e4dad6faf79958b603bb63b2a93bdd62c2a4f14 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 28 Oct 2022 20:40:38 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 28 Oct 2022 20:40:38 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 28 Oct 2022 20:40:38 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 28 Oct 2022 20:40:39 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:17c9e6141fdb3387e5a1c07d4f9b6a05ac1498e96029fa3ea55470d4504f7770`  
		Last Modified: Tue, 25 Oct 2022 01:47:28 GMT  
		Size: 55.0 MB (55046332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b6cdd3c4f04a6a611badcb0210b13df1430faf9e1bcbb3d09c250db0335722`  
		Last Modified: Tue, 25 Oct 2022 02:54:15 GMT  
		Size: 200.8 MB (200843786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884af1d6a84e6fb21557765610c8ea3d7d8dddfd7d35a8dd3dbf70652e604332`  
		Last Modified: Fri, 28 Oct 2022 20:51:16 GMT  
		Size: 47.3 MB (47300676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdffedef40eb55f11aee264604c61e6c4a071099d30dd9af9457f059f2428906`  
		Last Modified: Fri, 28 Oct 2022 20:51:10 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3109348bd2a5b661dfb159a5d745642b9462397f1a4016bfdfa96cc2bfa1d955`  
		Last Modified: Fri, 28 Oct 2022 20:51:10 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:bbe91fa76cc80b952110b4c5de5b9c202c0e2904debb5bbf1c9bb8c9ef1465a8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300578937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02ef9cf6dbc2a6272eaeb3fda1f665fd0304885346b0e63ee1201447097a6222`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 25 Oct 2022 05:45:55 GMT
ADD file:b16745ece8ef84c028d7e9ac4bf026ac64f885d4170bfcc9d435f237144a1b99 in / 
# Tue, 25 Oct 2022 05:45:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 23:53:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Oct 2022 15:48:52 GMT
COPY dir:2fc3a52010e404362374a6fbc2449d1ef85a3bc7bb00efe969cabc1864797789 in /opt/java/openjdk 
# Wed, 26 Oct 2022 15:48:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Oct 2022 20:31:04 GMT
ENV CLOJURE_VERSION=1.11.1.1182
# Fri, 28 Oct 2022 20:31:04 GMT
WORKDIR /tmp
# Fri, 28 Oct 2022 20:31:16 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "0e80041419bb91e142e2e8683e4dad6faf79958b603bb63b2a93bdd62c2a4f14 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 28 Oct 2022 20:31:17 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 28 Oct 2022 20:31:17 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 28 Oct 2022 20:31:17 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 28 Oct 2022 20:31:17 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:8e1d92e7d04d2a9a9880cb45dc3c32c2805912cd86abed96d0ada3ff28748205`  
		Last Modified: Tue, 25 Oct 2022 05:48:40 GMT  
		Size: 53.7 MB (53701966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8997f9b1128d353add7d065052afcf1047aea6a037bed4d3396015998ab5e3ca`  
		Last Modified: Wed, 26 Oct 2022 16:05:23 GMT  
		Size: 199.6 MB (199582421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2de57316782b9ea3a36ba39384fc588876a70574356f1c0f2ffab09f4a0c09a`  
		Last Modified: Fri, 28 Oct 2022 20:39:36 GMT  
		Size: 47.3 MB (47293533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48bbe6b7df4d9a999674258b9271cfa064ae7aa957a41e226669111c899db8b4`  
		Last Modified: Fri, 28 Oct 2022 20:39:32 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19e556f4201c04b7aebc2c414d5bcb6d4a1c74959ab79c5e6584f4d8fac07958`  
		Last Modified: Fri, 28 Oct 2022 20:39:31 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
