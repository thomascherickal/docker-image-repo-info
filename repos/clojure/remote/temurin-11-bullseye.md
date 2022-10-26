## `clojure:temurin-11-bullseye`

```console
$ docker pull clojure@sha256:6b25d0517dd0fdd3a0d351056e22dd54a4ea09cf39533a52dba11e79a97f62cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:d7dace4a762cb6340241e5e7767f2168d843b62e3cf696195fd8285bca84c00d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.5 MB (300469873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c75c4923e2f21b975a0098ac0b5b1593775500f649a3efbef13c524a759cf3a4`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:42 GMT
ADD file:26702ba2c3e94cb21cdb3c550cf01cf848823d160f3417b559116d4c718e5df0 in / 
# Tue, 25 Oct 2022 01:43:42 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:32:27 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 02:36:10 GMT
COPY dir:e3c63d67b32fccda756dd62000a0cf47da966d18fe6f1f25cd1f37b60881f0ec in /opt/java/openjdk 
# Tue, 25 Oct 2022 02:36:11 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 02:38:29 GMT
ENV CLOJURE_VERSION=1.11.1.1165
# Tue, 25 Oct 2022 02:38:29 GMT
WORKDIR /tmp
# Tue, 25 Oct 2022 02:38:44 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "72d662bdc99b79037f9e34996272384de35e01e0416d8eb79cc940ee0f0fc808 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 25 Oct 2022 02:38:45 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 25 Oct 2022 02:38:45 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:17c9e6141fdb3387e5a1c07d4f9b6a05ac1498e96029fa3ea55470d4504f7770`  
		Last Modified: Tue, 25 Oct 2022 01:47:28 GMT  
		Size: 55.0 MB (55046332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e425413bc0ae0b1045fcbc0ad4409b98eeded13a40018b63e55084142fd5a78e`  
		Last Modified: Tue, 25 Oct 2022 02:50:03 GMT  
		Size: 198.1 MB (198124992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2bdb6bb8eed353cd9bdad88865e0094a6a6f2c01c5436ba627e8f6d6d7c0bd`  
		Last Modified: Tue, 25 Oct 2022 02:51:13 GMT  
		Size: 47.3 MB (47297932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a731b92f5283b0fe6b2c485abe3271d411fc87058314bbb5e0645de4753e16`  
		Last Modified: Tue, 25 Oct 2022 02:51:08 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:7b47404cfe4967502ab88ec777f83fac95bea59bccbe5c95eed0aebbebc8255a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.9 MB (295862594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe8a4f97ff800d6a7ed09c6cf31f7a84db274995f57a4cf8b6004a48f207e29f`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 25 Oct 2022 05:45:55 GMT
ADD file:b16745ece8ef84c028d7e9ac4bf026ac64f885d4170bfcc9d435f237144a1b99 in / 
# Tue, 25 Oct 2022 05:45:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 23:53:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Oct 2022 15:37:43 GMT
COPY dir:0c9c8c2b9cd43799d246d5824c591352650ad79f5d15544287f00c2deb1e4608 in /opt/java/openjdk 
# Wed, 26 Oct 2022 15:37:48 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 15:42:58 GMT
ENV CLOJURE_VERSION=1.11.1.1165
# Wed, 26 Oct 2022 15:42:58 GMT
WORKDIR /tmp
# Wed, 26 Oct 2022 15:43:30 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "72d662bdc99b79037f9e34996272384de35e01e0416d8eb79cc940ee0f0fc808 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 26 Oct 2022 15:43:30 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 26 Oct 2022 15:43:30 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:8e1d92e7d04d2a9a9880cb45dc3c32c2805912cd86abed96d0ada3ff28748205`  
		Last Modified: Tue, 25 Oct 2022 05:48:40 GMT  
		Size: 53.7 MB (53701966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c7a7b51e23fc2e53d8018b07b36bae7b1c261267f2981e18b50be0d7b845881`  
		Last Modified: Wed, 26 Oct 2022 15:57:42 GMT  
		Size: 194.9 MB (194866970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624bbf40b0a3115da86bd822046649555c1947f2eed68aa2821f2ca18d305c77`  
		Last Modified: Wed, 26 Oct 2022 15:59:37 GMT  
		Size: 47.3 MB (47293041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adfe51daf9cf02bcca2737a4a9b3412309cc4fc46f4a180f4ac673a5897a9d5`  
		Last Modified: Wed, 26 Oct 2022 15:59:32 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
