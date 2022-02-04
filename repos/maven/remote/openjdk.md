## `maven:openjdk`

```console
$ docker pull maven@sha256:9949b7df3e4d6e2d0f73f0adfd4f3f39804e4ef84d4b0f41b7981405a3471445
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:openjdk` - linux; amd64

```console
$ docker pull maven@sha256:f0bb3c149471cf156862355adc8be7c6c4dd4ef59deba6bbcad53c8e37fb430b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **427.5 MB (427504501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07a2aa468c9dd18fdbadd0d27d8ff6c3413f2f3e20c876cdc526c37cd39897d0`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 04 Feb 2022 05:30:31 GMT
ADD file:17957b69b27e30b1d860c0919546da181b5e126b4aca4e1935ab44fd1832578e in / 
# Fri, 04 Feb 2022 05:30:31 GMT
CMD ["/bin/bash"]
# Fri, 04 Feb 2022 06:31:47 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 04 Feb 2022 06:32:56 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Fri, 04 Feb 2022 06:32:56 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Feb 2022 06:32:57 GMT
ENV LANG=C.UTF-8
# Fri, 04 Feb 2022 06:32:57 GMT
ENV JAVA_VERSION=17.0.2
# Fri, 04 Feb 2022 06:33:07 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='0022753d0cceecacdd3a795dd4cea2bd7ffdf9dc06e22ffd1be98411742fbb44'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='13bfd976acf8803f862e82c7113fb0e9311ca5458b1decaef8a09ffd91119fa4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 04 Feb 2022 06:33:08 GMT
CMD ["jshell"]
# Fri, 04 Feb 2022 09:06:06 GMT
ARG MAVEN_VERSION=3.8.4
# Fri, 04 Feb 2022 09:06:07 GMT
ARG USER_HOME_DIR=/root
# Fri, 04 Feb 2022 09:06:07 GMT
ARG SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8
# Fri, 04 Feb 2022 09:06:07 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries
# Fri, 04 Feb 2022 09:06:36 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN microdnf install findutils git
# Fri, 04 Feb 2022 09:06:46 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 04 Feb 2022 09:06:46 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 04 Feb 2022 09:06:46 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 04 Feb 2022 09:06:46 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 04 Feb 2022 09:06:47 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 04 Feb 2022 09:06:47 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 04 Feb 2022 09:06:47 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:f431a76c5f59c48efd4a4076677acaae2b540a7562de00075162ef8a340fd69b`  
		Last Modified: Fri, 04 Feb 2022 05:31:30 GMT  
		Size: 42.1 MB (42102405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a0509e57e85d3b85eac03c20f8f88d1cb2481d6122bdae0020851f7022e3b31`  
		Last Modified: Fri, 04 Feb 2022 08:22:45 GMT  
		Size: 13.5 MB (13513973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99183953ac5d5bafa925c1b03d239d433576f5dc1cae53fee20bc6c37d09568e`  
		Last Modified: Fri, 04 Feb 2022 08:24:05 GMT  
		Size: 187.5 MB (187527734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585acf03578a70e3eaf78fe46619b8e5559bb5f8128ff094da4e334a47c34352`  
		Last Modified: Fri, 04 Feb 2022 09:09:10 GMT  
		Size: 175.2 MB (175249360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85bd88906eabd7f75d468e70fe66c65bca6d19baf5dfbe5b0d44b9df5a109a2`  
		Last Modified: Fri, 04 Feb 2022 09:08:57 GMT  
		Size: 9.1 MB (9109809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6460e9eedcee6bc8e85069b1334527dd1bd7c83ebf7d7f03c361a51ec239569`  
		Last Modified: Fri, 04 Feb 2022 09:08:56 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fce482a6e9b1bed1f111af1c53d428b01ef4fb2350d41997a5cb89d4002c9bb`  
		Last Modified: Fri, 04 Feb 2022 09:08:56 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:openjdk` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:984d291beef497c84caec5a424f13e42dfcd4be297f0d5f0ff4110b16e107abb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **417.6 MB (417609035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfc6c3f99243088b1b6ee6261c8be1e2dbd0e994a8cb9ee52884285f743085b1`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 04 Feb 2022 04:13:53 GMT
ADD file:22ac13d97f9f75668fec05f2cf9d182e5edcf2822b08ef38929b0bb8d61f5edb in / 
# Fri, 04 Feb 2022 04:13:54 GMT
CMD ["/bin/bash"]
# Fri, 04 Feb 2022 05:34:11 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 04 Feb 2022 05:38:14 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Fri, 04 Feb 2022 05:38:14 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Feb 2022 05:38:15 GMT
ENV LANG=C.UTF-8
# Fri, 04 Feb 2022 05:38:16 GMT
ENV JAVA_VERSION=17.0.2
# Fri, 04 Feb 2022 05:38:27 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='0022753d0cceecacdd3a795dd4cea2bd7ffdf9dc06e22ffd1be98411742fbb44'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='13bfd976acf8803f862e82c7113fb0e9311ca5458b1decaef8a09ffd91119fa4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 04 Feb 2022 05:38:28 GMT
CMD ["jshell"]
# Fri, 04 Feb 2022 06:31:09 GMT
ARG MAVEN_VERSION=3.8.4
# Fri, 04 Feb 2022 06:31:09 GMT
ARG USER_HOME_DIR=/root
# Fri, 04 Feb 2022 06:31:10 GMT
ARG SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8
# Fri, 04 Feb 2022 06:31:11 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries
# Fri, 04 Feb 2022 06:32:09 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN microdnf install findutils git
# Fri, 04 Feb 2022 06:32:24 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 04 Feb 2022 06:32:24 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 04 Feb 2022 06:32:25 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 04 Feb 2022 06:32:27 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 04 Feb 2022 06:32:28 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 04 Feb 2022 06:32:28 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 04 Feb 2022 06:32:29 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:200ed4b56d545919e183ba8dfa2493452065262be1759dd78c3de721a71882cb`  
		Last Modified: Fri, 04 Feb 2022 04:14:59 GMT  
		Size: 42.0 MB (42011648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4545cbf19e4d384cf8f28f10cdb2cb3e0cfb6a09f47542c1c092358c7fd1b5`  
		Last Modified: Fri, 04 Feb 2022 05:50:37 GMT  
		Size: 14.3 MB (14290526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c52ee4a32a999688ddd79222e497c2226d984006f6ec5b3bdc773ef75e033e7`  
		Last Modified: Fri, 04 Feb 2022 05:52:14 GMT  
		Size: 186.4 MB (186364048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3b5c4666629d6529892827b1953536a0b7675ffd185db1aac82d63bd7c9b59`  
		Last Modified: Fri, 04 Feb 2022 06:36:01 GMT  
		Size: 165.8 MB (165831820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31854bd0b628632995392e3ca014821338738e06c36629d7cff9d85fe07ab9f8`  
		Last Modified: Fri, 04 Feb 2022 06:35:45 GMT  
		Size: 9.1 MB (9109775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c973e7b8d97ddaa68d294a0bae7dd14e53702cccc7dbc96aca80e4e815c3e766`  
		Last Modified: Fri, 04 Feb 2022 06:35:44 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61078f0389fab702c8eea03958cdc3153fecf06880eedc468f8e68c9dd47b13e`  
		Last Modified: Fri, 04 Feb 2022 06:35:44 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
