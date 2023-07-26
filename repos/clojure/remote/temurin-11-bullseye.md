## `clojure:temurin-11-bullseye`

```console
$ docker pull clojure@sha256:e01b3a12cfceafa0c0905bc5de65a57583b871f75d596f85939dcd7b47c85dc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:8cd53527c70110b6451d063a9e9cdcc76571500f5030ef5a4b6fc44b217b89fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.5 MB (325487798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af8bcdddcef6b5eb62f9f0c4b619f4173a21b25abe5d99c0ec6f312289cbc058`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:09 GMT
ADD file:b7c0be2bb90e88689b1c16da78dea0b85760b55b90ef2e5bc4a529c89e4fa25b in / 
# Tue, 04 Jul 2023 01:20:10 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:59:14 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 05 Jul 2023 11:18:57 GMT
COPY dir:3cd19417e6ca044e31be7ef3c49c7d24f962c0f648fd205b421373092856c87f in /opt/java/openjdk 
# Wed, 05 Jul 2023 11:18:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Jul 2023 11:22:29 GMT
ENV CLOJURE_VERSION=1.11.1.1347
# Wed, 05 Jul 2023 11:22:29 GMT
WORKDIR /tmp
# Wed, 05 Jul 2023 11:22:53 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "d9158bf3a1d92fbf8551656e47a86f42e93d10f1db9defa2124bfee206ce8c8f *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 05 Jul 2023 11:22:54 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 05 Jul 2023 11:22:54 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:34df401c391c7595044379e04e8ad4856a5a3974cdbf5a160f0a204d761e88aa`  
		Last Modified: Tue, 04 Jul 2023 01:25:21 GMT  
		Size: 55.1 MB (55055300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f32c79546e308866ce38369edf4614a73777193f0a490707182288427a0b9a`  
		Last Modified: Wed, 05 Jul 2023 11:32:34 GMT  
		Size: 198.5 MB (198549453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87849fd2df727a44b349a0ec9efbd5309753987073a75145c77c606e829c730b`  
		Last Modified: Wed, 05 Jul 2023 11:34:21 GMT  
		Size: 71.9 MB (71882429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:051cd579d16340382fbf8d08a47c1d551d22d2e523c0514631adf4de4a3d9915`  
		Last Modified: Wed, 05 Jul 2023 11:34:13 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:5f4d2162ff1813e3b8e62bcb5ddd8341c067da5142d122ef6841e89f1426c13f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.3 MB (267271097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d50dc13e44a59d1a8e4041871977d3d4f983f6638dc06ed78c150903a47c67d0`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:43 GMT
ADD file:e626446584d8094b7b58d72a717380ca64d3e9ab924fc625406fe26a83fe1d8b in / 
# Tue, 04 Jul 2023 01:57:43 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:43:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Jul 2023 01:07:04 GMT
COPY dir:e71da8247d58ed4b0dfbf219951c863c79ac94b7f45cb60320ea827dfa699275 in /opt/java/openjdk 
# Wed, 26 Jul 2023 01:07:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jul 2023 01:10:22 GMT
ENV CLOJURE_VERSION=1.11.1.1347
# Wed, 26 Jul 2023 01:10:22 GMT
WORKDIR /tmp
# Wed, 26 Jul 2023 01:10:38 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "d9158bf3a1d92fbf8551656e47a86f42e93d10f1db9defa2124bfee206ce8c8f *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 26 Jul 2023 01:10:39 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 26 Jul 2023 01:10:39 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:29279ac7c19f9c667f1c6b07bfba6fba20ca0d945b9fbc6edad6f75d13361fae`  
		Last Modified: Tue, 04 Jul 2023 02:01:38 GMT  
		Size: 53.7 MB (53703979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a099a46124988665742eae84cd51e5a2ec69ba12a5a0324bfdecb15c9fcca0ec`  
		Last Modified: Wed, 26 Jul 2023 01:13:29 GMT  
		Size: 141.6 MB (141565305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58edb4e407ccd51ad080d713bda95b42946822fc3c33b86606e7eb074291ae41`  
		Last Modified: Wed, 26 Jul 2023 01:15:08 GMT  
		Size: 72.0 MB (72001196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5dfe25f46e3bf9c1582e348731f7ab1aa6587d265699b3d9da4354dfdd82076`  
		Last Modified: Wed, 26 Jul 2023 01:15:01 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
