## `clojure:temurin-8-tools-deps-1.11.1.1257-bullseye`

```console
$ docker pull clojure@sha256:bc76f30507883b386dd4d6692da63f0e68ff8c61116023e8485c1c2fc8a78801
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-tools-deps-1.11.1.1257-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:4aae6c2c0924877c9b2d99c9b3ad4989cdf9328d3cb001b865169ac8a92d33d2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.6 MB (181559387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81af1412020eb56d408b3ef91616080e1f6b67cd36f2823e49aee2141be4e1e1`
-	Default Command: `["clj"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:15 GMT
ADD file:459d1e92eb8c24ff4758f974d289ca8a2abe04cf50b6fe2bd760aa4589478289 in / 
# Thu, 23 Mar 2023 01:30:15 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:16:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:17:00 GMT
COPY dir:bbb84183d7ea38d81d8401f01e29d08935ee4c8bf6f90c6527579a1554c3bde1 in /opt/java/openjdk 
# Thu, 23 Mar 2023 06:17:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:19:07 GMT
ENV CLOJURE_VERSION=1.11.1.1257
# Thu, 23 Mar 2023 06:19:07 GMT
WORKDIR /tmp
# Thu, 23 Mar 2023 06:19:26 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "be032cf21dc67ecf072f7254a01c3587d97aa311198f53cd1a1777ddfb3e9244 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 23 Mar 2023 06:19:27 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 23 Mar 2023 06:19:27 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:3e440a7045683e27f8e2fa04000e0e078d8dfac0c971358ae0f8c65c13321c8e`  
		Last Modified: Thu, 23 Mar 2023 01:34:00 GMT  
		Size: 55.0 MB (55045608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5629480cb1323c2f01db8609391416fe9380f0b3fc3c8da30bdfaf6c963d0c`  
		Last Modified: Thu, 23 Mar 2023 06:29:13 GMT  
		Size: 54.6 MB (54635545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5696079656bd41494af0e6f3ea3f265c8c2c02f11f50dabfff7748cb78b7851`  
		Last Modified: Thu, 23 Mar 2023 06:30:03 GMT  
		Size: 71.9 MB (71877617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64bbaf724ee7d82409859f3c962d98138417f85505103656df1ea2c9272c1de`  
		Last Modified: Thu, 23 Mar 2023 06:29:55 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-tools-deps-1.11.1.1257-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:eff9b8cf828efb13d0e4ac921d3f30ada5f93838d7f9e0cca5e4e628eb050495
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.4 MB (179419822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:933dfe7467fd85c14be377be3aa10dac630eafcd1a907af04a926dff41797774`
-	Default Command: `["clj"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:02 GMT
ADD file:70d18f9eea4e4fbdb941e66490ccb7233e182fe7ded1185de91c7d55580dd13e in / 
# Thu, 23 Mar 2023 00:45:02 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:52:12 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:52:13 GMT
COPY dir:b6d7e5613532d986930216de9e0fece0632e82564ce7a6a98baf63b4115f840d in /opt/java/openjdk 
# Thu, 23 Mar 2023 06:52:14 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:53:49 GMT
ENV CLOJURE_VERSION=1.11.1.1257
# Thu, 23 Mar 2023 06:53:49 GMT
WORKDIR /tmp
# Thu, 23 Mar 2023 06:54:04 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "be032cf21dc67ecf072f7254a01c3587d97aa311198f53cd1a1777ddfb3e9244 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 23 Mar 2023 06:54:05 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 23 Mar 2023 06:54:05 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:8022b074731d9ecee7f4fba79b993920973811dda168bbc08636f18523b90122`  
		Last Modified: Thu, 23 Mar 2023 00:47:46 GMT  
		Size: 53.7 MB (53703099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db05ddb8bb6879c9a35043060daf1e3be2ff6486c8fdb3f0f54e8240f31ac24`  
		Last Modified: Thu, 23 Mar 2023 07:02:31 GMT  
		Size: 53.7 MB (53727922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851b3269dc40a5843e25a1d36c9ec0714593b772ec3f98cd1523975be785c935`  
		Last Modified: Thu, 23 Mar 2023 07:03:21 GMT  
		Size: 72.0 MB (71988184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a44a8b5e2d1b088c554e56f278a72c349e38cc4163bd4178906c43d66786c2`  
		Last Modified: Thu, 23 Mar 2023 07:03:15 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
