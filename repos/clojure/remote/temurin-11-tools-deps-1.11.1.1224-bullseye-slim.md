## `clojure:temurin-11-tools-deps-1.11.1.1224-bullseye-slim`

```console
$ docker pull clojure@sha256:868ad16f2ad71659c1b3b50e4e9ffa3089f20a642624da05956e324fc2976f12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-tools-deps-1.11.1.1224-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:33a1d8feba52995f15f0a3c8585ea64bd3d7421538b54ad3680963a5dfe2cf0c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.4 MB (291372960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76a9a6f457e44010ad2a0ffaa1ee4cadacbf025571efeed34ab6edf2672836cb`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:41:22 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Mar 2023 07:44:16 GMT
COPY dir:fdbc5e9dec2946fa124877176e92a68dd3fe3a70def5bb906a6040c4a1303a2d in /opt/java/openjdk 
# Wed, 01 Mar 2023 07:44:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 07:46:13 GMT
ENV CLOJURE_VERSION=1.11.1.1224
# Wed, 01 Mar 2023 07:46:13 GMT
WORKDIR /tmp
# Wed, 01 Mar 2023 07:46:30 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "3bbab4d253eda43e3122fd5705014a69c44944a6dee8ea4d7d567afe157eb4ef *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 01 Mar 2023 07:46:30 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 01 Mar 2023 07:46:30 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56844ef93a6b4ee76d993441c680d901208ad2f1618368d240a20da46ff08911`  
		Last Modified: Wed, 01 Mar 2023 07:57:07 GMT  
		Size: 198.5 MB (198475514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71fc029e127ca848226f7a83226586b3995105cb9bafa7b58900b96ce69c8070`  
		Last Modified: Wed, 01 Mar 2023 07:58:06 GMT  
		Size: 61.5 MB (61485426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380432334792909875045e6a54f1f0db49abff4ef893ffb377502c67afdf39b0`  
		Last Modified: Wed, 01 Mar 2023 07:57:58 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-tools-deps-1.11.1.1224-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:2a1fdc24f0937285beb63d63fdc6641dcc3704cea86acf65f934ea973c199bac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.9 MB (286903021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9302f1ec2115f42c12c7e6a5a25635e4351249def72f72f32ca4db04fe10aeaf`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:02:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 02 Mar 2023 07:02:38 GMT
COPY dir:10bda54a6f055ef6cbbc2c7efdd1ef99bb798b3ae26972613c5ee4e57e620aeb in /opt/java/openjdk 
# Thu, 02 Mar 2023 07:02:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 07:05:43 GMT
ENV CLOJURE_VERSION=1.11.1.1224
# Thu, 02 Mar 2023 07:05:43 GMT
WORKDIR /tmp
# Thu, 02 Mar 2023 07:05:56 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "3bbab4d253eda43e3122fd5705014a69c44944a6dee8ea4d7d567afe157eb4ef *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 02 Mar 2023 07:05:57 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 02 Mar 2023 07:05:57 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4594d0c25b8198dd3c5842d1aeb5b5630309d3dc5160dd9849d5f1ba6b3b6b55`  
		Last Modified: Thu, 02 Mar 2023 07:17:16 GMT  
		Size: 195.2 MB (195240256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc6a42194262874dc17ead385d4e6ec470672e55c5bb4f4fa78c96870bd8de6`  
		Last Modified: Thu, 02 Mar 2023 07:19:00 GMT  
		Size: 61.6 MB (61599333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4014483c201aee9689570719ffe712c79dec90e920d40ce7cfa1677930440c2`  
		Last Modified: Thu, 02 Mar 2023 07:18:54 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
