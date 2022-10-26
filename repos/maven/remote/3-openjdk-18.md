## `maven:3-openjdk-18`

```console
$ docker pull maven@sha256:e880c26bd935086b3fbf1ac9e836322d0448e23dbd9ef556aaee12ba3c91ae6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-openjdk-18` - linux; amd64

```console
$ docker pull maven@sha256:6e7387ff8daab9124e86f187ae349b31144fc6e2b698afbef53431753bfb4283
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **443.5 MB (443466217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78780cd3365089d24e7269910767b69d5141df688a220baaeb618fcba2e0bf8a`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 21 Oct 2022 19:20:54 GMT
ADD file:66ffe38a497f15c1941fcc4c64fda875cf27856f2ade5128546c10590c5ca84a in / 
# Fri, 21 Oct 2022 19:20:54 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 19:51:29 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 21 Oct 2022 19:52:32 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Fri, 21 Oct 2022 19:52:32 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Oct 2022 19:52:32 GMT
ENV LANG=C.UTF-8
# Fri, 21 Oct 2022 19:52:32 GMT
ENV JAVA_VERSION=18.0.2.1
# Fri, 21 Oct 2022 19:52:42 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_linux-x64_bin.tar.gz'; 			downloadSha256='3bfdb59fc38884672677cebca9a216902d87fe867563182ae8bc3373a65a2ebd'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='79900237a5912045f8c9f1065b5204a474803cbbb4d075ab9620650fb75dfc1b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 21 Oct 2022 19:52:43 GMT
CMD ["jshell"]
# Fri, 21 Oct 2022 20:15:18 GMT
RUN microdnf install findutils git
# Fri, 21 Oct 2022 20:15:19 GMT
ARG MAVEN_VERSION=3.8.6
# Fri, 21 Oct 2022 20:15:19 GMT
ARG USER_HOME_DIR=/root
# Fri, 21 Oct 2022 20:15:19 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Fri, 21 Oct 2022 20:15:19 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Fri, 21 Oct 2022 20:15:26 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 21 Oct 2022 20:15:26 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 21 Oct 2022 20:15:26 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 21 Oct 2022 20:15:26 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 21 Oct 2022 20:15:26 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 21 Oct 2022 20:15:26 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 21 Oct 2022 20:15:26 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:50cbc88660a5576a306374b5ee70e3e8aeb602409e05ffa41cd4680769ae0574`  
		Last Modified: Fri, 21 Oct 2022 19:22:39 GMT  
		Size: 40.6 MB (40588747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f15da7b20d89dec72e0bff2c38edc4d7119a8f5049343764ac32b207f7bd7b9`  
		Last Modified: Fri, 21 Oct 2022 19:55:16 GMT  
		Size: 12.2 MB (12231175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812b9f471c4d3fc2f4cbb321294c1ba3ff80d3fdcca1e2d2caac573ca335fdca`  
		Last Modified: Fri, 21 Oct 2022 19:57:07 GMT  
		Size: 188.7 MB (188744692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482f442c6a52a1c153ee5f9a7898cfa23ab4c47da5bb9e68574474f4c5a6cee7`  
		Last Modified: Fri, 21 Oct 2022 20:17:57 GMT  
		Size: 193.2 MB (193160887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6821bb033912063f6893bc14ce6583596e3105679e2f4b527d3095c1892d8a90`  
		Last Modified: Fri, 21 Oct 2022 20:17:43 GMT  
		Size: 8.7 MB (8739500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f358cb8a3bde1a4b3ef658fcac98732ab4cd49b4d7a7600643dce013cc0fc08`  
		Last Modified: Fri, 21 Oct 2022 20:17:42 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2c41250f1c72335e5c101151247284e1dd72bf9aa09492161a6223718931e0`  
		Last Modified: Fri, 21 Oct 2022 20:17:42 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-openjdk-18` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:4bee7361d4a462766cd7b2abc9ed95b6ab19c121d19e3ec95111b4211957a3fb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **454.7 MB (454693118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c452c4a53d555f9ea9f803787fa49a7fa607194b2103f137254a8949e11a20c2`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 21 Oct 2022 19:41:03 GMT
ADD file:2ccafa0c5b388d404f1100108ad9a9cb06c3e4ca4543c4b0f2aadfd9c4b97e45 in / 
# Fri, 21 Oct 2022 19:41:03 GMT
CMD ["/bin/bash"]
# Wed, 26 Oct 2022 00:43:34 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 26 Oct 2022 00:46:00 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Wed, 26 Oct 2022 00:46:00 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 00:46:00 GMT
ENV LANG=C.UTF-8
# Wed, 26 Oct 2022 00:46:00 GMT
ENV JAVA_VERSION=18.0.2.1
# Wed, 26 Oct 2022 00:46:08 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_linux-x64_bin.tar.gz'; 			downloadSha256='3bfdb59fc38884672677cebca9a216902d87fe867563182ae8bc3373a65a2ebd'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='79900237a5912045f8c9f1065b5204a474803cbbb4d075ab9620650fb75dfc1b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 26 Oct 2022 00:46:09 GMT
CMD ["jshell"]
# Wed, 26 Oct 2022 15:15:52 GMT
RUN microdnf install findutils git
# Wed, 26 Oct 2022 15:15:55 GMT
ARG MAVEN_VERSION=3.8.6
# Wed, 26 Oct 2022 15:15:55 GMT
ARG USER_HOME_DIR=/root
# Wed, 26 Oct 2022 15:15:55 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Wed, 26 Oct 2022 15:15:55 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Wed, 26 Oct 2022 15:16:01 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 26 Oct 2022 15:16:01 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 26 Oct 2022 15:16:01 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 26 Oct 2022 15:16:01 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 26 Oct 2022 15:16:01 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 26 Oct 2022 15:16:01 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 26 Oct 2022 15:16:01 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:ba2bcb842ee086f4d448ac74f4e172e2568d56d24e6efae9b402c0e37f418943`  
		Last Modified: Fri, 21 Oct 2022 19:42:50 GMT  
		Size: 39.4 MB (39408151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e435e89e01609b5f7794b35f7cd9ecdea4fd71ca761c724e6d77a2911953776`  
		Last Modified: Wed, 26 Oct 2022 00:49:53 GMT  
		Size: 13.1 MB (13059774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7f91ff024b6704a5d8f9084a9648f7a4e11beb8c2dc4596fa329d1f9c608de`  
		Last Modified: Wed, 26 Oct 2022 00:53:43 GMT  
		Size: 187.7 MB (187659416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670b7777f178262627a57550a4d8111eae408f53b51d3510f815a96e87419bae`  
		Last Modified: Wed, 26 Oct 2022 15:22:15 GMT  
		Size: 205.8 MB (205825047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a006579b4649bf7232fef70b78c732bb94f75f83e5be39ad318467f634c0e81a`  
		Last Modified: Wed, 26 Oct 2022 15:22:03 GMT  
		Size: 8.7 MB (8739512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c23aa79bf61908404882bb5654b2f5161134d5d0d69c92e5dd8bb9976d2e138c`  
		Last Modified: Wed, 26 Oct 2022 15:22:02 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d7054a49a34de79e30833de8066cdf07f7f7fcd0df60ec5ce89de39b4c8c7e`  
		Last Modified: Wed, 26 Oct 2022 15:22:02 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
