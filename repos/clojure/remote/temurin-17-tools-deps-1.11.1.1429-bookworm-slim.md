## `clojure:temurin-17-tools-deps-1.11.1.1429-bookworm-slim`

```console
$ docker pull clojure@sha256:75c24e4f7f061e6031ac8799c68af3c6e90710a4037e732ad6e5bb1773807dce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-17-tools-deps-1.11.1.1429-bookworm-slim` - linux; amd64

```console
$ docker pull clojure@sha256:0b7a722cc2d1f0c663e29b8af690ac808c301b6b7af88d8388269d39fd3e01d7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.2 MB (246168791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cc972f0a17b08c5859986dba40febd0707dd8eb4cd32f44ba025e16b7969943`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:08:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 10:02:19 GMT
COPY dir:e13dbcd57950f4d4d23f4aba8428b6fbbf838d8f4801d32a25e344d37d33c37e in /opt/java/openjdk 
# Sat, 02 Dec 2023 10:02:20 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 18:29:21 GMT
ENV CLOJURE_VERSION=1.11.1.1429
# Tue, 05 Dec 2023 18:29:21 GMT
WORKDIR /tmp
# Tue, 05 Dec 2023 18:29:38 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "bf08cfeb007118b7277aa7423734f5d507604b868f7fc44c0f9929ca9cd94ed4 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 05 Dec 2023 18:29:39 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 05 Dec 2023 18:29:39 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 05 Dec 2023 18:29:39 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 05 Dec 2023 18:29:39 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0885deee54f6adeddb534e83c7fede08982afb277d99e56cc4f45a0a4902c5d`  
		Last Modified: Sat, 02 Dec 2023 10:18:38 GMT  
		Size: 144.9 MB (144873901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a80db499f42aa49344ec688dcc644e36b0e56943631a1a6aa8fb7ebcc9df99`  
		Last Modified: Tue, 05 Dec 2023 18:40:57 GMT  
		Size: 72.1 MB (72143966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38547c72cb109caa22207dc1db305037a7c48a4e28f9831debd7a18f021b61a`  
		Last Modified: Tue, 05 Dec 2023 18:40:49 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0ee5073123f7d845744ccbc0d5df25a81bfe9c815e47064a32068419eccb52`  
		Last Modified: Tue, 05 Dec 2023 18:40:49 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
