## `clojure:openjdk-19-tools-deps`

```console
$ docker pull clojure@sha256:6a9201acac853dbd8768181eaf1dd043411006936a5440b1a7cb8b493b9f31f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-19-tools-deps` - linux; amd64

```console
$ docker pull clojure@sha256:db49cb5e684ad934ec16c6696777f2b41760d84d32061ced90fd1f84925b2177
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.3 MB (288329222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2660a7e540f460b4bfd67a74e7b53c7fe30f8f12d6eb41ad0fa9566c0f049ef7`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 10:47:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:47:39 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Wed, 20 Apr 2022 10:47:39 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 10:47:40 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 10:47:40 GMT
ENV JAVA_VERSION=19-ea+18
# Wed, 20 Apr 2022 10:47:54 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/18/GPL/openjdk-19-ea+18_linux-x64_bin.tar.gz'; 			downloadSha256='c79b13e466464b0054cad0301cf53bcd4b083d591f5fe61e932f39d34063f93b'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/18/GPL/openjdk-19-ea+18_linux-aarch64_bin.tar.gz'; 			downloadSha256='eeec6bd83fea107d1c6de91d7eb2936b7829e8315e81458beb4e401a9f51f006'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 20 Apr 2022 10:47:55 GMT
CMD ["jshell"]
# Thu, 21 Apr 2022 00:44:06 GMT
ENV CLOJURE_VERSION=1.11.1.1105
# Thu, 21 Apr 2022 00:44:06 GMT
WORKDIR /tmp
# Thu, 21 Apr 2022 00:44:22 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "5655c3ee3ea495d0778d8a87ce05a719045d3ceae9dd5cc29033379d8f82cce5 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 21 Apr 2022 00:44:22 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 21 Apr 2022 00:44:22 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Thu, 21 Apr 2022 00:44:22 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 21 Apr 2022 00:44:22 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d3aa8d076675d49d85180b0ced9daef210fe4fdff4bdbb422b9cf384e591d0`  
		Last Modified: Wed, 20 Apr 2022 11:01:25 GMT  
		Size: 1.6 MB (1582162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec81747289a74f92d409fda762e1d848247d7063e6d0ede76ba77831fb67ef71`  
		Last Modified: Wed, 20 Apr 2022 11:01:40 GMT  
		Size: 194.9 MB (194918667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6154aabe00618ed89429d66d31b8b5bae181201e90d56b9028ace70e4a537687`  
		Last Modified: Thu, 21 Apr 2022 01:03:08 GMT  
		Size: 60.4 MB (60448384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9e7c72422a865173f94288ff1a3f0c5d1baaf15c4943dea01ef7c9bf790ffc`  
		Last Modified: Thu, 21 Apr 2022 01:03:01 GMT  
		Size: 624.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31893046ba1174a3eccfd27c52dc84f284ec86a597b0da2786736c8320568418`  
		Last Modified: Thu, 21 Apr 2022 01:03:01 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-19-tools-deps` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:9341e832224ee50aafe05c91d510a452769d80d6890c24af17f6cf02129ff220
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.4 MB (285358092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04ee837b49580e239289c8b4a4e0ca836060bbec9c450798a28994318536794d`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:10 GMT
ADD file:84523b5820128293b713ef35d8db618921162250da1e4c72bf9923f34ad7d87d in / 
# Wed, 20 Apr 2022 04:29:11 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 10:24:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:24:39 GMT
ENV JAVA_HOME=/usr/local/openjdk-19
# Wed, 20 Apr 2022 10:24:40 GMT
ENV PATH=/usr/local/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 10:24:41 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 10:24:42 GMT
ENV JAVA_VERSION=19-ea+18
# Wed, 20 Apr 2022 10:24:56 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/18/GPL/openjdk-19-ea+18_linux-x64_bin.tar.gz'; 			downloadSha256='c79b13e466464b0054cad0301cf53bcd4b083d591f5fe61e932f39d34063f93b'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/18/GPL/openjdk-19-ea+18_linux-aarch64_bin.tar.gz'; 			downloadSha256='eeec6bd83fea107d1c6de91d7eb2936b7829e8315e81458beb4e401a9f51f006'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 20 Apr 2022 10:24:56 GMT
CMD ["jshell"]
# Thu, 21 Apr 2022 03:37:25 GMT
ENV CLOJURE_VERSION=1.11.1.1105
# Thu, 21 Apr 2022 03:37:25 GMT
WORKDIR /tmp
# Thu, 21 Apr 2022 03:37:41 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "5655c3ee3ea495d0778d8a87ce05a719045d3ceae9dd5cc29033379d8f82cce5 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 21 Apr 2022 03:37:42 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 21 Apr 2022 03:37:43 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Thu, 21 Apr 2022 03:37:43 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 21 Apr 2022 03:37:44 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:6d4a449ac69c579312443ded09f57c4894e7adb42f7406abd364f95982fafc59`  
		Last Modified: Wed, 20 Apr 2022 04:35:49 GMT  
		Size: 30.1 MB (30065801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59f13dc084e185af417a4c6d1be2534adaff0c4f35ac2166a539260f4e8e945`  
		Last Modified: Wed, 20 Apr 2022 10:46:08 GMT  
		Size: 1.4 MB (1361221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef98f5f03593c1f62a0e65ec140b18903bcf0ff8b40b28a45e3eaab92cd80652`  
		Last Modified: Wed, 20 Apr 2022 10:46:27 GMT  
		Size: 193.6 MB (193558199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dee14b8a1f0b2f450ca639f2d3d1cfed0177a474368d0b7f0713806e40090e7`  
		Last Modified: Thu, 21 Apr 2022 04:01:34 GMT  
		Size: 60.4 MB (60371844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8ab56b7cf813f2d7d7d921ecd6b1f8b7d313787d8f26dc508dbf0074963eca`  
		Last Modified: Thu, 21 Apr 2022 04:01:26 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09455a981bf5c04bd5ec564a9eb0a907c3b28872628a1fe857599eb83adc86a2`  
		Last Modified: Thu, 21 Apr 2022 04:01:26 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
