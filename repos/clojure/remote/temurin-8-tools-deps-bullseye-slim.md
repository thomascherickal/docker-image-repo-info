## `clojure:temurin-8-tools-deps-bullseye-slim`

```console
$ docker pull clojure@sha256:79ba92d39d10845b7fc22987b9933fab98ab78247061d0f4bcb762dbe2b13d64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-tools-deps-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:a35c93baffb522d2fdb285f4449979c44d278993861845089802744a1b9171c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.5 MB (147537146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09a122e99bed08490ead5a13e7ee8ed3952f9367f165341358121a7a6d88c98e`
-	Default Command: `["clj"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:17:46 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:17:47 GMT
COPY dir:bbb84183d7ea38d81d8401f01e29d08935ee4c8bf6f90c6527579a1554c3bde1 in /opt/java/openjdk 
# Thu, 23 Mar 2023 06:17:48 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:19:31 GMT
ENV CLOJURE_VERSION=1.11.1.1257
# Thu, 23 Mar 2023 06:19:31 GMT
WORKDIR /tmp
# Thu, 23 Mar 2023 06:19:47 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "be032cf21dc67ecf072f7254a01c3587d97aa311198f53cd1a1777ddfb3e9244 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 23 Mar 2023 06:19:47 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 23 Mar 2023 06:19:47 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1977e261c2ece5904696fe62d44f44495568e580f96e10c2adb6f00ef7e609c9`  
		Last Modified: Thu, 23 Mar 2023 06:29:27 GMT  
		Size: 54.6 MB (54635545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956940efc3439ca83db0ef5e2ba9eb4618daacd3caf479b57133d579a1d05b46`  
		Last Modified: Thu, 23 Mar 2023 06:30:20 GMT  
		Size: 61.5 MB (61489579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47034acf9c93491b473d4106e19939e6dab679fa02f4f84c2c4be7a41308d433`  
		Last Modified: Thu, 23 Mar 2023 06:30:13 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-tools-deps-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:2d1307abbc1e7530c855e13471ee585c2d329a7fc992c22ba611f57770c29e3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.4 MB (145396168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3855740a350e801855bcf63d5a6e47bac89d22cb633983a823c84bf9e61620a0`
-	Default Command: `["clj"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:52:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:52:40 GMT
COPY dir:b6d7e5613532d986930216de9e0fece0632e82564ce7a6a98baf63b4115f840d in /opt/java/openjdk 
# Thu, 23 Mar 2023 06:52:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:54:08 GMT
ENV CLOJURE_VERSION=1.11.1.1257
# Thu, 23 Mar 2023 06:54:08 GMT
WORKDIR /tmp
# Thu, 23 Mar 2023 06:54:21 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "be032cf21dc67ecf072f7254a01c3587d97aa311198f53cd1a1777ddfb3e9244 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 23 Mar 2023 06:54:22 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 23 Mar 2023 06:54:22 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18f48d2f27de7b5e53c0560c7b25baf6904fad54afeb5ea0f8dc5d66dd42d6ee`  
		Last Modified: Thu, 23 Mar 2023 07:02:45 GMT  
		Size: 53.7 MB (53727901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33cf9a5342649c705333dbe7ab93e8f88d49a171dee411521e21024b21e04b44`  
		Last Modified: Thu, 23 Mar 2023 07:03:37 GMT  
		Size: 61.6 MB (61604950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a8dd4f64c2807984717f7e555a5ecc86229aa3dafe1ceb1f379cbd89696db4`  
		Last Modified: Thu, 23 Mar 2023 07:03:31 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
