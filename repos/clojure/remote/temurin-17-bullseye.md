## `clojure:temurin-17-bullseye`

```console
$ docker pull clojure@sha256:00eecee9aa078dd0d718a1abdf855b324210fbc4db70251ccaadf9e9d3962020
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:310b05c4581122081ca75ca0578c43421b6d7f97317adcdd0bb1648c48528ce5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.8 MB (294785194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1833281b656af202c401c1f827bdc6954e6d7e10e89b9e5b1647fffcd6a94e7`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:41 GMT
ADD file:553d20b03d45305e58cde07e0c259421bba044155ac90b4559e5cc0b69093347 in / 
# Tue, 06 Dec 2022 01:20:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:48:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 06:41:36 GMT
COPY dir:6d447c71fb5cab25c46568db16879377c790ade488ebb14a9cc6935f6b8bd709 in /opt/java/openjdk 
# Fri, 09 Dec 2022 06:41:37 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 06:44:45 GMT
ENV CLOJURE_VERSION=1.11.1.1200
# Fri, 09 Dec 2022 06:44:46 GMT
WORKDIR /tmp
# Fri, 09 Dec 2022 06:45:00 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "694381cb78d44f143bdcc38657507f012ebac4009bc57cec67abef1675447878 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 09 Dec 2022 06:45:01 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 09 Dec 2022 06:45:01 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 09 Dec 2022 06:45:01 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 09 Dec 2022 06:45:01 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698`  
		Last Modified: Tue, 06 Dec 2022 01:24:48 GMT  
		Size: 55.0 MB (55041342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd66dd8de79208b3ac1ba78188137da46ecd5c4585e3964d2bf9fe06372b58aa`  
		Last Modified: Fri, 09 Dec 2022 06:56:44 GMT  
		Size: 192.4 MB (192431275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc42eff892d43a8da7721989a5f276dbef8d7b5febbf6c17b97f8c0c1346e2e7`  
		Last Modified: Fri, 09 Dec 2022 06:58:55 GMT  
		Size: 47.3 MB (47311564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc709e2b3bbbd5ba2c1e72c47740b053e905870f43756d9a7c2a6f5e053a958`  
		Last Modified: Fri, 09 Dec 2022 06:58:49 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58c875d485a33901930a235dc7834b9eab15f0127e47bb65829cb866cd9d81d7`  
		Last Modified: Fri, 09 Dec 2022 06:58:49 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:ff771e99bcfb953494554994c3352a4c6bd5553ae9097eeb9b0fca215708a7e3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.2 MB (292219515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59316c1b23b9b9436beb5f895e3110e9958e143a3e4c8657a7f49084fd5b516f`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:06 GMT
ADD file:b1e7652678bbfc9556636e77d79c947ff1436888e2929f9c5c3ddb42a50c1176 in / 
# Tue, 06 Dec 2022 01:40:07 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:17:15 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 05:07:54 GMT
COPY dir:533cfee1c12b6052cd1297ebc89704c8b7da6e8016c06b0e341bcec0d4934dde in /opt/java/openjdk 
# Fri, 09 Dec 2022 05:07:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 05:10:41 GMT
ENV CLOJURE_VERSION=1.11.1.1200
# Fri, 09 Dec 2022 05:10:41 GMT
WORKDIR /tmp
# Fri, 09 Dec 2022 05:10:52 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "694381cb78d44f143bdcc38657507f012ebac4009bc57cec67abef1675447878 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 09 Dec 2022 05:10:53 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 09 Dec 2022 05:10:53 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 09 Dec 2022 05:10:53 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 09 Dec 2022 05:10:53 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:4948a51a9a3f176f30ac619014f4a2da453a943244eacb53096ee9742eb7cef1`  
		Last Modified: Tue, 06 Dec 2022 01:43:33 GMT  
		Size: 53.7 MB (53699146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7e87ae6358ff8aab3fb41f68232225878ffb398969ae416f8e58ce122fdb05`  
		Last Modified: Fri, 09 Dec 2022 05:21:15 GMT  
		Size: 191.2 MB (191215204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ef1cadebc2eead3bb7d10870698b531d54154c33332f87e6dc7119cc0955be`  
		Last Modified: Fri, 09 Dec 2022 05:23:19 GMT  
		Size: 47.3 MB (47304148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d18f67ee91a928053e6aa689e950cf6cc3b04ea0861723fa6bab15bdacc054`  
		Last Modified: Fri, 09 Dec 2022 05:23:14 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18066b4be5483753f0dadc8e8eb9ad1597e37750f828c73ac566917c844791c`  
		Last Modified: Fri, 09 Dec 2022 05:23:14 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
