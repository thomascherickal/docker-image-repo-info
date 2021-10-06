## `maven:3-openjdk-16`

```console
$ docker pull maven@sha256:9a1c0c95f96534e2c5dbc320b4e55d19115f8132e85b055327da66276d0b1a6e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-openjdk-16` - linux; amd64

```console
$ docker pull maven@sha256:c074f22968a662b2fc87c12f387026edd5a536d31cc54c5bcf055516b56dedc9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **408.8 MB (408833037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61e916a4ae2d96fe3520478034d0f6d42aee9d27dae51060d735efb1963116dc`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 29 Sep 2021 16:28:05 GMT
ADD file:99c665dc5bddb30b592aa86f66d1256f41b468201a93afe0c6164edb42c388c4 in / 
# Wed, 29 Sep 2021 16:28:06 GMT
CMD ["/bin/bash"]
# Wed, 29 Sep 2021 16:53:34 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 29 Sep 2021 16:55:41 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Wed, 29 Sep 2021 16:55:41 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 16:55:41 GMT
ENV LANG=C.UTF-8
# Wed, 29 Sep 2021 16:55:41 GMT
ENV JAVA_VERSION=16.0.2
# Wed, 29 Sep 2021 16:55:52 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='6c714ded7d881ca54970ec949e283f43d673a142fda1de79b646ddd619da9c0c'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='1ffb9c7748334945d9056b3324de3f797d906fce4dad86beea955153aa1e28fe'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 29 Sep 2021 16:55:52 GMT
CMD ["jshell"]
# Wed, 06 Oct 2021 21:09:56 GMT
ARG MAVEN_VERSION=3.8.3
# Wed, 06 Oct 2021 21:09:56 GMT
ARG USER_HOME_DIR=/root
# Wed, 06 Oct 2021 21:09:56 GMT
ARG SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa
# Wed, 06 Oct 2021 21:09:56 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries
# Wed, 06 Oct 2021 21:10:23 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries MAVEN_VERSION=3.8.3 SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa USER_HOME_DIR=/root
RUN microdnf install findutils git
# Wed, 06 Oct 2021 21:10:32 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries MAVEN_VERSION=3.8.3 SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 06 Oct 2021 21:10:32 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 06 Oct 2021 21:10:32 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 06 Oct 2021 21:10:33 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 06 Oct 2021 21:10:33 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 06 Oct 2021 21:10:33 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 06 Oct 2021 21:10:33 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:6540cb32758bf3f150d56508f216b26487b14ac6fd20b1c92f1e1c8357730ea9`  
		Last Modified: Wed, 29 Sep 2021 16:29:48 GMT  
		Size: 42.0 MB (41963002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3acb1bb05d773c14486a356ac78716bf3e9e5b34aefb39b421cc776aea66e606`  
		Last Modified: Wed, 29 Sep 2021 17:02:29 GMT  
		Size: 13.5 MB (13490694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42588ce1c6735812e5a3cc3788e53770bfdde7d2027f1537b74304063f1a37e2`  
		Last Modified: Wed, 29 Sep 2021 17:05:41 GMT  
		Size: 184.8 MB (184807186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3a7981572164e5f3d0272236756e2d52fb3fdd83a15ca77a77a1ee77e29baf`  
		Last Modified: Wed, 06 Oct 2021 21:21:24 GMT  
		Size: 159.5 MB (159465287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02eda70ea5c88b8ace301c8e2df45305f533f9684d365a75a3a8d4a3ab40d0a6`  
		Last Modified: Wed, 06 Oct 2021 21:21:11 GMT  
		Size: 9.1 MB (9105645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b216d910c18efae743b249b209294b73e2abba7bceb6acb6baea8e6c3155e5c9`  
		Last Modified: Wed, 06 Oct 2021 21:21:10 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d2779bd0546f2f7e28e805d76716ba5a0a4035466209b634360ef3c7ef2135`  
		Last Modified: Wed, 06 Oct 2021 21:21:10 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-openjdk-16` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:d03855b907be7e06865450e83204e0b85667fc6d6c501b58eee4558931d6f392
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **390.1 MB (390091199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d749c35cfbcb1b658895a1513257f44c97991424c96bb989c2498c3bf41072d3`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 29 Sep 2021 09:28:21 GMT
ADD file:19a29c4f8accf14e581617044399a0a04fbdf31b2a3dd531b59c72d011deea65 in / 
# Wed, 29 Sep 2021 09:28:21 GMT
CMD ["/bin/bash"]
# Wed, 29 Sep 2021 10:13:29 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 29 Sep 2021 10:16:42 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Wed, 29 Sep 2021 10:16:42 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 10:16:42 GMT
ENV LANG=C.UTF-8
# Wed, 29 Sep 2021 10:16:43 GMT
ENV JAVA_VERSION=16.0.2
# Wed, 29 Sep 2021 10:16:51 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='6c714ded7d881ca54970ec949e283f43d673a142fda1de79b646ddd619da9c0c'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='1ffb9c7748334945d9056b3324de3f797d906fce4dad86beea955153aa1e28fe'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 29 Sep 2021 10:16:52 GMT
CMD ["jshell"]
# Wed, 06 Oct 2021 21:17:03 GMT
ARG MAVEN_VERSION=3.8.3
# Wed, 06 Oct 2021 21:17:03 GMT
ARG USER_HOME_DIR=/root
# Wed, 06 Oct 2021 21:17:03 GMT
ARG SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa
# Wed, 06 Oct 2021 21:17:03 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries
# Wed, 06 Oct 2021 21:17:27 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries MAVEN_VERSION=3.8.3 SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa USER_HOME_DIR=/root
RUN microdnf install findutils git
# Wed, 06 Oct 2021 21:17:36 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries MAVEN_VERSION=3.8.3 SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 06 Oct 2021 21:17:36 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 06 Oct 2021 21:17:36 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 06 Oct 2021 21:17:37 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 06 Oct 2021 21:17:37 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 06 Oct 2021 21:17:37 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 06 Oct 2021 21:17:37 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:fbe1b66208e55e97b0e90b882e6fdeed78abb9318897a2d87343840b78e723ef`  
		Last Modified: Wed, 29 Sep 2021 09:29:46 GMT  
		Size: 41.9 MB (41883345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8fe2b96b9211b7b369c53846fe42fa00426fa23a6d736fb50873c69ffc8b3c9`  
		Last Modified: Wed, 29 Sep 2021 10:29:47 GMT  
		Size: 14.3 MB (14275215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f32d2c117014198642e9c4d4a5422a7380260c883f4b1fa52584899eb8fa57c`  
		Last Modified: Wed, 29 Sep 2021 10:33:45 GMT  
		Size: 179.2 MB (179188965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31954afb683e98bf4c9498849093570184c7c5f818982e2edb066e67826a6ad`  
		Last Modified: Wed, 06 Oct 2021 21:28:52 GMT  
		Size: 145.6 MB (145636811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3de8d936e7217703b00e0805b60ec4733b181a13cac8e38a4d5823f177c53c`  
		Last Modified: Wed, 06 Oct 2021 21:28:37 GMT  
		Size: 9.1 MB (9105646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb8f838191e512ce8effb8ce7f5894fe5546c68a51924261b763c1dbe524609e`  
		Last Modified: Wed, 06 Oct 2021 21:28:36 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c046d1d7b295fcf674b4cae206e82bb7b2421217bf97d6317df87d216f981448`  
		Last Modified: Wed, 06 Oct 2021 21:28:36 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
