## `clojure:temurin-17-tools-deps-1.11.1.1208-bullseye`

```console
$ docker pull clojure@sha256:57e553212271c49b5795cd968faaf5ba4f5a9faf9729a2d225cb3ca29d81b4a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-tools-deps-1.11.1.1208-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:70b9213a4ae78fe4de17177b5fdf134fbf46782793336993a2166e628fc37730
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.3 MB (319322551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c89be606d42e511ff70ec89d7aa75ba0d16b93a46db3dd2203ac82b0a9d512f`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:29 GMT
ADD file:917750a82b29f8f7f88a121017bd9dfeb0fbcc8f0697a009f08b6b58246eff4b in / 
# Wed, 11 Jan 2023 02:34:30 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:18:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 25 Jan 2023 00:45:22 GMT
COPY dir:bb223240e99e5b7e66eb621e33f54e49ced87035f56dd975e567c739be4bfe96 in /opt/java/openjdk 
# Wed, 25 Jan 2023 00:45:24 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 25 Jan 2023 00:48:50 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Wed, 25 Jan 2023 00:48:51 GMT
WORKDIR /tmp
# Wed, 25 Jan 2023 00:49:08 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 25 Jan 2023 00:49:08 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 25 Jan 2023 00:49:08 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 25 Jan 2023 00:49:08 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 25 Jan 2023 00:49:08 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:bbeef03cda1f5d6c9e20c310c1c91382a6b0a1a2501c3436b28152f13896f082`  
		Last Modified: Wed, 11 Jan 2023 02:38:42 GMT  
		Size: 55.0 MB (55025206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147288dc8989fb24ee233733fb7ef84c2cf5d7be2f0863fe9ea1e153e52a350f`  
		Last Modified: Wed, 25 Jan 2023 00:57:58 GMT  
		Size: 192.4 MB (192438164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea27bab58af737d7f15321e929da41aa312ebf5960d8d7e89cd08b7fa67f753`  
		Last Modified: Wed, 25 Jan 2023 01:00:43 GMT  
		Size: 71.9 MB (71858164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ec119728120183842cfe525503969ffdc11b6723e15b2ab92ae1382872f498`  
		Last Modified: Wed, 25 Jan 2023 01:00:34 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506923c3df97f5d178cf9f5b6f8ef7cfac10698d44697682bbe7f200e4124c9a`  
		Last Modified: Wed, 25 Jan 2023 01:00:34 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-tools-deps-1.11.1.1208-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:5dd77ad52aee150f7c8abf34a722479eeab63a6f5e0b74781fbc1556c83dd6a0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.9 MB (316927819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee7014b6efab000e7e2b9dd5c354ea8cc92ced9d0179644b5e905442a2fb243b`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:24 GMT
ADD file:9e185c2d9ca8a231a39ee2b1761fcdff75065252d25a65a207acb7a319c1cf23 in / 
# Wed, 11 Jan 2023 02:57:25 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:38:14 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 20:54:01 GMT
COPY dir:a1bd99c3d82513db94430c73467e1e5c69ea4624d0489571d594afe503e15dc5 in /opt/java/openjdk 
# Tue, 31 Jan 2023 20:54:05 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 20:56:47 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Tue, 31 Jan 2023 20:56:47 GMT
WORKDIR /tmp
# Tue, 31 Jan 2023 20:57:01 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 31 Jan 2023 20:57:01 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 31 Jan 2023 20:57:01 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 31 Jan 2023 20:57:01 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 31 Jan 2023 20:57:01 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:c345c9e441f5f49235768af74b8ab37743652d38958afaa000edd56d7b2f0540`  
		Last Modified: Wed, 11 Jan 2023 03:00:56 GMT  
		Size: 53.7 MB (53681859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f61d91708311a5923680a9fa5ce56fc7a173443a91b20c1941a3baab459e19`  
		Last Modified: Tue, 31 Jan 2023 21:07:15 GMT  
		Size: 191.3 MB (191260441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de9c4442b99f60afab884ff80fecb42bf468ee8f08cd91e280fe886741bfebf`  
		Last Modified: Tue, 31 Jan 2023 21:09:22 GMT  
		Size: 72.0 MB (71984503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc7d3e994b0b344adbdedb96142c70c0180dbe3c3ec9a669be3a6033d317f14`  
		Last Modified: Tue, 31 Jan 2023 21:09:15 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f4ea8309851549f1db0d39a37db451bc8c11a4a7ad8a1c7409a65c742e5e5e`  
		Last Modified: Tue, 31 Jan 2023 21:09:15 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
