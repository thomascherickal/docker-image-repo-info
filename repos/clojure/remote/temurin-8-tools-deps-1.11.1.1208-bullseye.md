## `clojure:temurin-8-tools-deps-1.11.1.1208-bullseye`

```console
$ docker pull clojure@sha256:0fc5618960a1cc4f45bc97c8d04a9473d7d45627b97541b82b151add6e66adde
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-tools-deps-1.11.1.1208-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:182bb1f722e6643011013686931a78aee976cec60062b12fd6f6f1f151c16451
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.9 MB (205866359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9e5862f9479f51c10803ec42774f1e751419aa8d1a5068bd4a3d7b86f7d0b53`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:21 GMT
ADD file:c13b430c8699df107ffd9ea5230b92238bc037a8e1cbbe35d6ab664941d575da in / 
# Wed, 21 Dec 2022 01:20:22 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:50:07 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 21 Dec 2022 01:50:10 GMT
COPY dir:53540f2d79f4eef9b2bf8c4b39ecdbbd82fb14bfcf951e14853afffd2efa2ecb in /opt/java/openjdk 
# Wed, 21 Dec 2022 01:50:11 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Dec 2022 01:52:38 GMT
ENV CLOJURE_VERSION=1.11.1.1200
# Wed, 21 Dec 2022 01:52:38 GMT
WORKDIR /tmp
# Wed, 21 Dec 2022 01:52:54 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "694381cb78d44f143bdcc38657507f012ebac4009bc57cec67abef1675447878 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 21 Dec 2022 01:52:55 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 21 Dec 2022 01:52:55 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:32de3c850997ce03b6ff4ae8fb00b34b9d7d7f9a35bfcdb8538e22cc7b77c29d`  
		Last Modified: Wed, 21 Dec 2022 01:24:10 GMT  
		Size: 55.0 MB (55025166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81441fc84c30ecd83d6155d0413d2d8a8941b7d8adaa0d20178da27d0be26b86`  
		Last Modified: Wed, 21 Dec 2022 02:05:09 GMT  
		Size: 103.5 MB (103530611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4bf8109381088cd767bf9282589984618a5eb78fac511a3494c75fd7d7938f`  
		Last Modified: Wed, 21 Dec 2022 02:06:06 GMT  
		Size: 47.3 MB (47309965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91e3d3021401e2808244a1c4062ac34f8c09d2fb6f60e559dffecfbcae2998d`  
		Last Modified: Wed, 21 Dec 2022 02:06:01 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-tools-deps-1.11.1.1208-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:3ce60001ffa7b6f251078deecc920bda43f6276ade93ca827270cff01ac776a6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.6 MB (203611920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cf116460c721a40c398459d2280a9e4597125abd283a713cb14945afbbe814b`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:40 GMT
ADD file:5bbdc914ec8ed60ac85293e88ee1aafc3f0290762e320fc86dc9d79fa201834e in / 
# Wed, 21 Dec 2022 01:39:41 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:18:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 21 Dec 2022 02:18:06 GMT
COPY dir:8a3fd802e7e57a45d80b19a89e91b421563b952585d39995819354f278317671 in /opt/java/openjdk 
# Wed, 21 Dec 2022 02:18:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Dec 2022 02:19:59 GMT
ENV CLOJURE_VERSION=1.11.1.1200
# Wed, 21 Dec 2022 02:19:59 GMT
WORKDIR /tmp
# Wed, 21 Dec 2022 02:20:13 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "694381cb78d44f143bdcc38657507f012ebac4009bc57cec67abef1675447878 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 21 Dec 2022 02:20:13 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 21 Dec 2022 02:20:13 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:c3e6129b48b69d14c5e7a5605e2b94003fb71aac82eac46b8689f5b8007af2c5`  
		Last Modified: Wed, 21 Dec 2022 01:42:49 GMT  
		Size: 53.7 MB (53681797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6100ae9251c3fa47a7e33ea8291f08f02fc3029cfa40a52f572ccce640a5978`  
		Last Modified: Wed, 21 Dec 2022 02:30:41 GMT  
		Size: 102.6 MB (102626555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ceb75d666381a02ce360df108ad1ebe44634dc4517c62a281bbd8d556092acb`  
		Last Modified: Wed, 21 Dec 2022 02:31:35 GMT  
		Size: 47.3 MB (47302950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607e9409a09406cac01430925d39dda540c9095b33fb83bb13f47efe3362076f`  
		Last Modified: Wed, 21 Dec 2022 02:31:29 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
