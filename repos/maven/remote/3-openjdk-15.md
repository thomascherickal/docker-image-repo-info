## `maven:3-openjdk-15`

```console
$ docker pull maven@sha256:eba9c1d9f678ef13cfc961da2b70b06948eee293a512f0d2d7a11bd14bf84d9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-openjdk-15` - linux; amd64

```console
$ docker pull maven@sha256:0ea9dd84f24edf11068a4b502528c140cadd02e00b0a11d583974753cd72c2a2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.9 MB (350896649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89cbe56afc70e453ac6222060640cbc5a616a361250aefa371cc5fc6e15ae6df`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 30 Aug 2018 21:49:27 GMT
MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>
# Fri, 11 Sep 2020 09:49:59 GMT
ADD file:50f1210cda2b0463fc72e0e56a1636cc26b6685c08c7e2cabf7fc2329b04537b in / 
# Fri, 11 Sep 2020 09:49:59 GMT
CMD ["/bin/bash"]
# Fri, 11 Sep 2020 10:23:52 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 11 Sep 2020 10:23:52 GMT
ENV LANG=C.UTF-8
# Fri, 11 Sep 2020 10:25:00 GMT
ENV JAVA_HOME=/usr/java/openjdk-15
# Fri, 11 Sep 2020 10:25:00 GMT
ENV PATH=/usr/java/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Sep 2020 10:25:01 GMT
ENV JAVA_VERSION=15
# Fri, 11 Sep 2020 10:25:39 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/GA/jdk15/779bf45e88a44cbd9ea6621d33e33db1/36/GPL/openjdk-15_linux-aarch64_bin.tar.gz; 			downloadSha256=01e7e07dd8a67a65b32fdcaff75ba3f21cd9cfc749287e7c9b1c6037f96a3537; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/GA/jdk15/779bf45e88a44cbd9ea6621d33e33db1/36/GPL/openjdk-15_linux-x64_bin.tar.gz; 			downloadSha256=bb67cadee687d7b486583d03c9850342afea4593be4f436044d785fba9508fb7; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Sep 2020 10:25:40 GMT
CMD ["jshell"]
# Fri, 11 Sep 2020 11:03:11 GMT
ARG MAVEN_VERSION=3.6.3
# Fri, 11 Sep 2020 11:03:12 GMT
ARG USER_HOME_DIR=/root
# Fri, 11 Sep 2020 11:03:12 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Fri, 11 Sep 2020 11:03:12 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Fri, 11 Sep 2020 11:03:25 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN microdnf install findutils
# Fri, 11 Sep 2020 11:03:26 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 11 Sep 2020 11:03:27 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 11 Sep 2020 11:03:27 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 11 Sep 2020 11:03:27 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 11 Sep 2020 11:03:27 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 11 Sep 2020 11:03:27 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 11 Sep 2020 11:03:27 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:4374a5c9a09aec3eb7169ecd4f7ff91fedce7aeb23b479e5f83af47ec91c5d7c`  
		Last Modified: Fri, 11 Sep 2020 09:51:53 GMT  
		Size: 53.2 MB (53194134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628f382586998761d4d6eaf3d2f5d56829c3099ff15ff17f86c2767c85530a14`  
		Last Modified: Fri, 11 Sep 2020 10:28:24 GMT  
		Size: 13.4 MB (13409452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7d6e4835ca8690c3fc3b84969a166e2b131fea809e448db00637a4899a15ed`  
		Last Modified: Fri, 11 Sep 2020 10:29:29 GMT  
		Size: 195.8 MB (195751109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7fc21f60a10cd0b9d0e2e49bc0e15d35aa76796e7817fd11730838640172aa5`  
		Last Modified: Fri, 11 Sep 2020 11:05:37 GMT  
		Size: 79.0 MB (78959518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a439c29d0ce642452d83d4c83be4de6f1d730610c46712be4cd981652cd86e`  
		Last Modified: Fri, 11 Sep 2020 11:05:32 GMT  
		Size: 9.6 MB (9581225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb41d2cc92a86370eddca4463861cee8fb7e3ee6aaadfad6c922ce207056238d`  
		Last Modified: Fri, 11 Sep 2020 11:05:32 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9a89481a52a3fd4658c7558b8b6b4e30f3a2ea63d48f06524028b67100d615`  
		Last Modified: Fri, 11 Sep 2020 11:05:31 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-openjdk-15` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:ec3d7c92f11adf2b98ffca6ab2e66d022dc8c1ce81509f2d8600b7e9990f5e32
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.3 MB (305292673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:844fcb8bd075e8714a76f5cc6a3afe93119117173228df9349c3f154a8909200`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 31 May 2019 21:40:52 GMT
MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>
# Fri, 11 Sep 2020 06:39:42 GMT
ADD file:c8745918ce90d90daefed5ea00db8b400158109f53a85988975f96ce7084c609 in / 
# Fri, 11 Sep 2020 06:39:46 GMT
CMD ["/bin/bash"]
# Fri, 11 Sep 2020 07:09:36 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 11 Sep 2020 07:09:38 GMT
ENV LANG=C.UTF-8
# Fri, 11 Sep 2020 07:10:43 GMT
ENV JAVA_HOME=/usr/java/openjdk-15
# Fri, 11 Sep 2020 07:10:45 GMT
ENV PATH=/usr/java/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Sep 2020 07:10:45 GMT
ENV JAVA_VERSION=15
# Fri, 11 Sep 2020 07:11:01 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/GA/jdk15/779bf45e88a44cbd9ea6621d33e33db1/36/GPL/openjdk-15_linux-aarch64_bin.tar.gz; 			downloadSha256=01e7e07dd8a67a65b32fdcaff75ba3f21cd9cfc749287e7c9b1c6037f96a3537; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/GA/jdk15/779bf45e88a44cbd9ea6621d33e33db1/36/GPL/openjdk-15_linux-x64_bin.tar.gz; 			downloadSha256=bb67cadee687d7b486583d03c9850342afea4593be4f436044d785fba9508fb7; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Sep 2020 07:11:03 GMT
CMD ["jshell"]
# Fri, 11 Sep 2020 07:35:47 GMT
ARG MAVEN_VERSION=3.6.3
# Fri, 11 Sep 2020 07:35:48 GMT
ARG USER_HOME_DIR=/root
# Fri, 11 Sep 2020 07:35:48 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Fri, 11 Sep 2020 07:35:49 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Fri, 11 Sep 2020 07:36:07 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN microdnf install findutils
# Fri, 11 Sep 2020 07:36:18 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 11 Sep 2020 07:36:19 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 11 Sep 2020 07:36:20 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 11 Sep 2020 07:36:20 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 11 Sep 2020 07:36:21 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 11 Sep 2020 07:36:22 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 11 Sep 2020 07:36:22 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:b0a89fc27ec40345cd34fac22c2caa5adb9d10c730a6bd900435007be8e8ac80`  
		Last Modified: Fri, 11 Sep 2020 06:41:50 GMT  
		Size: 53.3 MB (53291835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54565c8f5569913127216a9630522b7177b23429e528cdd38041680808117936`  
		Last Modified: Fri, 11 Sep 2020 07:13:47 GMT  
		Size: 14.3 MB (14311816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40191ee521b563b4db94363a57a9631c007fa36ee9b8189d59a989b4db0e524e`  
		Last Modified: Fri, 11 Sep 2020 07:15:23 GMT  
		Size: 174.9 MB (174859066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a473ed1e88fa047d54c6b539561918cbdff273cfe02b01a6e6df1042067e5617`  
		Last Modified: Fri, 11 Sep 2020 07:38:12 GMT  
		Size: 53.2 MB (53247544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5862828b97ec6586efe938c96729e2e91e85f98d6aa7c9494a90abf6003fb5c2`  
		Last Modified: Fri, 11 Sep 2020 07:38:06 GMT  
		Size: 9.6 MB (9581198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e64ca6e407a51c31ec0372286b52be2ed342352ce798e5ba82d9433e8fc633`  
		Last Modified: Fri, 11 Sep 2020 07:38:04 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e16189b1d7554693e5c8822debf17cda167eef8550e0dcb579d05390ef2971`  
		Last Modified: Fri, 11 Sep 2020 07:38:04 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
