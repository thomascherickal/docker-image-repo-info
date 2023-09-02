## `clojure:temurin-11-bullseye`

```console
$ docker pull clojure@sha256:7a1f8bf3f06a0f03b0b9825347fe28b8c34046ce4303557a1538e55f59b8f1a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:fd095c8534ee93dba361a3a8e3c6a9017508312c28e737fa234421b96b59c8d8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.8 MB (271761182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8920d27d746cf7a960766ac973e83b69d9f1c41f2f246c9cc10428fcc025d461`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:57 GMT
ADD file:20f89ff93bfbd6c9fb1a97058a1f3de4485a8974e8a83892072c511fbd2e4134 in / 
# Wed, 16 Aug 2023 00:59:58 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:06 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 31 Aug 2023 23:22:26 GMT
COPY dir:9c2351d5d5cdf669213a7cfcfa52bd6bd8e9fc36b0a8e93328276d7280e1bab3 in /opt/java/openjdk 
# Thu, 31 Aug 2023 23:22:27 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 31 Aug 2023 23:29:28 GMT
ENV CLOJURE_VERSION=1.11.1.1413
# Thu, 31 Aug 2023 23:29:29 GMT
WORKDIR /tmp
# Thu, 31 Aug 2023 23:29:47 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "ad9aa1e99c59a4f7eb66450914fbec543337d9fada60dd9d34eec7fe18ae4965 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 31 Aug 2023 23:29:48 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 31 Aug 2023 23:29:48 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:6a70103cc499a199e10e379794c60aa524d9598587cc2bdfe2995642c2da8df7`  
		Last Modified: Wed, 16 Aug 2023 01:04:50 GMT  
		Size: 55.1 MB (55056621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab352bd56ec5464a5d56238b020eb3ec17516ac2525535fdf339dacbad129b6`  
		Last Modified: Thu, 31 Aug 2023 23:41:03 GMT  
		Size: 144.8 MB (144826073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b22774749efd55fe031cbdfa0a386098a026fc4631de0726a41e6bca67e9d9`  
		Last Modified: Thu, 31 Aug 2023 23:43:00 GMT  
		Size: 71.9 MB (71877870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f089de89d382ef569a275846f9d8a0ce1563a42a78d4461b60071bdaee3ac906`  
		Last Modified: Thu, 31 Aug 2023 23:42:52 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:49df5b68b7e7b4c5010f94f32e07bfa0feda5142d75d369964148e400507d7ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.3 MB (267273833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d549e7bcb12eb2ce1362bc89f2029edb509b950ae6d4d060176e78e7d840517`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:03 GMT
ADD file:8973cddb2d84a543b71001635599951bea6485a3526ae4ff916443b584864c83 in / 
# Tue, 15 Aug 2023 23:40:04 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:14 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Sep 2023 01:43:53 GMT
COPY dir:68819d2d348aedadecb99120d7ca4a63dcc1e3aa0bb526ecbd9925396c38234c in /opt/java/openjdk 
# Sat, 02 Sep 2023 01:43:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Sep 2023 01:46:28 GMT
ENV CLOJURE_VERSION=1.11.1.1413
# Sat, 02 Sep 2023 01:46:28 GMT
WORKDIR /tmp
# Sat, 02 Sep 2023 01:46:47 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "ad9aa1e99c59a4f7eb66450914fbec543337d9fada60dd9d34eec7fe18ae4965 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Sat, 02 Sep 2023 01:46:47 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Sat, 02 Sep 2023 01:46:47 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:e837d9f05c625de5b814b851adbc03559ba02ea7078f57c81a01e18fc65bf42b`  
		Last Modified: Tue, 15 Aug 2023 23:43:37 GMT  
		Size: 53.7 MB (53704779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e4e3a8bbfd2bdf093ae59fc74ef766b5e27c2748069f457d192d1719121d34`  
		Last Modified: Sat, 02 Sep 2023 01:53:12 GMT  
		Size: 141.6 MB (141570380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be118cfdcade305e8a5111ac50f573481ddd614eb60ef654556fe58585c458c7`  
		Last Modified: Sat, 02 Sep 2023 01:54:31 GMT  
		Size: 72.0 MB (71998055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5e2365ff1d842171fbcdb71109bd19445d0ebf5bb4087a9464d5e70ab33a8f`  
		Last Modified: Sat, 02 Sep 2023 01:54:24 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
