## `clojure:openjdk-18-tools-deps`

```console
$ docker pull clojure@sha256:0a359aeac17c66e58cb6cdf3dcf4d42c25c07d77f6a0b8d51e469bc34bec10f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-18-tools-deps` - linux; amd64

```console
$ docker pull clojure@sha256:56a56be1c5c8aeea56e3b256104baa0391b00e58901ee9cab76ad50b0d203e0e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.6 MB (256615007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1538e796898c85e10291d7c987883507a82910ebfdce945516312576bba7faa1`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 08:32:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:32:41 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Fri, 03 Sep 2021 08:32:42 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 08:32:42 GMT
ENV LANG=C.UTF-8
# Sat, 04 Sep 2021 09:42:51 GMT
ENV JAVA_VERSION=18-ea+13
# Sat, 04 Sep 2021 09:43:04 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/13/GPL/openjdk-18-ea+13_linux-x64_bin.tar.gz'; 			downloadSha256='396584ea555ad439176473f4e22c146817290a8eeaad02e3072dfb398ba786e0'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/13/GPL/openjdk-18-ea+13_linux-aarch64_bin.tar.gz'; 			downloadSha256='4601ee9811daa3bf282753e1fa6b8caffd869d0e56c9acfe95e1670bc580ed34'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 04 Sep 2021 09:43:05 GMT
CMD ["jshell"]
# Sat, 04 Sep 2021 10:05:18 GMT
ENV CLOJURE_VERSION=1.10.3.943
# Sat, 04 Sep 2021 10:05:18 GMT
WORKDIR /tmp
# Sat, 04 Sep 2021 10:05:34 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "f1fdb786fa8b9ef3a08d0b331a51861cd5a6eea277e93bbad64bf37774df17c6 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Sat, 04 Sep 2021 10:05:34 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb538b78785f115f86e312f41ac522a9b30e0cb77d061dd273f331e57ae2e471`  
		Last Modified: Fri, 03 Sep 2021 08:50:36 GMT  
		Size: 3.3 MB (3269611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33484bc42c97b072286bc3ad7418ceadb72c38d4cf944c0f5b3b91dd023ed6dc`  
		Last Modified: Sat, 04 Sep 2021 09:52:26 GMT  
		Size: 187.8 MB (187780325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be175ca10a54c9f7e2c752e026238dc5e83477ca5d0e30359b9c08b4f8d865cf`  
		Last Modified: Sat, 04 Sep 2021 10:17:14 GMT  
		Size: 38.4 MB (38419227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-18-tools-deps` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:11cbb7de6e352e576ff1b054d56ac80388d6176d83d0dcf4cfe93384a49b0fa6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.5 MB (253466487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56f676eaa59a75e0516e6bcae65e97268c90371f277bce2afb460e709b14eeff`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:58 GMT
ADD file:4a1d7f2d989aee6bd83da076b6e9dd3da2da97cf5654bd37568e9baec30ac4b1 in / 
# Fri, 03 Sep 2021 00:40:58 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 10:45:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 10:45:24 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Fri, 03 Sep 2021 10:45:24 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 10:45:24 GMT
ENV LANG=C.UTF-8
# Sat, 04 Sep 2021 01:48:52 GMT
ENV JAVA_VERSION=18-ea+13
# Sat, 04 Sep 2021 01:49:09 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/13/GPL/openjdk-18-ea+13_linux-x64_bin.tar.gz'; 			downloadSha256='396584ea555ad439176473f4e22c146817290a8eeaad02e3072dfb398ba786e0'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/13/GPL/openjdk-18-ea+13_linux-aarch64_bin.tar.gz'; 			downloadSha256='4601ee9811daa3bf282753e1fa6b8caffd869d0e56c9acfe95e1670bc580ed34'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 04 Sep 2021 01:49:10 GMT
CMD ["jshell"]
# Sat, 04 Sep 2021 02:20:00 GMT
ENV CLOJURE_VERSION=1.10.3.943
# Sat, 04 Sep 2021 02:20:01 GMT
WORKDIR /tmp
# Sat, 04 Sep 2021 02:20:17 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "f1fdb786fa8b9ef3a08d0b331a51861cd5a6eea277e93bbad64bf37774df17c6 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Sat, 04 Sep 2021 02:20:17 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:d10c227306ce3db344a8399cbc02bbf0dcb36519318efbde3c6027c00be8b40e`  
		Last Modified: Fri, 03 Sep 2021 00:49:47 GMT  
		Size: 25.9 MB (25914860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4152925219b6247cb64144905f215af10ba4621b4f699e896b93191fc575742`  
		Last Modified: Fri, 03 Sep 2021 11:06:36 GMT  
		Size: 3.1 MB (3119119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fb875a0b42ddc2ab4045c837a0adb20ffa21f4660056b204938225221f23b1`  
		Last Modified: Sat, 04 Sep 2021 02:05:24 GMT  
		Size: 186.5 MB (186519633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023711de79c66ee1a845404752b4a70617b07541f78812f20b8ba3e19c78d2fd`  
		Last Modified: Sat, 04 Sep 2021 02:32:56 GMT  
		Size: 37.9 MB (37912875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
