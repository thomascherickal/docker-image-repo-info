## `clojure:temurin-19-bullseye-slim`

```console
$ docker pull clojure@sha256:d87d6a89dcd9b5a6dfa704af724dc8ac1fc80681ebee661445bc0d6ee3ff71a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:8a02ca3020ad67e9c80e08e089677fb970dcdc97399d8b891f4ac7a48409be6b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.0 MB (294015003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a895a32675ef74026d5f5c2659ea82e41b11348a01f0484757a20eb7810688cf`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:17:46 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:25:51 GMT
COPY dir:94cb5af8175285c10c94286222d8a35302f3f8c290e00011a75c67156659d6ab in /opt/java/openjdk 
# Thu, 23 Mar 2023 06:25:53 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:27:32 GMT
ENV CLOJURE_VERSION=1.11.1.1257
# Thu, 23 Mar 2023 06:27:32 GMT
WORKDIR /tmp
# Thu, 23 Mar 2023 06:27:47 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "be032cf21dc67ecf072f7254a01c3587d97aa311198f53cd1a1777ddfb3e9244 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 23 Mar 2023 06:27:48 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 23 Mar 2023 06:27:48 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Thu, 23 Mar 2023 06:27:48 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 23 Mar 2023 06:27:48 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d50160c605f9c02acd78ef392f7194eee61162e99ab69aa71a85d2c04e97ff86`  
		Last Modified: Thu, 23 Mar 2023 06:34:39 GMT  
		Size: 201.1 MB (201112949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8667ae93d847ed996d363be7df371f02164750c398e891b347fe86280d523ac8`  
		Last Modified: Thu, 23 Mar 2023 06:35:31 GMT  
		Size: 61.5 MB (61489634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5237831ab30e101b79015d88e1196ec444757d7ed1b0378afc603ac238ce9ee`  
		Last Modified: Thu, 23 Mar 2023 06:35:23 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea4cd427ad240dfa55ef31696bedf1f3406e67d0d6ba6b6f61a82aec1d73b076`  
		Last Modified: Thu, 23 Mar 2023 06:35:23 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:e51fa6ebfb67c53427d0971a5796835bb907f8489da5e19d5c5a0522395f634c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.5 MB (291523642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0dca71d9494b078239641b813e6ba36590c0cf6da6653473bd4ff3d1cacb67a`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:52:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:59:40 GMT
COPY dir:9a6a873ca11063f6f04e7f088397a1fce771e2b1aa8590b72eb07158cfac883f in /opt/java/openjdk 
# Thu, 23 Mar 2023 06:59:44 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 07:01:10 GMT
ENV CLOJURE_VERSION=1.11.1.1257
# Thu, 23 Mar 2023 07:01:10 GMT
WORKDIR /tmp
# Thu, 23 Mar 2023 07:01:24 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "be032cf21dc67ecf072f7254a01c3587d97aa311198f53cd1a1777ddfb3e9244 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 23 Mar 2023 07:01:24 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 23 Mar 2023 07:01:24 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Thu, 23 Mar 2023 07:01:24 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 23 Mar 2023 07:01:24 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274b1a27e7816b7f1e1f1324be385765b25723b5eddb3f339875cd4a1fa13c6e`  
		Last Modified: Thu, 23 Mar 2023 07:07:40 GMT  
		Size: 199.9 MB (199855165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5960bd22b347b59e49d599de91065229929673b93616c5c18c21f0b2da6e6fc`  
		Last Modified: Thu, 23 Mar 2023 07:08:32 GMT  
		Size: 61.6 MB (61604760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ddfc60c7d16c91d51eee1f3de07ee7cb9bdd0ae39345ca73d0592bfcd9bc08`  
		Last Modified: Thu, 23 Mar 2023 07:08:26 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b8914d10ae0698b4e8428b1ce1ae4fb124b7f1c9aa91f4e81bb46073d8aa70`  
		Last Modified: Thu, 23 Mar 2023 07:08:26 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
