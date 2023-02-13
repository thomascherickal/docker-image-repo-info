## `clojure:temurin-17-tools-deps-bullseye`

```console
$ docker pull clojure@sha256:bcb91f516114cf2ddd6af2e90376303db7306b5e7fd8492ec91ca5b6099cd3c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-tools-deps-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:256bb43030b667a0500be7891be36dcc018f17383d288ed744e7fdcacb412211
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.4 MB (319353799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a821e6503440d2f464773c896998cdbe4af4ccf018e97c222f39d60b9d1869c8`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:05 GMT
ADD file:b03d13d345c29f69557f410c8504e748226756d1f48e5abdb63cd40179b2640c in / 
# Thu, 09 Feb 2023 03:20:05 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:28:07 GMT
COPY dir:5cf52f938fe415b0022fbccb8cf978562c503c0b8313cc9dedf46c1c4edb35cf in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:28:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:30:11 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Thu, 09 Feb 2023 09:30:11 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:30:28 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 09 Feb 2023 09:30:29 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 09 Feb 2023 09:30:29 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Thu, 09 Feb 2023 09:30:29 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 09 Feb 2023 09:30:29 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:1e4aec178e0864db93a6f97a20bde3445871a4562c1801185eca1238d3a0e80d`  
		Last Modified: Thu, 09 Feb 2023 03:24:47 GMT  
		Size: 55.0 MB (55046771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1f93ea764dcf05c1b60ac69868cb3e583d17322a93bc9f10b76202e4b5f41e`  
		Last Modified: Thu, 09 Feb 2023 09:40:17 GMT  
		Size: 192.4 MB (192438166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d49ff24d82782600c063b01159dd9369b9f798ea7bb62d5f2fc444d0875091`  
		Last Modified: Thu, 09 Feb 2023 09:41:33 GMT  
		Size: 71.9 MB (71867843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff1169c2e340041fdc0936017dbdd9f2dc3d1f1006fe746d40eef3daeeb0a1b`  
		Last Modified: Thu, 09 Feb 2023 09:41:19 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcdaf349bd5a88a46c968d59572f462cb713e850f78ceb7439a67e1e3c1189c4`  
		Last Modified: Thu, 09 Feb 2023 09:41:19 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-tools-deps-bullseye` - linux; arm64 variant v8

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
