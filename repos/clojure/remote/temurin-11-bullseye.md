## `clojure:temurin-11-bullseye`

```console
$ docker pull clojure@sha256:54e2a8dbc2df32215e6a9e47159850fd751d9020d776317d5a4430e518b2d19b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:217f76f4772f6ce1986eef4707c899c849665ee509549d71e0500ac66ba30fc0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.8 MB (271786229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fae2eb16b52778ed9341aa79af2d12c5fc3f9b6b9afaa2acf4cfb90414ccc1e6`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:01 GMT
ADD file:8a9222387b89a9ac763fd72610ce01ab17f64387cbfde30a6af1861a82030aad in / 
# Wed, 11 Oct 2023 18:35:01 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:51:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 12:45:01 GMT
COPY dir:2526dfaf6aedccef54b8de2f87890e86c6d3fe8431985d8e74dcfc29195b01ed in /opt/java/openjdk 
# Fri, 13 Oct 2023 12:45:02 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 12:50:28 GMT
ENV CLOJURE_VERSION=1.11.1.1413
# Fri, 13 Oct 2023 12:50:28 GMT
WORKDIR /tmp
# Fri, 13 Oct 2023 12:50:49 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "ad9aa1e99c59a4f7eb66450914fbec543337d9fada60dd9d34eec7fe18ae4965 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 13 Oct 2023 12:50:50 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 13 Oct 2023 12:50:50 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:69b3efbf67c2d9a46fdfdc8480b5a03ef73e9999a53aad57213447784f01eb6e`  
		Last Modified: Wed, 11 Oct 2023 18:39:54 GMT  
		Size: 55.1 MB (55058028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb795fe3c9891f009fd979aba8b303ac17d8263f44bbed3ded94759592267537`  
		Last Modified: Fri, 13 Oct 2023 13:05:34 GMT  
		Size: 144.8 MB (144826232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89aebd43f3adfa3657cc0a202ef5d641d1c3be860db567e1c814349df22db704`  
		Last Modified: Fri, 13 Oct 2023 13:08:30 GMT  
		Size: 71.9 MB (71901352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641691d31069f157f080263f37ee52980abbf19138ec81e69124283cf2fe66e4`  
		Last Modified: Fri, 13 Oct 2023 13:08:22 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:a3cd11a31cd5ee90dafda1d94adddfc7df24722a918735c4bb9b8d7e788c968f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.3 MB (267296144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cebc12a0ba60158281ddcdbee0e9fdf6b450fad714f69f3c421bb12e48b02a4`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:58 GMT
ADD file:e1a6c6c976e5e7c53eb2a7343a7a763b46e56828588535f4c79e63d6ec08198d in / 
# Wed, 11 Oct 2023 18:24:58 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:45:20 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 10:13:03 GMT
COPY dir:b4903e9e1c2782550c5bca9cb7b0f840b4fdb810848e07ca44af328ac9dd84f6 in /opt/java/openjdk 
# Fri, 13 Oct 2023 10:13:06 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 10:17:27 GMT
ENV CLOJURE_VERSION=1.11.1.1413
# Fri, 13 Oct 2023 10:17:27 GMT
WORKDIR /tmp
# Fri, 13 Oct 2023 10:17:44 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "ad9aa1e99c59a4f7eb66450914fbec543337d9fada60dd9d34eec7fe18ae4965 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 13 Oct 2023 10:17:45 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 13 Oct 2023 10:17:45 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:dd0dc10f921f4b3b65b17f20d367374079e6cb4e26531624ee64caaaf4adcc28`  
		Last Modified: Wed, 11 Oct 2023 18:28:45 GMT  
		Size: 53.7 MB (53707810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84f7633d1d2771c9ab00f2a01ba865738fa3a78d5441c5b21022c97aeaa5ebe`  
		Last Modified: Fri, 13 Oct 2023 10:30:01 GMT  
		Size: 141.6 MB (141570530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad97ff17b0ae2bcdd02d2bd7b4f577ecda27af1de3d06afa2f8a99b2afc96702`  
		Last Modified: Fri, 13 Oct 2023 10:32:44 GMT  
		Size: 72.0 MB (72017187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cae44abc70b98b1f6437239858d8fe4fa19027922d07080f5b518bb807f3d5f`  
		Last Modified: Fri, 13 Oct 2023 10:32:38 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
