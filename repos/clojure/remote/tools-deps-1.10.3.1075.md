## `clojure:tools-deps-1.10.3.1075`

```console
$ docker pull clojure@sha256:56f3676f2f776ba9f6d17bccf0385614ce8dd9305176d06368b9e8b14a9b30e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:tools-deps-1.10.3.1075` - linux; amd64

```console
$ docker pull clojure@sha256:c8433cb7a224ee680f7513446d8e089a9e65f50f214cef7196312dd0e064c20e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.9 MB (280881213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fd1c21d37b63399be39877e8f16b8ebda12d0d1a487bad472f86b8ad3f56d71`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:35 GMT
ADD file:90495c24c897ec47982e200f732f8be3109fcd791691ddffae0756898f91024f in / 
# Wed, 26 Jan 2022 01:40:36 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 09:18:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:22:30 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Wed, 26 Jan 2022 09:22:30 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:22:30 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 09:22:31 GMT
ENV JAVA_VERSION=17.0.2
# Wed, 26 Jan 2022 09:22:58 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='0022753d0cceecacdd3a795dd4cea2bd7ffdf9dc06e22ffd1be98411742fbb44'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='13bfd976acf8803f862e82c7113fb0e9311ca5458b1decaef8a09ffd91119fa4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 26 Jan 2022 09:22:59 GMT
CMD ["jshell"]
# Fri, 04 Feb 2022 23:51:18 GMT
ENV CLOJURE_VERSION=1.10.3.1075
# Fri, 04 Feb 2022 23:51:19 GMT
WORKDIR /tmp
# Fri, 04 Feb 2022 23:51:36 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a6b72c9b23d348a0636813c5f59db5dda622e3b8dbb86124cbb51e3aced714d *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 04 Feb 2022 23:51:37 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 04 Feb 2022 23:51:37 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 04 Feb 2022 23:51:37 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 04 Feb 2022 23:51:38 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:5eb5b503b37671af16371272f9c5313a3e82f1d0756e14506704489ad9900803`  
		Last Modified: Wed, 26 Jan 2022 01:46:39 GMT  
		Size: 31.4 MB (31366257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc79ff7de66b9ef44dc6cd4f500aa92bd1f0b09ccd13eb0ee6441084fbb719cf`  
		Last Modified: Wed, 26 Jan 2022 09:41:32 GMT  
		Size: 1.6 MB (1582049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601a7753163a82e58164b68f17f35605d4e91cb610380e5cdc1e47d045bba5da`  
		Last Modified: Wed, 26 Jan 2022 09:48:21 GMT  
		Size: 187.9 MB (187900233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:887e37025ef86c29d12318ad6093c5c7deb9cfa60e7cc4445345fdfa457165e1`  
		Last Modified: Sat, 05 Feb 2022 01:42:20 GMT  
		Size: 60.0 MB (60031637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea5082d98e0fff774c606bf41575f1c4348386e11825427640f975f3a324c75d`  
		Last Modified: Sat, 05 Feb 2022 01:42:06 GMT  
		Size: 628.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91abd27e7844cbb73c0e3bceee0d8a07db19f1ccd1a28aee6e528c0504c31568`  
		Last Modified: Sat, 05 Feb 2022 01:42:06 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:tools-deps-1.10.3.1075` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:9cf1739cb0bed93eefca3a7d9d77d3c3af2732b03d4a2347eb8e1b9fab3d18f3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.1 MB (278106171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d0e5566808f5a031597fb75de9f138cb3b9d5e419417db1fa9c896dc00db3e3`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:49:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:54:28 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Wed, 26 Jan 2022 05:54:29 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 05:54:30 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 05:54:31 GMT
ENV JAVA_VERSION=17.0.2
# Wed, 26 Jan 2022 05:54:45 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='0022753d0cceecacdd3a795dd4cea2bd7ffdf9dc06e22ffd1be98411742fbb44'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='13bfd976acf8803f862e82c7113fb0e9311ca5458b1decaef8a09ffd91119fa4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 26 Jan 2022 05:54:45 GMT
CMD ["jshell"]
# Fri, 04 Feb 2022 21:48:12 GMT
ENV CLOJURE_VERSION=1.10.3.1075
# Fri, 04 Feb 2022 21:48:13 GMT
WORKDIR /tmp
# Fri, 04 Feb 2022 21:48:29 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a6b72c9b23d348a0636813c5f59db5dda622e3b8dbb86124cbb51e3aced714d *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 04 Feb 2022 21:48:30 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 04 Feb 2022 21:48:31 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 04 Feb 2022 21:48:31 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 04 Feb 2022 21:48:32 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abf67e3e34eccefabf68f15c7d753f1a4c8e241beb1818f97e276186d54124e`  
		Last Modified: Wed, 26 Jan 2022 06:13:02 GMT  
		Size: 1.6 MB (1565889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf423efb00f6c398e72a29f80e84cf999f7b9a81877dedb0e179db07c4daaa2`  
		Last Modified: Wed, 26 Jan 2022 06:20:25 GMT  
		Size: 186.5 MB (186527434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2827c71def4a5ade7a76ce5769889dfbbfe862db754bd1a14ab1b53f1e0b757`  
		Last Modified: Fri, 04 Feb 2022 22:00:40 GMT  
		Size: 60.0 MB (59955042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7995330b775917b12354a1567d81091a0f674d85496cb573126882f19b09812b`  
		Last Modified: Fri, 04 Feb 2022 22:00:31 GMT  
		Size: 625.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2d850419e9bc76aa0c1f93d1bc14138fe1c4e020f6099d37e519a95dd1f1331`  
		Last Modified: Fri, 04 Feb 2022 22:00:31 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
