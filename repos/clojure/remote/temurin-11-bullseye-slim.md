## `clojure:temurin-11-bullseye-slim`

```console
$ docker pull clojure@sha256:02e0bc6b345897a53d172e4900cd214fa7f5e825caae3aab3e1ef4fc9adcbdee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:878db3f8f08b7b4e14e7f0ddc2189dd82c2a9cf428269803dd400e2465f8e64d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.7 MB (237748224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42cb667356379c8fefd918b930469b6013a118de21cd72f48c00c5962ae2acd0`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:51:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 12:45:36 GMT
COPY dir:2526dfaf6aedccef54b8de2f87890e86c6d3fe8431985d8e74dcfc29195b01ed in /opt/java/openjdk 
# Fri, 13 Oct 2023 12:45:37 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 12:50:52 GMT
ENV CLOJURE_VERSION=1.11.1.1413
# Fri, 13 Oct 2023 12:50:53 GMT
WORKDIR /tmp
# Fri, 13 Oct 2023 12:51:09 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "ad9aa1e99c59a4f7eb66450914fbec543337d9fada60dd9d34eec7fe18ae4965 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 13 Oct 2023 12:51:10 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 13 Oct 2023 12:51:10 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119a53a4a8795e7699b47fa3480b38b8b13e889bb26254f2a28ca9e57185096c`  
		Last Modified: Fri, 13 Oct 2023 13:05:54 GMT  
		Size: 144.8 MB (144826181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a54e850a66b645a7af9343e6c735cf3f429ca08dab1ebee022a682beec108e3`  
		Last Modified: Fri, 13 Oct 2023 13:08:48 GMT  
		Size: 61.5 MB (61503563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c70d13f5bf2cd5ab8397086b63ec29b3fccd10bfc737fa7e1ff08135bfd327`  
		Last Modified: Fri, 13 Oct 2023 13:08:41 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:cc3aa6c646e53453e4a0f0db94dabed41f3ad2338257f1c5b2ac5eab026e8175
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.3 MB (233255403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feb46561f11bce4d1d45fbf333608dfd6a780b95462cf17715fd14bf8929c3c0`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:46:08 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 08:26:07 GMT
COPY dir:b4903e9e1c2782550c5bca9cb7b0f840b4fdb810848e07ca44af328ac9dd84f6 in /opt/java/openjdk 
# Fri, 13 Oct 2023 10:13:35 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 10:17:47 GMT
ENV CLOJURE_VERSION=1.11.1.1413
# Fri, 13 Oct 2023 10:17:47 GMT
WORKDIR /tmp
# Fri, 13 Oct 2023 10:18:01 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "ad9aa1e99c59a4f7eb66450914fbec543337d9fada60dd9d34eec7fe18ae4965 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 13 Oct 2023 10:18:01 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 13 Oct 2023 10:18:01 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe38f36b0480d7264c9d22fe6161aee59046ea148d7c5db5adf031ed382ecb6`  
		Last Modified: Fri, 13 Oct 2023 08:29:47 GMT  
		Size: 141.6 MB (141570598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09bc2ab1b851bbb9922be339be740d673a37507832ff142d8cf3f49eb34a2854`  
		Last Modified: Fri, 13 Oct 2023 10:33:03 GMT  
		Size: 61.6 MB (61620104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e839a7a392877feeebd41c3424d3195ba95bf719656e5b661e36bcf7fbdc9021`  
		Last Modified: Fri, 13 Oct 2023 10:32:56 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
