## `clojure:temurin-11-tools-deps-1.11.1.1224-bullseye`

```console
$ docker pull clojure@sha256:929b893cfd51a9e7bd1fdd30b6c1a8881a49ab7db472950ada615e92123f5d5b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `clojure:temurin-11-tools-deps-1.11.1.1224-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:ecba652396493f003c949b5a35f333b408ed3bf3e059e4dd1c3beae17e20a957
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.9 MB (320935637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:201f0841a4816f2983dde36245dd518d7fce8ae482622ffd07ba9f4b046900be`
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
# Mon, 13 Feb 2023 20:43:24 GMT
ENV CLOJURE_VERSION=1.11.1.1224
# Mon, 13 Feb 2023 20:43:24 GMT
WORKDIR /tmp
# Mon, 13 Feb 2023 20:43:38 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "3bbab4d253eda43e3122fd5705014a69c44944a6dee8ea4d7d567afe157eb4ef *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Mon, 13 Feb 2023 20:43:39 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Mon, 13 Feb 2023 20:43:39 GMT
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
	-	`sha256:7567efa076501d7a499bbbdd01dc348eaec88358df98ca7a3387ee96eaf9e534`  
		Last Modified: Mon, 13 Feb 2023 20:51:39 GMT  
		Size: 72.0 MB (71991326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9dc962f2e0984a5ab12eea5e42d9fb854022e01f37e2a522fca5a406e54f9df`  
		Last Modified: Mon, 13 Feb 2023 20:51:32 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
