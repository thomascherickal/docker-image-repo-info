## `clojure:temurin-17-tools-deps-1.11.1.1224-bullseye-slim`

```console
$ docker pull clojure@sha256:2302c52dfd2586e0428e061c4748b4ded806ea5b61b59f13961ae1bcc9dfe561
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-tools-deps-1.11.1.1224-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:586cb7746983faf0bda1d5dbc05e865b431d1153fd9f8ba6cda5193b1fee6ee3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.3 MB (285336185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ae8992159e539aa724efc40dbe3460b688a216d0b8bcc2b64d2273ee4842d7a`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:41:22 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Mar 2023 07:47:19 GMT
COPY dir:5cf52f938fe415b0022fbccb8cf978562c503c0b8313cc9dedf46c1c4edb35cf in /opt/java/openjdk 
# Wed, 01 Mar 2023 07:47:21 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 07:49:11 GMT
ENV CLOJURE_VERSION=1.11.1.1224
# Wed, 01 Mar 2023 07:49:11 GMT
WORKDIR /tmp
# Wed, 01 Mar 2023 07:49:28 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "3bbab4d253eda43e3122fd5705014a69c44944a6dee8ea4d7d567afe157eb4ef *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 01 Mar 2023 07:49:29 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 01 Mar 2023 07:49:29 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 01 Mar 2023 07:49:29 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 01 Mar 2023 07:49:29 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f039bcab9992b3a477fd101e656d4f5ad27c8c30323fd021475c390e3d41213e`  
		Last Modified: Wed, 01 Mar 2023 07:58:57 GMT  
		Size: 192.4 MB (192438214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9517723369746fa5876b8fee1d9a4aff0709f6f78c8cd0c802a16cf7538a05fc`  
		Last Modified: Wed, 01 Mar 2023 08:00:15 GMT  
		Size: 61.5 MB (61485552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca58a5a7e292660e4640e629e2edec0a1824ffbb40fd1fdfd8465d8dbc737646`  
		Last Modified: Wed, 01 Mar 2023 08:00:07 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9d94ab9494f6fc011cc48215091fd8a50d718e31f9515ecd43d038632012e3`  
		Last Modified: Wed, 01 Mar 2023 08:00:07 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-tools-deps-1.11.1.1224-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:6ad35420eb69693c29c603af482b8e6c7e1ef529e6f94ce8b6af83b2589fa139
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.9 MB (282924502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5605dfbce8b2508e5c887347abad60d1a724a549407ce13f37a4a89125eeb9f5`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:02:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 02 Mar 2023 07:07:04 GMT
COPY dir:47c117bbc947c5c1164b5a20eeec0ba16c306f5991a85f22c54db31ca24ce4a8 in /opt/java/openjdk 
# Thu, 02 Mar 2023 07:07:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 07:09:39 GMT
ENV CLOJURE_VERSION=1.11.1.1224
# Thu, 02 Mar 2023 07:09:39 GMT
WORKDIR /tmp
# Thu, 02 Mar 2023 07:09:52 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "3bbab4d253eda43e3122fd5705014a69c44944a6dee8ea4d7d567afe157eb4ef *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 02 Mar 2023 07:09:53 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 02 Mar 2023 07:09:53 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Thu, 02 Mar 2023 07:09:53 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 02 Mar 2023 07:09:53 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee2a535b626ac45b3b701a33ede28cb7ec44388615e651313d6818cbca5d626`  
		Last Modified: Thu, 02 Mar 2023 07:20:21 GMT  
		Size: 191.3 MB (191260449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62bdfb431a072433ecaec2643540d1deed8962e6cf0dd61983cd9189a86a860`  
		Last Modified: Thu, 02 Mar 2023 07:22:28 GMT  
		Size: 61.6 MB (61600220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bfab8a452064eb814eb470fcbdf20460834e0895ba9109262bd7a27845f62f6`  
		Last Modified: Thu, 02 Mar 2023 07:22:22 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3727c5b358f618dde06293783cb4233b593fa6a24657a7738deeaf450c9553c0`  
		Last Modified: Thu, 02 Mar 2023 07:22:22 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
