## `clojure:temurin-11-tools-deps-1.11.1.1224-bullseye`

```console
$ docker pull clojure@sha256:89cb690fd391a7acbd7f99d1017723e77e2036c3b852248a114122cee83cb862
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-tools-deps-1.11.1.1224-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:33ab0d1f4065b3d3de35a49b9f973209eb1fd80d44ab4cd195da37ef02870766
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.4 MB (325400335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b3d8b4c878b5a72b8c107143be65131150eb0840a1d0de7af65fa138eb09167`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:40:41 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Mar 2023 07:43:44 GMT
COPY dir:fdbc5e9dec2946fa124877176e92a68dd3fe3a70def5bb906a6040c4a1303a2d in /opt/java/openjdk 
# Wed, 01 Mar 2023 07:43:46 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 07:45:49 GMT
ENV CLOJURE_VERSION=1.11.1.1224
# Wed, 01 Mar 2023 07:45:49 GMT
WORKDIR /tmp
# Wed, 01 Mar 2023 07:46:06 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "3bbab4d253eda43e3122fd5705014a69c44944a6dee8ea4d7d567afe157eb4ef *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 01 Mar 2023 07:46:07 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 01 Mar 2023 07:46:07 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c0b29cc6adaf6091151573ab5a4ba12f03dcfaea1402985879aea0d535da14c`  
		Last Modified: Wed, 01 Mar 2023 07:56:45 GMT  
		Size: 198.5 MB (198475588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9005ebac901a10e3a7c1749a401e7b9e8acdfa9de8fd330e81f930886009e1ff`  
		Last Modified: Wed, 01 Mar 2023 07:57:48 GMT  
		Size: 71.9 MB (71878210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be0954c0566d44b28867aa3851da1e702c8fd3f7d3107a66e247f70666aeb40`  
		Last Modified: Wed, 01 Mar 2023 07:57:40 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-tools-deps-1.11.1.1224-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:774163281879ef66e65bfb74712984377d52c64f483fc8de0f8f39e8bc316c45
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.9 MB (320934071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36a19d2feafd5e82583340f83dda4826dc854215636156cbcf3f3f038492f959`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:30 GMT
ADD file:a6a1df499d0d5b07fb366d776a11c42ddee6261e2425a921041b38e868192770 in / 
# Wed, 01 Mar 2023 02:20:30 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:01:14 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 02 Mar 2023 07:02:06 GMT
COPY dir:10bda54a6f055ef6cbbc2c7efdd1ef99bb798b3ae26972613c5ee4e57e620aeb in /opt/java/openjdk 
# Thu, 02 Mar 2023 07:02:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 07:05:19 GMT
ENV CLOJURE_VERSION=1.11.1.1224
# Thu, 02 Mar 2023 07:05:19 GMT
WORKDIR /tmp
# Thu, 02 Mar 2023 07:05:38 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "3bbab4d253eda43e3122fd5705014a69c44944a6dee8ea4d7d567afe157eb4ef *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 02 Mar 2023 07:05:39 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 02 Mar 2023 07:05:39 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:0f5fe16b1836feccd4765ac5685fc7a7b9c73445cac94fc595d2ffbc3cb59a7a`  
		Last Modified: Wed, 01 Mar 2023 02:23:53 GMT  
		Size: 53.7 MB (53703215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2257672252a1a5ea1cc84b22bcdf9e8c2de57f555374ecbd0173cf802564a507`  
		Last Modified: Thu, 02 Mar 2023 07:16:55 GMT  
		Size: 195.2 MB (195240142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee87b448a31f592866cd53c73d0d7f28be4b604955dabf6089fd317adcecef3`  
		Last Modified: Thu, 02 Mar 2023 07:18:43 GMT  
		Size: 72.0 MB (71990095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de725bc6c7a1c5f9a9df4f95b0136c5645146051222cc68ef2bbb7d8772e7a1`  
		Last Modified: Thu, 02 Mar 2023 07:18:37 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
