## `clojure:temurin-20-tools-deps-1.11.1.1347-bullseye`

```console
$ docker pull clojure@sha256:fb3460dbb3fb92203bf8528cba1fc812dd14928e76475453cb0d7f2296c1246d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-20-tools-deps-1.11.1.1347-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:2992439abf80dfd1a286022904709abc3eb68974b5238691df6bbe27ab9a3f50
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.8 MB (329751417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90fe3a387b1a3ef216ed20f9e9c95fb2c939bce154f3a883f3d7322e4568aabf`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:43:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 03:52:38 GMT
COPY dir:02736280d197ac4d1b6ebf68d948efb46e7eeffd579505356f8c94946dbcce6f in /opt/java/openjdk 
# Tue, 13 Jun 2023 03:52:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 03:53:32 GMT
ENV CLOJURE_VERSION=1.11.1.1347
# Tue, 13 Jun 2023 03:53:32 GMT
WORKDIR /tmp
# Tue, 13 Jun 2023 03:53:48 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "d9158bf3a1d92fbf8551656e47a86f42e93d10f1db9defa2124bfee206ce8c8f *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 13 Jun 2023 03:53:49 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 13 Jun 2023 03:53:49 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 13 Jun 2023 03:53:49 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 13 Jun 2023 03:53:49 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:93c2d578e4211e82e47e7ada9ed05d1869a2362c6f7509f2ee8d91ccebfb7fbd`  
		Last Modified: Mon, 12 Jun 2023 23:26:08 GMT  
		Size: 55.1 MB (55055162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff552612282fa24c92a5dfa87c11041f0b4f4d7cd27c3ce8fb2a67f243f9330`  
		Last Modified: Tue, 13 Jun 2023 04:00:38 GMT  
		Size: 202.8 MB (202814025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c4c5e74339bbb3794174b37168b0ccacbd874759084dac391eaeea3060e6af`  
		Last Modified: Tue, 13 Jun 2023 04:01:21 GMT  
		Size: 71.9 MB (71881216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e3387aeafa798def23c842ad476fd6d03955c82d1d619a0af77473433eaa42`  
		Last Modified: Tue, 13 Jun 2023 04:01:13 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ce436b74d240225aa876d8029a13171f20a9f2a615840f126a368a5c05dcbe`  
		Last Modified: Tue, 13 Jun 2023 04:01:13 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-20-tools-deps-1.11.1.1347-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:1591bcd964018c0f61d7bb20acdad5917d06b90ee170529eb5181854274afde6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.9 MB (326860213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b0b77461398118e973232ac390c99414004e27e21a85443e5b4bbfa11a73c7d`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:22 GMT
ADD file:caddd2f40296ec5c1bf7487617ca8694cfff9a1d9b7484159e203b6514cb5f5f in / 
# Mon, 12 Jun 2023 23:40:23 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:50:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 04:57:52 GMT
COPY dir:f555428af67a610819205eec573e23f479077e0999818ee9dc0f3375599d21db in /opt/java/openjdk 
# Tue, 13 Jun 2023 04:57:57 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 04:58:42 GMT
ENV CLOJURE_VERSION=1.11.1.1347
# Tue, 13 Jun 2023 04:58:42 GMT
WORKDIR /tmp
# Tue, 13 Jun 2023 04:58:56 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "d9158bf3a1d92fbf8551656e47a86f42e93d10f1db9defa2124bfee206ce8c8f *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 13 Jun 2023 04:58:57 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 13 Jun 2023 04:58:57 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 13 Jun 2023 04:58:57 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 13 Jun 2023 04:58:57 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:663ccfaf62a5d7b997bca03d1dc6d5dfff01b9e0de08d86dbea8957ea92d7d16`  
		Last Modified: Mon, 12 Jun 2023 23:44:25 GMT  
		Size: 53.7 MB (53704136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7fbc4a56457275b512e08117bbea540a06635c8ef73e73b83254270abe2921`  
		Last Modified: Tue, 13 Jun 2023 05:04:44 GMT  
		Size: 201.2 MB (201158012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40544225a78e0dca4534d195a78b5be0a2312b35b126f85f07da844ef762f49`  
		Last Modified: Tue, 13 Jun 2023 05:05:20 GMT  
		Size: 72.0 MB (71997055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d146f5901339d7ecff55f91a5009b65a0647612eaa9ff702aa8fcfa33cc419`  
		Last Modified: Tue, 13 Jun 2023 05:05:14 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd8fe1e2d1d24d35be647ffa622119b5f884868b6020bf65cca4984cf422581`  
		Last Modified: Tue, 13 Jun 2023 05:05:13 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
