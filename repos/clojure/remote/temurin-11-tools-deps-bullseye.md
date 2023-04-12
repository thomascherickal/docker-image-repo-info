## `clojure:temurin-11-tools-deps-bullseye`

```console
$ docker pull clojure@sha256:ddc69096202e5fa604546daf0e9548a3fa7034edf950da90af87b9e3e934e07b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-tools-deps-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:d797fa77cb538bf410ad19f901bdde3554c89ce62a0ffa6b1cc7ef9d825cf8eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.4 MB (325409202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bfbc19c29d03ea8d8c49d52875171b2c45ad35b7d5ea9026cbed4b5df3fe3d9`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:10:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:13:28 GMT
COPY dir:e649a995635d4b28f1458e8ccc09f5f71440b52479cfda5ea11e99ab14d0ce82 in /opt/java/openjdk 
# Wed, 12 Apr 2023 08:13:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 08:15:25 GMT
ENV CLOJURE_VERSION=1.11.1.1267
# Wed, 12 Apr 2023 08:15:25 GMT
WORKDIR /tmp
# Wed, 12 Apr 2023 08:15:42 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "c949c9ba24ee46a2c57c6e6aeff262ebb0ff8112ee2367b3dbabd2f2df75380a *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 12 Apr 2023 08:15:42 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 12 Apr 2023 08:15:42 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc28d33e44b328c3a33e1c0717d82dcbea604364ba89e1ab1b64f3d3a2f165a`  
		Last Modified: Wed, 12 Apr 2023 08:22:57 GMT  
		Size: 198.5 MB (198476040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206cb3aa0b9926fe1736c654997d240535b33778d3a3bc42660af94300437f6f`  
		Last Modified: Wed, 12 Apr 2023 08:23:54 GMT  
		Size: 71.9 MB (71879809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e39b0700fe46e094eceab5979a5e6088137791e7e4d327ce09dd184471b215`  
		Last Modified: Wed, 12 Apr 2023 08:23:47 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-tools-deps-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:c1e311f8b20b173e714dcf40e84de20062936752957ee0ef5d106000cdbbe3eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.9 MB (320945272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:665292dae647ab1229186bed8d7758cfa696eee47a1c80c721e8bdd27cf68fd5`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:20:38 GMT
COPY dir:d446509417048b798354227404c222c2c6031477a91cb1b64eded33f5e598adf in /opt/java/openjdk 
# Wed, 12 Apr 2023 01:20:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 01:22:28 GMT
ENV CLOJURE_VERSION=1.11.1.1267
# Wed, 12 Apr 2023 01:22:28 GMT
WORKDIR /tmp
# Wed, 12 Apr 2023 01:22:42 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "c949c9ba24ee46a2c57c6e6aeff262ebb0ff8112ee2367b3dbabd2f2df75380a *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 12 Apr 2023 01:22:43 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 12 Apr 2023 01:22:43 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e34d229c4186d9e7e7ce0aee26abda131ebcee8bee99be5af11bfc1bf391db`  
		Last Modified: Wed, 12 Apr 2023 01:29:24 GMT  
		Size: 195.2 MB (195242537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5585b1ca4a2f3ad56fc345ce4d5222726834dcf99d544c64a0e4c206ef7145`  
		Last Modified: Wed, 12 Apr 2023 01:30:20 GMT  
		Size: 72.0 MB (71996590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af892a80c1e67e491172870a61d2540c5b79ab559e2f18814dc44cc035bb6ea4`  
		Last Modified: Wed, 12 Apr 2023 01:30:13 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
