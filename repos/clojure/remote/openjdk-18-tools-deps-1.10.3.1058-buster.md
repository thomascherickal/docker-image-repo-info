## `clojure:openjdk-18-tools-deps-1.10.3.1058-buster`

```console
$ docker pull clojure@sha256:0addffbc61804802713c0ac7e66c58f4e01f7d5023b85df9e5f3d687df832984
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-18-tools-deps-1.10.3.1058-buster` - linux; amd64

```console
$ docker pull clojure@sha256:5e2a3e7f644b36c702fecc76e2170cdfb9db57d604d5ab98c54adcefad94a7ea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.5 MB (353536929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b45d070904d558f52759cd06d38ec377886e8394d467588a61624b41412f8879`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:53 GMT
ADD file:be998d04a8927e9c4b105995e3b9d6800ea798807389f7c5921c0f4774328e21 in / 
# Tue, 21 Dec 2021 01:22:53 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:53:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:53:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 01:53:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 22:58:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 22:59:42 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Tue, 21 Dec 2021 22:59:42 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 22:59:42 GMT
ENV LANG=C.UTF-8
# Mon, 27 Dec 2021 18:54:23 GMT
ENV JAVA_VERSION=18-ea+29
# Mon, 27 Dec 2021 18:54:34 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/29/GPL/openjdk-18-ea+29_linux-x64_bin.tar.gz'; 			downloadSha256='79501105196281bcb3b1c356529238c3f943a51a24e8695bcee0e3b3e1881507'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/29/GPL/openjdk-18-ea+29_linux-aarch64_bin.tar.gz'; 			downloadSha256='cecaad040cc1f7b0507c8b62275e90ddc32a203da239dccfd5d711f47518bc3c'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 27 Dec 2021 18:54:35 GMT
CMD ["jshell"]
# Fri, 07 Jan 2022 20:23:20 GMT
ENV CLOJURE_VERSION=1.10.3.1058
# Fri, 07 Jan 2022 20:23:20 GMT
WORKDIR /tmp
# Fri, 07 Jan 2022 20:23:31 GMT
RUN apt-get update && apt-get install -y make rlwrap && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "980168025a3827bd7ed9d5ab1681ce29808ac8e6cbced3ab6683db8b365b54df *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)"
# Fri, 07 Jan 2022 20:23:31 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 07 Jan 2022 20:23:32 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 07 Jan 2022 20:23:32 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 07 Jan 2022 20:23:32 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:9b99af5931b39ce167150ad668cfa57ddf7664697be9996cb7e0e6aebbf05843`  
		Last Modified: Tue, 21 Dec 2021 01:28:07 GMT  
		Size: 50.4 MB (50437136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6013b3e77fe6fd3dcf46a05f8e5b3afa9fbca7ba0161c62e56beb4058334dec`  
		Last Modified: Tue, 21 Dec 2021 02:02:46 GMT  
		Size: 7.8 MB (7833863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbced17b6899896c8e4016d62c885d737fe667acace2733e17c64bb974232887`  
		Last Modified: Tue, 21 Dec 2021 02:02:46 GMT  
		Size: 10.0 MB (9997172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b609dabefa83fae157bcd42123a8ed45199bb6c301e09a11260c1cad9babfef`  
		Last Modified: Tue, 21 Dec 2021 02:03:05 GMT  
		Size: 51.8 MB (51841352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdedc4ba2f5e3c8c742aac0efd5bf20b6ff7b5777dcb5308ff111a3e4396d984`  
		Last Modified: Tue, 21 Dec 2021 23:15:30 GMT  
		Size: 13.9 MB (13921199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546fbb2fb42584e61764836d9013c251e07fe06a0c61a71ad4749d5af77414b9`  
		Last Modified: Mon, 27 Dec 2021 19:07:01 GMT  
		Size: 188.7 MB (188744928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598694e85c0fe56bd8dc9b24d69d4da1e540cb01cce666802755cc79e2f03a76`  
		Last Modified: Fri, 07 Jan 2022 20:32:16 GMT  
		Size: 30.8 MB (30760248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddfc68248f3cef3bc38d42935524604172d3e77779335ec4ff3cd148bc449c0`  
		Last Modified: Fri, 07 Jan 2022 20:32:13 GMT  
		Size: 624.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad43ac82909414dfa39afcfee3122350efcd4e3d116f6bae475115df15f44e61`  
		Last Modified: Fri, 07 Jan 2022 20:32:13 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-18-tools-deps-1.10.3.1058-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:6b6ea81af5922ceaa1aff46262c47dc20364a374fec69be80c03281c4970427f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.3 MB (351316649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5b19b78b6a9e7a52d77599f3697842eddf072dc5a906b3404ee251e06add240`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:34 GMT
ADD file:73bd5e773b257a6ea5d29845b2b112ebce468878a9467e7c0fe61c69994bb47f in / 
# Tue, 21 Dec 2021 01:42:35 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:13:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:13:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:14:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:54:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:56:18 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Tue, 21 Dec 2021 02:56:19 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 02:56:20 GMT
ENV LANG=C.UTF-8
# Mon, 27 Dec 2021 17:47:44 GMT
ENV JAVA_VERSION=18-ea+29
# Mon, 27 Dec 2021 17:48:02 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/29/GPL/openjdk-18-ea+29_linux-x64_bin.tar.gz'; 			downloadSha256='79501105196281bcb3b1c356529238c3f943a51a24e8695bcee0e3b3e1881507'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/29/GPL/openjdk-18-ea+29_linux-aarch64_bin.tar.gz'; 			downloadSha256='cecaad040cc1f7b0507c8b62275e90ddc32a203da239dccfd5d711f47518bc3c'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 27 Dec 2021 17:48:02 GMT
CMD ["jshell"]
# Fri, 07 Jan 2022 20:44:42 GMT
ENV CLOJURE_VERSION=1.10.3.1058
# Fri, 07 Jan 2022 20:44:43 GMT
WORKDIR /tmp
# Fri, 07 Jan 2022 20:44:55 GMT
RUN apt-get update && apt-get install -y make rlwrap && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "980168025a3827bd7ed9d5ab1681ce29808ac8e6cbced3ab6683db8b365b54df *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)"
# Fri, 07 Jan 2022 20:44:56 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 07 Jan 2022 20:44:57 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 07 Jan 2022 20:44:57 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 07 Jan 2022 20:44:58 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:741eb94195433e00f9799629cc66740c97d607d6f3ed207e5738995897c52959`  
		Last Modified: Tue, 21 Dec 2021 01:49:16 GMT  
		Size: 49.2 MB (49223144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d098cf33298807975a4d84f59f6689e0bf729b62fca9b7320adb80ebeaabc578`  
		Last Modified: Tue, 21 Dec 2021 02:23:45 GMT  
		Size: 7.7 MB (7695163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0317c7db28bd6855b787608d1f4236185907b452f6f545a9954be870828af6`  
		Last Modified: Tue, 21 Dec 2021 02:23:45 GMT  
		Size: 9.8 MB (9767165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4301bfae0dab5df877b31fde90c919b02335f783b7405d66b6123acfe03e69e`  
		Last Modified: Tue, 21 Dec 2021 02:24:05 GMT  
		Size: 52.2 MB (52168887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c1cf4e1d86834082c63f5bd67efeec8dccd801ae671f9bce3cdf6f178be4a9`  
		Last Modified: Tue, 21 Dec 2021 03:17:02 GMT  
		Size: 14.7 MB (14671031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8510fbaa2e9131074dd71f2902aa054553b35aec0fb1037b8011281cb2ae63`  
		Last Modified: Mon, 27 Dec 2021 18:07:29 GMT  
		Size: 187.7 MB (187690696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d55d38de545745240f18760c2953025ebb60d9991fd734e4ff692b2b49dea53`  
		Last Modified: Fri, 07 Jan 2022 20:57:49 GMT  
		Size: 30.1 MB (30099530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707ec59c8b3f1abc7f2b9d883665c596d8796de99b617af4b6faf41f5c2e68f5`  
		Last Modified: Fri, 07 Jan 2022 20:57:46 GMT  
		Size: 626.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d431bf5ec0d6896329e9f84aaa8213f9011a40d2e8f2360f4e0d5ce4823db288`  
		Last Modified: Fri, 07 Jan 2022 20:57:46 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
