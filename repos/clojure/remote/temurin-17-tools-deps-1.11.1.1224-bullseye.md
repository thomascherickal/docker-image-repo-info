## `clojure:temurin-17-tools-deps-1.11.1.1224-bullseye`

```console
$ docker pull clojure@sha256:0ed09824eb65a448d666858e917536ab679bee14d3a0553a66fce8ef063c47be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `clojure:temurin-17-tools-deps-1.11.1.1224-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:630b4543dddb8cd3875d88b8a9577c7aff0b4ebc6365ce07d5103c72394d6346
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.0 MB (316955894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bd9a2cf113eaf187b5c4c8b0a422e9aaf76726c8ba160c713a206a06594c7e4`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:29 GMT
ADD file:5cf2de182dac36d99ec41918889c9755f9c49c56fa0a8d0ca14040c1d8c04541 in / 
# Thu, 09 Feb 2023 03:58:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:23:26 GMT
COPY dir:a1bd99c3d82513db94430c73467e1e5c69ea4624d0489571d594afe503e15dc5 in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:23:31 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 13 Feb 2023 20:44:47 GMT
ENV CLOJURE_VERSION=1.11.1.1224
# Mon, 13 Feb 2023 20:44:47 GMT
WORKDIR /tmp
# Mon, 13 Feb 2023 20:45:01 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "3bbab4d253eda43e3122fd5705014a69c44944a6dee8ea4d7d567afe157eb4ef *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Mon, 13 Feb 2023 20:45:01 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Mon, 13 Feb 2023 20:45:01 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Mon, 13 Feb 2023 20:45:02 GMT
ENTRYPOINT ["entrypoint"]
# Mon, 13 Feb 2023 20:45:02 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:80dae1b9d879348c210c40024c6e90ef92677ac3515456375fcbb70bdf07b104`  
		Last Modified: Thu, 09 Feb 2023 04:02:11 GMT  
		Size: 53.7 MB (53703368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58beb3d7fb4976caa5ecfe5652ba8512378861c8fbbb227ff0dee4db622d0e2`  
		Last Modified: Thu, 09 Feb 2023 09:34:05 GMT  
		Size: 191.3 MB (191260472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42787068cfcb963face6349cd4f3fec4d0a14bbea88d6deb2465adb80a464a47`  
		Last Modified: Mon, 13 Feb 2023 20:53:08 GMT  
		Size: 72.0 MB (71991032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223076fac6616cf7ad442d37b942766cbfc6e22c474f45aecac15c2bcc1b6302`  
		Last Modified: Mon, 13 Feb 2023 20:53:01 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3adc55b9ff2b5bed60f6ad0393a18b5b1bada0d293867ce78b55b7538453295e`  
		Last Modified: Mon, 13 Feb 2023 20:53:01 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
