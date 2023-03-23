## `clojure:temurin-19-tools-deps-1.11.1.1257-bullseye`

```console
$ docker pull clojure@sha256:7d0a2226df216f6bf6ee6a1f0eae79946e987e06912c154d9461d68ec708bfdd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-tools-deps-1.11.1.1257-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:f9122d1a1c5ab8b7b56c8b0bdf3f42320e2f2ddaa012f3e57589aaac3727edfb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.0 MB (328037243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d31f62648bb1821879b8fd0a976b9b6749f282b31e116eb3f859261155bbdd21`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:15 GMT
ADD file:459d1e92eb8c24ff4758f974d289ca8a2abe04cf50b6fe2bd760aa4589478289 in / 
# Thu, 23 Mar 2023 01:30:15 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:16:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:25:19 GMT
COPY dir:94cb5af8175285c10c94286222d8a35302f3f8c290e00011a75c67156659d6ab in /opt/java/openjdk 
# Thu, 23 Mar 2023 06:25:21 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:27:12 GMT
ENV CLOJURE_VERSION=1.11.1.1257
# Thu, 23 Mar 2023 06:27:12 GMT
WORKDIR /tmp
# Thu, 23 Mar 2023 06:27:27 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "be032cf21dc67ecf072f7254a01c3587d97aa311198f53cd1a1777ddfb3e9244 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 23 Mar 2023 06:27:28 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 23 Mar 2023 06:27:28 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Thu, 23 Mar 2023 06:27:28 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 23 Mar 2023 06:27:28 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:3e440a7045683e27f8e2fa04000e0e078d8dfac0c971358ae0f8c65c13321c8e`  
		Last Modified: Thu, 23 Mar 2023 01:34:00 GMT  
		Size: 55.0 MB (55045608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db7c7fe7e43e56d1e5e7153ccd41c7b1bf9e8b831af647a69ed9da06d59f2d9b`  
		Last Modified: Thu, 23 Mar 2023 06:34:16 GMT  
		Size: 201.1 MB (201112948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6835ec6d3d1ed4343fb6456818a413fefbd35c253abd67756e7de842b6f294be`  
		Last Modified: Thu, 23 Mar 2023 06:35:14 GMT  
		Size: 71.9 MB (71877676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51bbec3c7573c9373d7f4db215ea7f94a9d0c68d802d45a044baae0ff0d32d12`  
		Last Modified: Thu, 23 Mar 2023 06:35:06 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ff23d2d9b49db1eae0bceb656cb1085fc3639076015344f5cfc9e17b9db36b`  
		Last Modified: Thu, 23 Mar 2023 06:35:07 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-tools-deps-1.11.1.1257-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:5e7705b6eae95f13c67b4d79bde1ec632541d68b6be1a934969392d60ffd4f3f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.5 MB (325547877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c97607978608c277dc4eeb7b4e1777b9a801df31633325f8163ae181d1800a7`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:02 GMT
ADD file:70d18f9eea4e4fbdb941e66490ccb7233e182fe7ded1185de91c7d55580dd13e in / 
# Thu, 23 Mar 2023 00:45:02 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:52:12 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:59:08 GMT
COPY dir:9a6a873ca11063f6f04e7f088397a1fce771e2b1aa8590b72eb07158cfac883f in /opt/java/openjdk 
# Thu, 23 Mar 2023 06:59:13 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 07:00:55 GMT
ENV CLOJURE_VERSION=1.11.1.1257
# Thu, 23 Mar 2023 07:00:55 GMT
WORKDIR /tmp
# Thu, 23 Mar 2023 07:01:08 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "be032cf21dc67ecf072f7254a01c3587d97aa311198f53cd1a1777ddfb3e9244 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 23 Mar 2023 07:01:08 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 23 Mar 2023 07:01:08 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Thu, 23 Mar 2023 07:01:09 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 23 Mar 2023 07:01:09 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:8022b074731d9ecee7f4fba79b993920973811dda168bbc08636f18523b90122`  
		Last Modified: Thu, 23 Mar 2023 00:47:46 GMT  
		Size: 53.7 MB (53703099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d0a6a3f6f4458fd84817e257a4ed1795d2fe3740eb80c763937a14d0cf186a`  
		Last Modified: Thu, 23 Mar 2023 07:07:20 GMT  
		Size: 199.9 MB (199855189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560083074b9227be967fba77f3af623e5b1770be24c79ee1fca80b299acda3ce`  
		Last Modified: Thu, 23 Mar 2023 07:08:15 GMT  
		Size: 72.0 MB (71988574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ecfc5f642a04cac85674b0071ddc75bf80dff07470897980aea50bc7add6817`  
		Last Modified: Thu, 23 Mar 2023 07:08:09 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c8cc479a7d630600eb58d52d475b0dc49a9bd5da510dba095cb50342c9b79e6`  
		Last Modified: Thu, 23 Mar 2023 07:08:09 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
