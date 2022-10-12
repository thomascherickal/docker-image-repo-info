## `maven:3-openjdk-18`

```console
$ docker pull maven@sha256:4464fc772e53fba05bd754a31dfe5b4f9509953a1ad441b155fb3c356d1de542
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-openjdk-18` - linux; amd64

```console
$ docker pull maven@sha256:46d8f3924cdf2c369d8963c594259c4ae2da93c9199fe0a8c83e9c71c30832d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **442.9 MB (442915685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fd033d671127b2213c3846ba7de384af8788e7d7414bfd609c0bfdb8c730245`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 12 Oct 2022 21:20:42 GMT
ADD file:ceac4c0bc6dd71b3868d5af15bdaab832a2f61b45c12116b2df42ef8cfbf9fa1 in / 
# Wed, 12 Oct 2022 21:20:42 GMT
CMD ["/bin/bash"]
# Wed, 12 Oct 2022 21:40:55 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 12 Oct 2022 21:41:25 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Wed, 12 Oct 2022 21:41:25 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Oct 2022 21:41:25 GMT
ENV LANG=C.UTF-8
# Wed, 12 Oct 2022 21:41:25 GMT
ENV JAVA_VERSION=18.0.2.1
# Wed, 12 Oct 2022 21:41:37 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_linux-x64_bin.tar.gz'; 			downloadSha256='3bfdb59fc38884672677cebca9a216902d87fe867563182ae8bc3373a65a2ebd'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='79900237a5912045f8c9f1065b5204a474803cbbb4d075ab9620650fb75dfc1b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 12 Oct 2022 21:41:37 GMT
CMD ["jshell"]
# Wed, 12 Oct 2022 22:02:52 GMT
RUN microdnf install findutils git
# Wed, 12 Oct 2022 22:02:53 GMT
ARG MAVEN_VERSION=3.8.6
# Wed, 12 Oct 2022 22:02:53 GMT
ARG USER_HOME_DIR=/root
# Wed, 12 Oct 2022 22:02:53 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Wed, 12 Oct 2022 22:02:53 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Wed, 12 Oct 2022 22:02:55 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 12 Oct 2022 22:02:55 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 12 Oct 2022 22:02:55 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 12 Oct 2022 22:02:56 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 12 Oct 2022 22:02:56 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 12 Oct 2022 22:02:56 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 12 Oct 2022 22:02:56 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:5ed150ed0abef03007b46722de75bcb3e517f22532a46146fcec4fb1761d4347`  
		Last Modified: Wed, 12 Oct 2022 21:22:08 GMT  
		Size: 40.6 MB (40589408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8fce0a0221dc76ef1ed6d64872744f5f3b00d86ec9efaa593d6f606dbd55ab`  
		Last Modified: Wed, 12 Oct 2022 21:44:03 GMT  
		Size: 12.2 MB (12231062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b1ab00442e1823799fd319248209689c83674a36012ff2268d313be4207fab9`  
		Last Modified: Wed, 12 Oct 2022 21:45:19 GMT  
		Size: 188.7 MB (188744851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9564d04b1c53479d9812996615964f7641901f215d6c3672e090eaaeea5e5268`  
		Last Modified: Wed, 12 Oct 2022 22:05:26 GMT  
		Size: 192.6 MB (192609641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fe600d818b8ffadf2f254437877bc07d2535d6f1aca52e591b0b1df1918686f`  
		Last Modified: Wed, 12 Oct 2022 22:05:11 GMT  
		Size: 8.7 MB (8739510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5241e84a2ad073d0a62c549f510bfb12cb47246d8b5ce1e7ce82dff7025e195`  
		Last Modified: Wed, 12 Oct 2022 22:05:10 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f86921713a87b560d4cdb221bc7370f410fdf510b570c9ebceaf3c3f3d2688c`  
		Last Modified: Wed, 12 Oct 2022 22:05:11 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-openjdk-18` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:f25f92477b9e700dd3be9c3f0ed37bbcf7844b7081f480461d4db325d03044f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **452.7 MB (452689186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bd5f6d698f1c175781bb6619634f92ce16afa02765f454e1a6940f05c556b1e`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 12 Oct 2022 20:40:56 GMT
ADD file:049ff2e28998fde860d1a12f43ec245d10345a71953f67108180c23c237ce26e in / 
# Wed, 12 Oct 2022 20:40:56 GMT
CMD ["/bin/bash"]
# Wed, 12 Oct 2022 20:58:37 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 12 Oct 2022 21:15:44 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Wed, 12 Oct 2022 21:15:45 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Oct 2022 21:15:46 GMT
ENV LANG=C.UTF-8
# Wed, 12 Oct 2022 21:15:47 GMT
ENV JAVA_VERSION=18.0.2.1
# Wed, 12 Oct 2022 21:15:58 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_linux-x64_bin.tar.gz'; 			downloadSha256='3bfdb59fc38884672677cebca9a216902d87fe867563182ae8bc3373a65a2ebd'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='79900237a5912045f8c9f1065b5204a474803cbbb4d075ab9620650fb75dfc1b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 12 Oct 2022 21:15:58 GMT
CMD ["jshell"]
# Wed, 12 Oct 2022 21:41:02 GMT
RUN microdnf install findutils git
# Wed, 12 Oct 2022 21:41:03 GMT
ARG MAVEN_VERSION=3.8.6
# Wed, 12 Oct 2022 21:41:03 GMT
ARG USER_HOME_DIR=/root
# Wed, 12 Oct 2022 21:41:04 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Wed, 12 Oct 2022 21:41:05 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Wed, 12 Oct 2022 21:41:15 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 12 Oct 2022 21:41:16 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 12 Oct 2022 21:41:17 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 12 Oct 2022 21:41:19 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 12 Oct 2022 21:41:20 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 12 Oct 2022 21:41:20 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 12 Oct 2022 21:41:21 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:828689dcde4b0fe396ab27cf3a6d5f71ee01d48891421ec4381d74ed415be5d0`  
		Last Modified: Wed, 12 Oct 2022 20:42:33 GMT  
		Size: 39.4 MB (39409290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f742b2cfb7e7c72c98123d08c444932851dc28c95bdb7a2a6a4ebfbcd5456bd`  
		Last Modified: Wed, 12 Oct 2022 21:20:59 GMT  
		Size: 13.1 MB (13054769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642e9a9e0a5fb5861127a7b90ed2c284e64d3a692dfb0a11821127b99c9985d6`  
		Last Modified: Wed, 12 Oct 2022 21:22:37 GMT  
		Size: 187.7 MB (187659415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eacf770dd642f8d757e682e6da32f99c9d210397c1eb2424c29909ab6bd388ff`  
		Last Modified: Wed, 12 Oct 2022 21:44:56 GMT  
		Size: 203.8 MB (203825032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80af197c67710bb35ee0653e53ba1cab45b7fa2b075a3e4fc194914a59c7427a`  
		Last Modified: Wed, 12 Oct 2022 21:44:40 GMT  
		Size: 8.7 MB (8739463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1437116ee2bd91f29007d812f463b5209dd6ad65908ddd590931243512639a`  
		Last Modified: Wed, 12 Oct 2022 21:44:38 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0d3427051bb9123eaf1e391189bc1364157b9a35433efac71d8added6fe0e1`  
		Last Modified: Wed, 12 Oct 2022 21:44:38 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
