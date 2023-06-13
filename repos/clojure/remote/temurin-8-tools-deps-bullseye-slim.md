## `clojure:temurin-8-tools-deps-bullseye-slim`

```console
$ docker pull clojure@sha256:72bc5e267e9dd18c6611ff2ded3578339a0b621ada0ef97f3d28560c4cd36a79
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-tools-deps-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:c109b32aa02e6def7e80093fb32046185ae2f6471227dcef45c5e0c1136db1f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.6 MB (147556113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5202851ea9506ed986659766f08bc0209f941e42a63bb6e3d4d5537d91355976`
-	Default Command: `["clj"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:44:37 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 03:44:38 GMT
COPY dir:715eb4123a1bd94a1f232c902a6f3cdcc4011195a3e566c0f0ddc35dd1e83095 in /opt/java/openjdk 
# Tue, 13 Jun 2023 03:44:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 03:46:28 GMT
ENV CLOJURE_VERSION=1.11.1.1347
# Tue, 13 Jun 2023 03:46:28 GMT
WORKDIR /tmp
# Tue, 13 Jun 2023 03:46:44 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "d9158bf3a1d92fbf8551656e47a86f42e93d10f1db9defa2124bfee206ce8c8f *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 13 Jun 2023 03:46:45 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 13 Jun 2023 03:46:45 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a06b2482c1581bf48768b9037153a524f6626b4fdbab3333e123405ee98c4d`  
		Last Modified: Tue, 13 Jun 2023 03:55:36 GMT  
		Size: 54.6 MB (54642102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17fa89b015a707946fb4958baa983f8c80cc5d04cea4d6ac58afa6a38e9a2126`  
		Last Modified: Tue, 13 Jun 2023 03:56:31 GMT  
		Size: 61.5 MB (61495986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edefd48b8a407735e061d56a685a8a726fb642a2f3e8ac9cd72a03eff0355ce3`  
		Last Modified: Tue, 13 Jun 2023 03:56:24 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-tools-deps-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:81291b87673a035c20328844a6cb3a70c78b67a77d6276f28618e7c687b21369
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.4 MB (145417302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf13628c799edc352d9d09e59de0a0348dc50297ea85db8fc3b3cdc58214cbce`
-	Default Command: `["clj"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:28:47 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 04:51:12 GMT
COPY dir:f6bbe63c81e220d954915791686219263d8c45918fd81b238f7c9f6b21f076f8 in /opt/java/openjdk 
# Tue, 13 Jun 2023 04:51:13 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 04:52:49 GMT
ENV CLOJURE_VERSION=1.11.1.1347
# Tue, 13 Jun 2023 04:52:49 GMT
WORKDIR /tmp
# Tue, 13 Jun 2023 04:53:03 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "d9158bf3a1d92fbf8551656e47a86f42e93d10f1db9defa2124bfee206ce8c8f *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 13 Jun 2023 04:53:04 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 13 Jun 2023 04:53:04 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c42dbe9973fad0e5db82fff74ab48ee24033b2296cd2ca6fdcba69bad893d2`  
		Last Modified: Tue, 13 Jun 2023 05:00:32 GMT  
		Size: 53.7 MB (53742662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83123ae7dbdc6814d261f5910bda01787c980f6179a4aca95b5070b9b9aaba1d`  
		Last Modified: Tue, 13 Jun 2023 05:01:25 GMT  
		Size: 61.6 MB (61611193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9739d6480312a102f7e45f5fc05b678a8c5d32566a33f9ec06b9b5dd0b973240`  
		Last Modified: Tue, 13 Jun 2023 05:01:19 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
