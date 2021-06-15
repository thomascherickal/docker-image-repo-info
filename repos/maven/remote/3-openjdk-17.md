## `maven:3-openjdk-17`

```console
$ docker pull maven@sha256:3fee88a0bafb14a0961a5dfbd7f6811e2799b434246b6b77b51478c3f2d6fd46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-openjdk-17` - linux; amd64

```console
$ docker pull maven@sha256:053b0881224bab7808139a9262a03c4fcd5432259b47b9a3110d7567a5f2f22f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **416.7 MB (416732124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0df8750e5d11942efd2f628532aaf097688ec957350833c2afd19c4c3b45aa23`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 02 Jun 2021 17:21:00 GMT
ADD file:b4c18f27ab03ed63f96174673a8d97d4b1b6abb552b6fe3201c6aec934e8312f in / 
# Wed, 02 Jun 2021 17:21:00 GMT
CMD ["/bin/bash"]
# Wed, 02 Jun 2021 17:37:54 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 02 Jun 2021 17:37:55 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Wed, 02 Jun 2021 17:37:55 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Jun 2021 17:37:55 GMT
ENV LANG=C.UTF-8
# Mon, 14 Jun 2021 21:22:49 GMT
ENV JAVA_VERSION=17-ea+26
# Mon, 14 Jun 2021 21:22:59 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/26/GPL/openjdk-17-ea+26_linux-x64_bin.tar.gz'; 			downloadSha256='9efe9a6b68a24e16a2a2e34b0f33c25fe17dcdace07970840e2a9bd014d13c30'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/26/GPL/openjdk-17-ea+26_linux-aarch64_bin.tar.gz'; 			downloadSha256='5914ae141494689362b74b2edc546f94f3ac4a4c8d6863a20048e851a0f6213f'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 14 Jun 2021 21:23:00 GMT
CMD ["jshell"]
# Mon, 14 Jun 2021 22:01:30 GMT
ARG MAVEN_VERSION=3.8.1
# Mon, 14 Jun 2021 22:01:30 GMT
ARG USER_HOME_DIR=/root
# Mon, 14 Jun 2021 22:01:30 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Mon, 14 Jun 2021 22:01:30 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Mon, 14 Jun 2021 22:01:56 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN microdnf install findutils git
# Mon, 14 Jun 2021 22:01:59 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Mon, 14 Jun 2021 22:01:59 GMT
ENV MAVEN_HOME=/usr/share/maven
# Mon, 14 Jun 2021 22:01:59 GMT
ENV MAVEN_CONFIG=/root/.m2
# Mon, 14 Jun 2021 22:01:59 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Mon, 14 Jun 2021 22:01:59 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Mon, 14 Jun 2021 22:02:00 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Mon, 14 Jun 2021 22:02:00 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:5a581c13a8b96af42c06955acd88fdb3aff53edcbdd33faa7bca9854fd8bfbaf`  
		Last Modified: Wed, 02 Jun 2021 17:22:10 GMT  
		Size: 42.2 MB (42183647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26cd02acd9c2b40dba18c3fe68882bcb5ebda0caeb5e550965d9ac81e3b55fbf`  
		Last Modified: Wed, 02 Jun 2021 17:43:15 GMT  
		Size: 13.4 MB (13400021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d558b04b7f9486d18df402f2dd765fd3dcbafa1e977313e3b3d05705a3647cc0`  
		Last Modified: Mon, 14 Jun 2021 21:31:21 GMT  
		Size: 187.2 MB (187151465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe393044451c8201b2ed1d8a9969ba1faa5f81e61f695494164974ee55a05130`  
		Last Modified: Mon, 14 Jun 2021 22:04:58 GMT  
		Size: 164.4 MB (164384794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054c73144a514dcb99574ccf717f3b4b8dec848ca78f42b14145bf48746a1e1b`  
		Last Modified: Mon, 14 Jun 2021 22:04:44 GMT  
		Size: 9.6 MB (9610981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c4ccc439f9583ee6be3272f44fcfe7f60fe6d0637694c40c08d320872defc2`  
		Last Modified: Mon, 14 Jun 2021 22:04:43 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5a9c88e60ed8907e557aeefa76d495ffb5534a4e8f0185308aea20ad3882f4`  
		Last Modified: Mon, 14 Jun 2021 22:04:43 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-openjdk-17` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:ac08a3228d4f01ed9c79aede955c6f72817ea7bfa3071f7e3a96975d12c3353f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.0 MB (394996656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63d7e91e66962a4122e0aa8a83d96963c4116447df9249d8dfaccfc84459c0ff`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 02 Jun 2021 17:41:03 GMT
ADD file:78235baf524ed2a030d5aee5012599777d5026bf83699d8d03662420d6804653 in / 
# Wed, 02 Jun 2021 17:41:03 GMT
CMD ["/bin/bash"]
# Wed, 02 Jun 2021 17:58:06 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 02 Jun 2021 17:58:06 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Wed, 02 Jun 2021 17:58:07 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Jun 2021 17:58:07 GMT
ENV LANG=C.UTF-8
# Mon, 14 Jun 2021 20:44:08 GMT
ENV JAVA_VERSION=17-ea+26
# Mon, 14 Jun 2021 20:44:18 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/26/GPL/openjdk-17-ea+26_linux-x64_bin.tar.gz'; 			downloadSha256='9efe9a6b68a24e16a2a2e34b0f33c25fe17dcdace07970840e2a9bd014d13c30'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/26/GPL/openjdk-17-ea+26_linux-aarch64_bin.tar.gz'; 			downloadSha256='5914ae141494689362b74b2edc546f94f3ac4a4c8d6863a20048e851a0f6213f'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 14 Jun 2021 20:44:18 GMT
CMD ["jshell"]
# Mon, 14 Jun 2021 21:31:58 GMT
ARG MAVEN_VERSION=3.8.1
# Mon, 14 Jun 2021 21:31:59 GMT
ARG USER_HOME_DIR=/root
# Mon, 14 Jun 2021 21:31:59 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Mon, 14 Jun 2021 21:31:59 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Mon, 14 Jun 2021 21:32:32 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN microdnf install findutils git
# Mon, 14 Jun 2021 21:32:35 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Mon, 14 Jun 2021 21:32:35 GMT
ENV MAVEN_HOME=/usr/share/maven
# Mon, 14 Jun 2021 21:32:35 GMT
ENV MAVEN_CONFIG=/root/.m2
# Mon, 14 Jun 2021 21:32:35 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Mon, 14 Jun 2021 21:32:36 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Mon, 14 Jun 2021 21:32:36 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Mon, 14 Jun 2021 21:32:36 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:4a780b35fbf92abdbd808aa7d8f30cb6c03db446424f04738aa715ba4935a1f6`  
		Last Modified: Wed, 02 Jun 2021 17:42:09 GMT  
		Size: 42.1 MB (42068993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b11c9e8386348cc9050d7280e19b5987140671e2de847d978f53d4ec578f94`  
		Last Modified: Wed, 02 Jun 2021 18:08:16 GMT  
		Size: 14.2 MB (14183644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a62ef88dfdd71498460ea46ba8e4705b31f1fc3d5e5fd8360139e33353ce5e0b`  
		Last Modified: Mon, 14 Jun 2021 20:59:24 GMT  
		Size: 186.0 MB (185967681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a46568ead303ac2b925ca80fb02606f336b0032960721cdfd0c6f58a9b7c38c`  
		Last Modified: Mon, 14 Jun 2021 21:37:23 GMT  
		Size: 143.2 MB (143164159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3d66b1c8a263b3af9e9e31c4c035f771318d2f53628b8a747cd08fcd1a2606`  
		Last Modified: Mon, 14 Jun 2021 21:37:09 GMT  
		Size: 9.6 MB (9610961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:899d688ca2f9876ede7f8a0c93912012b3b6548a3de708ab389fe1d3bcbcff9f`  
		Last Modified: Mon, 14 Jun 2021 21:37:07 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74780b850e224b454f8cf48e3a8fbc88129866897083434e94388f966329cc5`  
		Last Modified: Mon, 14 Jun 2021 21:37:08 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
