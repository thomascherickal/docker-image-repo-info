## `clojure:temurin-8-tools-deps-1.11.1.1165-bullseye-slim`

```console
$ docker pull clojure@sha256:e4acbf2587f75bdc33cdbfe30c0bf67073ac2b5100469346bbe4a8e787fe03b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-tools-deps-1.11.1.1165-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:72d2061c611920a11111a6a8da66b7940a465677ec9f36d0c4018ad79c05ff1a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.4 MB (196388572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c86eb1ba05f77bb1c55de3d1f2a5982815d455483fc6ec59920dbd2178aadd6`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:29 GMT
ADD file:5bd53bff884e470b3c12425132975ab9c6f99002c62c43bca1ff5cde9d863b92 in / 
# Tue, 13 Sep 2022 00:56:29 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:18:42 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 30 Sep 2022 22:21:04 GMT
COPY dir:300027169ac55d8fb6f67a0995ca298d5de23ab51f3dc8e227f6e221abd3d2c3 in /opt/java/openjdk 
# Fri, 30 Sep 2022 22:21:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 30 Sep 2022 22:23:21 GMT
ENV CLOJURE_VERSION=1.11.1.1165
# Fri, 30 Sep 2022 22:23:21 GMT
WORKDIR /tmp
# Fri, 30 Sep 2022 22:23:40 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "72d662bdc99b79037f9e34996272384de35e01e0416d8eb79cc940ee0f0fc808 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 30 Sep 2022 22:23:41 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 30 Sep 2022 22:23:41 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:31b3f1ad4ce1f369084d0f959813c51df0ca17d9877d5ee88c2db6ff88341430`  
		Last Modified: Tue, 13 Sep 2022 01:00:29 GMT  
		Size: 31.4 MB (31404121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b515481e3f48f5ef5749ccfcd2a56e22989feda711462e731a223a16a060f4`  
		Last Modified: Fri, 30 Sep 2022 22:36:08 GMT  
		Size: 103.5 MB (103513866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951394e1657ad2994c6eeadf43bb1fd1c48194b7b433984b01f7b7ca25f36ba2`  
		Last Modified: Fri, 30 Sep 2022 22:37:08 GMT  
		Size: 61.5 MB (61469968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60101a0e51abda239cde495cb42a5bc0b3072464bccf9703d1fdff5f07a46bfc`  
		Last Modified: Fri, 30 Sep 2022 22:37:01 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-tools-deps-1.11.1.1165-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:a0b9379869dfeca878161ce7f376863b09990b30111ec15dc88e8bce8b61e886
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.3 MB (194265991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42382936ca4de04c99004fd7cc45a32f1a4f606ef41ce8e1300551e7f853e643`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:56 GMT
ADD file:e8f00260a993aacae732bef51e6074b6c064d50a8ce1f0c44d53fe9e3c868e43 in / 
# Tue, 13 Sep 2022 02:10:56 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:58:12 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 30 Sep 2022 22:41:01 GMT
COPY dir:7668b70c49687fddef57006c57f288afd02ec3ccd6cde9cbc5231ec8fb9225f1 in /opt/java/openjdk 
# Fri, 30 Sep 2022 22:41:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 30 Sep 2022 22:43:34 GMT
ENV CLOJURE_VERSION=1.11.1.1165
# Fri, 30 Sep 2022 22:43:35 GMT
WORKDIR /tmp
# Fri, 30 Sep 2022 22:43:53 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "72d662bdc99b79037f9e34996272384de35e01e0416d8eb79cc940ee0f0fc808 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 30 Sep 2022 22:43:54 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 30 Sep 2022 22:43:54 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:3d898485473e3507374cea2e09f019c2ff5728f0911aa36c70b7a7235e9bc8ac`  
		Last Modified: Tue, 13 Sep 2022 02:16:19 GMT  
		Size: 30.1 MB (30054239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27700e5297add52eea6aaec46514b5c3aefc9690eb29f23c966f5b6c9a371425`  
		Last Modified: Fri, 30 Sep 2022 23:00:51 GMT  
		Size: 102.6 MB (102613748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc796aca97dd82885f029fdbbaa20169500c156980d22d7af42e2be4aa1c571`  
		Last Modified: Fri, 30 Sep 2022 23:01:59 GMT  
		Size: 61.6 MB (61597385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b0038543ae5d78707be4bc8d359b3f2305fb4fe3402485a6a6fdbd1336bfe97`  
		Last Modified: Fri, 30 Sep 2022 23:01:51 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
