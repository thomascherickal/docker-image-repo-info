## `clojure:temurin-17-tools-deps-bullseye`

```console
$ docker pull clojure@sha256:ad2d583f1dcf1907f7f66c9efc0aa8b2b801ddd979a2e14e4958bcc266674357
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
$ docker pull clojure@sha256:0ceca41d1ae3e95b708aa5c57df8349d29c353dcc64c0e3170a735ba54753fcb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.0 MB (316952097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82a45799f35160f82ecf9800c75f9c3ed8df8484330994925d6994df281a3baa`
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
# Thu, 09 Feb 2023 09:25:13 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Thu, 09 Feb 2023 09:25:13 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:25:27 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 09 Feb 2023 09:25:28 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 09 Feb 2023 09:25:28 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Thu, 09 Feb 2023 09:25:28 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 09 Feb 2023 09:25:28 GMT
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
	-	`sha256:bee838b547b38c95c7e13746cccc0c59eefd5be45cd25c5b84d235145483f1ca`  
		Last Modified: Thu, 09 Feb 2023 09:35:09 GMT  
		Size: 72.0 MB (71987235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2ffd6e91e76657f91ffe95bc0a09625bc29d52f5b36ec008e475761678cea5`  
		Last Modified: Thu, 09 Feb 2023 09:35:02 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6d0a99c6b694765fffdba9afc2857f4e5d2d48640d0ddd142338f64d06a099`  
		Last Modified: Thu, 09 Feb 2023 09:35:02 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
