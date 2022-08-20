## `maven:3-openjdk-18`

```console
$ docker pull maven@sha256:f6b5e720fa4c595b39a3b354496909b880a7c08cd2f81e6081060c440cfef2c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-openjdk-18` - linux; amd64

```console
$ docker pull maven@sha256:e68c38a0e60a0c7bd851da703c0d5b156f700c1bed9943845a30c570e7079d96
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **439.7 MB (439693793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a306d56e69114089c48a53c1e5422c5f5320008b14514eea63f2927d1996348a`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 04 Aug 2022 00:36:37 GMT
ADD file:0a05a213ae66f556b2b320291ac58ec9f2f67554e29338a072f1347f22864a49 in / 
# Thu, 04 Aug 2022 00:36:37 GMT
CMD ["/bin/bash"]
# Thu, 04 Aug 2022 01:35:27 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 04 Aug 2022 01:36:33 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Thu, 04 Aug 2022 01:36:33 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 Aug 2022 01:36:34 GMT
ENV LANG=C.UTF-8
# Sat, 20 Aug 2022 01:33:04 GMT
ENV JAVA_VERSION=18.0.2.1
# Sat, 20 Aug 2022 01:33:14 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_linux-x64_bin.tar.gz'; 			downloadSha256='3bfdb59fc38884672677cebca9a216902d87fe867563182ae8bc3373a65a2ebd'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='79900237a5912045f8c9f1065b5204a474803cbbb4d075ab9620650fb75dfc1b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 20 Aug 2022 01:33:15 GMT
CMD ["jshell"]
# Sat, 20 Aug 2022 02:05:45 GMT
RUN microdnf install findutils git
# Sat, 20 Aug 2022 02:05:46 GMT
ARG MAVEN_VERSION=3.8.6
# Sat, 20 Aug 2022 02:05:46 GMT
ARG USER_HOME_DIR=/root
# Sat, 20 Aug 2022 02:05:46 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Sat, 20 Aug 2022 02:05:46 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Sat, 20 Aug 2022 02:05:49 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Sat, 20 Aug 2022 02:05:49 GMT
ENV MAVEN_HOME=/usr/share/maven
# Sat, 20 Aug 2022 02:05:49 GMT
ENV MAVEN_CONFIG=/root/.m2
# Sat, 20 Aug 2022 02:05:50 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Sat, 20 Aug 2022 02:05:50 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Sat, 20 Aug 2022 02:05:50 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Sat, 20 Aug 2022 02:05:50 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:32c1bf40aba1f372a057d3280b0b7cdacde9d8500a069004e6f243bc09cde806`  
		Last Modified: Thu, 04 Aug 2022 00:37:33 GMT  
		Size: 39.2 MB (39223952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d72ac1fb23a36f89addf60367990f28d5c0882e4b8f569c77b51c51eb271261`  
		Last Modified: Thu, 04 Aug 2022 01:42:41 GMT  
		Size: 13.5 MB (13506500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c951706478088e69abce7bf812ce1b19c0a043776d88b1ab36b045d376445715`  
		Last Modified: Sat, 20 Aug 2022 01:44:26 GMT  
		Size: 188.7 MB (188744910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac8d2d65d9f98c4069842d5b889aefe7c48db713e96a979a83cd20fb80551ba8`  
		Last Modified: Sat, 20 Aug 2022 02:08:53 GMT  
		Size: 189.5 MB (189477737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b0f771d115c2f1127abb5f45e2b3f46a414f428be75297d5c8d005de85e0a7`  
		Last Modified: Sat, 20 Aug 2022 02:08:38 GMT  
		Size: 8.7 MB (8739479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be872bb8aacf3b7fd1dee69015bf40d6e6762db290d15eed3baf9830417c259`  
		Last Modified: Sat, 20 Aug 2022 02:08:38 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3f912b4dd19b3c48c742eb0fbd9819de899d8a126f66f93d7df4c1b361fad4`  
		Last Modified: Sat, 20 Aug 2022 02:08:37 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-openjdk-18` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:fee563bc8f62f49a0906afec536e332919779aea6124da90ea4dbee25d171e65
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **444.1 MB (444091617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bd047c297a11d49298aae030aff7bb83b83dd2b712a124729f891c100aeed56`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 04 Aug 2022 00:40:43 GMT
ADD file:a68d82fa032efe6adc2926f7e745508f0541bba3f906e2702d34252353100747 in / 
# Thu, 04 Aug 2022 00:40:44 GMT
CMD ["/bin/bash"]
# Thu, 04 Aug 2022 01:01:11 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 04 Aug 2022 01:03:11 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Thu, 04 Aug 2022 01:03:12 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 Aug 2022 01:03:13 GMT
ENV LANG=C.UTF-8
# Thu, 04 Aug 2022 01:03:14 GMT
ENV JAVA_VERSION=18.0.2
# Thu, 04 Aug 2022 01:03:25 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2/f6ad4b4450fd4d298113270ec84f30ee/9/GPL/openjdk-18.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='cf06f41a3952038df0550e8cbc2baf0aa877c3ba00cca0dd26f73134f8baf0e6'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2/f6ad4b4450fd4d298113270ec84f30ee/9/GPL/openjdk-18.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='99d994dab3c5ad0e87a3d72dc3be33d5b2f045f0ddda0cb7853dfbf6b5d5d3b0'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 04 Aug 2022 01:03:25 GMT
CMD ["jshell"]
# Thu, 04 Aug 2022 02:46:07 GMT
RUN microdnf install findutils git
# Thu, 04 Aug 2022 02:46:08 GMT
ARG MAVEN_VERSION=3.8.6
# Thu, 04 Aug 2022 02:46:08 GMT
ARG USER_HOME_DIR=/root
# Thu, 04 Aug 2022 02:46:09 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Thu, 04 Aug 2022 02:46:10 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Thu, 04 Aug 2022 02:46:13 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 04 Aug 2022 02:46:14 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 04 Aug 2022 02:46:15 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 04 Aug 2022 02:46:17 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 04 Aug 2022 02:46:18 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 04 Aug 2022 02:46:18 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 04 Aug 2022 02:46:19 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:ecf56004177eb6ca162c88de29e84bc4ba3d2e7efd3703df9ecae51b89003d52`  
		Last Modified: Thu, 04 Aug 2022 00:41:51 GMT  
		Size: 38.0 MB (38023046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e225b6ab834ff85ee0d347a2859ecb14fc169f362360408133589ab8a37d8333`  
		Last Modified: Thu, 04 Aug 2022 01:14:59 GMT  
		Size: 14.3 MB (14278746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ec648e0a6b9193d2b24914cf240a683985a431f3b66d01e7f3032c3c1b92ff`  
		Last Modified: Thu, 04 Aug 2022 01:18:05 GMT  
		Size: 187.7 MB (187664272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9614888b8475b0aa9f5210dd4c0bdbf6aed473310f844104a35e58c3b472b895`  
		Last Modified: Thu, 04 Aug 2022 02:50:25 GMT  
		Size: 195.4 MB (195384855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d288eebd24c8854affc8729651c27990d1239d09119d3bd31110616040d31b6e`  
		Last Modified: Thu, 04 Aug 2022 02:50:06 GMT  
		Size: 8.7 MB (8739481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16738b96ad971da2f71e9b475004700f2851d488aa3847149eb6c018c80229e`  
		Last Modified: Thu, 04 Aug 2022 02:50:05 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a2a6f6d9116530ed3ca678fee8f45cd17e49c81fe840e3d43a9f28fbbc8155`  
		Last Modified: Thu, 04 Aug 2022 02:50:05 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
