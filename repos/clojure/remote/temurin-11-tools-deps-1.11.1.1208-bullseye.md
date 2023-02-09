## `clojure:temurin-11-tools-deps-1.11.1.1208-bullseye`

```console
$ docker pull clojure@sha256:cb22788a4814d9b356df4745d97adf0649691f730d07155ed1f09a0eea304574
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-tools-deps-1.11.1.1208-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:b7288d177e50441154c6ddd28079eb6cd90ca99f5473dbc813e0709f0229a388
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.4 MB (325390937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:790256be9b6ac75ba8f35afc9d37643d6eebd957c7aa693c46dcbabcd7e95fa4`
-	Default Command: `["clj"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:05 GMT
ADD file:b03d13d345c29f69557f410c8504e748226756d1f48e5abdb63cd40179b2640c in / 
# Thu, 09 Feb 2023 03:20:05 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:25:04 GMT
COPY dir:fdbc5e9dec2946fa124877176e92a68dd3fe3a70def5bb906a6040c4a1303a2d in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:25:06 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:27:08 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Thu, 09 Feb 2023 09:27:09 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:27:26 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 09 Feb 2023 09:27:27 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 09 Feb 2023 09:27:27 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:1e4aec178e0864db93a6f97a20bde3445871a4562c1801185eca1238d3a0e80d`  
		Last Modified: Thu, 09 Feb 2023 03:24:47 GMT  
		Size: 55.0 MB (55046771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36fa5505d5f9a403b5fa799c74b7639e1188ddc30c0db155b99238ff035c03ed`  
		Last Modified: Thu, 09 Feb 2023 09:38:26 GMT  
		Size: 198.5 MB (198475422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:445e49a3de549b96bddaf0c3c3144fe7cc28e2dbaf5ad4d21f2d44a2b483610e`  
		Last Modified: Thu, 09 Feb 2023 09:39:29 GMT  
		Size: 71.9 MB (71868124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5f3af5454dc21787e776018a4b6b16978576ed57ac4ff6bdfa3bf113212a7a`  
		Last Modified: Thu, 09 Feb 2023 09:39:21 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-tools-deps-1.11.1.1208-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:455e3e723990a10869a05af87ae9b33835dee428a947aaa66e8ffde5008a5284
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.9 MB (320931286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8da2fbe1ea49082848ace95e915c04df172ca0193e2fd6e395118cee57de61ca`
-	Default Command: `["clj"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:29 GMT
ADD file:5cf2de182dac36d99ec41918889c9755f9c49c56fa0a8d0ca14040c1d8c04541 in / 
# Thu, 09 Feb 2023 03:58:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:17:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:20:57 GMT
COPY dir:b661686bf8d434588756c45f2ef6e7f314f32f753cf180ef8fb45397388f098c in /opt/java/openjdk 
# Thu, 09 Feb 2023 09:21:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 09:22:44 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Thu, 09 Feb 2023 09:22:44 GMT
WORKDIR /tmp
# Thu, 09 Feb 2023 09:22:57 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 09 Feb 2023 09:22:58 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 09 Feb 2023 09:22:58 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:80dae1b9d879348c210c40024c6e90ef92677ac3515456375fcbb70bdf07b104`  
		Last Modified: Thu, 09 Feb 2023 04:02:11 GMT  
		Size: 53.7 MB (53703368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84634f2412fd0db390d1dd82c75871f25a933e1333ec652a66114e5288d4d33f`  
		Last Modified: Thu, 09 Feb 2023 09:32:24 GMT  
		Size: 195.2 MB (195240325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e826677487139e20720ea6bedfe55a408793c2bf8e6805b57437d2099b87bba`  
		Last Modified: Thu, 09 Feb 2023 09:33:23 GMT  
		Size: 72.0 MB (71986975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fa272b3e59c2df0df08fc4ecac2b0fc2b93d9200796220fe77451e467f3bf4`  
		Last Modified: Thu, 09 Feb 2023 09:33:16 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
