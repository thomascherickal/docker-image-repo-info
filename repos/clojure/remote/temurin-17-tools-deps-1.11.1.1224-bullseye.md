## `clojure:temurin-17-tools-deps-1.11.1.1224-bullseye`

```console
$ docker pull clojure@sha256:20b89d2d065b74b81c1e79ad0d37ef26d98cf8e5e747e42584e6e4853ee2b663
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-tools-deps-1.11.1.1224-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:33a1423cd9186aa4e359b6af597a20086d1f8070813d6ada735b35f789ffee61
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.4 MB (319363293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e044d06d34f75e232630a51b99ef0ab057bdd47c2202023895f331b54269c6b7`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:40:41 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Mar 2023 07:46:48 GMT
COPY dir:5cf52f938fe415b0022fbccb8cf978562c503c0b8313cc9dedf46c1c4edb35cf in /opt/java/openjdk 
# Wed, 01 Mar 2023 07:46:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 07:48:51 GMT
ENV CLOJURE_VERSION=1.11.1.1224
# Wed, 01 Mar 2023 07:48:51 GMT
WORKDIR /tmp
# Wed, 01 Mar 2023 07:49:08 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "3bbab4d253eda43e3122fd5705014a69c44944a6dee8ea4d7d567afe157eb4ef *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 01 Mar 2023 07:49:09 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 01 Mar 2023 07:49:09 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 01 Mar 2023 07:49:09 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 01 Mar 2023 07:49:09 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2398cb32ac1a57ed5e07eacb837ab8e304b5c7c8726bc0e525810f442bb47c`  
		Last Modified: Wed, 01 Mar 2023 07:58:35 GMT  
		Size: 192.4 MB (192438071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12bad482b6e97fa618bf8d92e80e43c9e77cb15916edc29d3aaae4d1daf9d68`  
		Last Modified: Wed, 01 Mar 2023 07:59:54 GMT  
		Size: 71.9 MB (71878284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430175498ed76275d0c32c2cdf77d2313f8af1b4fab9d1b23a39e3d14d8428c1`  
		Last Modified: Wed, 01 Mar 2023 07:59:46 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d754726a67dfb77b7b6936347eec473bb46588db1d6bf737a22f71f8c620f3e`  
		Last Modified: Wed, 01 Mar 2023 07:59:46 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-tools-deps-1.11.1.1224-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:ecd3f55679633b78ef5024940ac37a5fc51123f044262fcffd028fe85faa4753
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.0 MB (316954390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:135101c58dc8f991a3fecfb0c0dd9961b61bb704b7f8184c38cf9a599a09ca7f`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:30 GMT
ADD file:a6a1df499d0d5b07fb366d776a11c42ddee6261e2425a921041b38e868192770 in / 
# Wed, 01 Mar 2023 02:20:30 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:01:14 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 02 Mar 2023 07:06:32 GMT
COPY dir:47c117bbc947c5c1164b5a20eeec0ba16c306f5991a85f22c54db31ca24ce4a8 in /opt/java/openjdk 
# Thu, 02 Mar 2023 07:06:36 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 07:09:19 GMT
ENV CLOJURE_VERSION=1.11.1.1224
# Thu, 02 Mar 2023 07:09:19 GMT
WORKDIR /tmp
# Thu, 02 Mar 2023 07:09:33 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "3bbab4d253eda43e3122fd5705014a69c44944a6dee8ea4d7d567afe157eb4ef *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 02 Mar 2023 07:09:34 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 02 Mar 2023 07:09:34 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Thu, 02 Mar 2023 07:09:34 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 02 Mar 2023 07:09:34 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:0f5fe16b1836feccd4765ac5685fc7a7b9c73445cac94fc595d2ffbc3cb59a7a`  
		Last Modified: Wed, 01 Mar 2023 02:23:53 GMT  
		Size: 53.7 MB (53703215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d4bb35cb769be425f0d1c938b7ff57112e361f17e432495be72cb2032f4d92`  
		Last Modified: Thu, 02 Mar 2023 07:20:00 GMT  
		Size: 191.3 MB (191260440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af64b03b91e29d59a4c0f521ba6272f9f98a4e48d8b15e5471be29797ec08b37`  
		Last Modified: Thu, 02 Mar 2023 07:22:11 GMT  
		Size: 72.0 MB (71989717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85b9dca6b3db603c30e8e352b97bd76c3cc9aa47027677b4c2ea68655707700`  
		Last Modified: Thu, 02 Mar 2023 07:22:05 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad9857f243bfaf2ef5f56f471d76b8d40d502d0ab3e5f27947bb449f710701b`  
		Last Modified: Thu, 02 Mar 2023 07:22:04 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
