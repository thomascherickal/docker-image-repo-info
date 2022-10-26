## `maven:3-amazoncorretto-19`

```console
$ docker pull maven@sha256:42eccb4a455911a1699f7cece7f14c4c091c06444f6a20b5cbd930ec9011dd3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-19` - linux; amd64

```console
$ docker pull maven@sha256:7f64963d57664d648eb03effe9ac00222cdb60d616f8541f96990d46e2699243
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.1 MB (234067483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a1d0f6a750035a917164e07c8e4ad97e8183c676284b8aef5f58236fdbeae6d`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 21 Oct 2022 00:19:49 GMT
ADD file:33ce740675602f8911c110c617b08d74ebe9c26c82226b4815019d8c2d0a2263 in / 
# Fri, 21 Oct 2022 00:19:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 01:10:48 GMT
ARG version=19.0.1.10-1
# Fri, 21 Oct 2022 01:11:13 GMT
# ARGS: version=19.0.1.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-19-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-19-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 21 Oct 2022 01:11:13 GMT
ENV LANG=C.UTF-8
# Fri, 21 Oct 2022 01:11:13 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-19-amazon-corretto
# Fri, 21 Oct 2022 02:02:47 GMT
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Fri, 21 Oct 2022 02:02:47 GMT
ARG MAVEN_VERSION=3.8.6
# Fri, 21 Oct 2022 02:02:47 GMT
ARG USER_HOME_DIR=/root
# Fri, 21 Oct 2022 02:02:47 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Fri, 21 Oct 2022 02:02:48 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Fri, 21 Oct 2022 02:02:49 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 21 Oct 2022 02:02:50 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 21 Oct 2022 02:02:50 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 21 Oct 2022 02:02:50 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 21 Oct 2022 02:02:50 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 21 Oct 2022 02:02:50 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 21 Oct 2022 02:02:50 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:e3cfe889ce0a44ace07ec174bd2a7e9022e493956fba0069812a53f81a6040e2`  
		Last Modified: Wed, 19 Oct 2022 18:11:43 GMT  
		Size: 62.3 MB (62306642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf6c501567b9864d5477f3bb4e798e53137c8a50576fa5bba6ccbb83c2d6faa`  
		Last Modified: Fri, 21 Oct 2022 01:16:26 GMT  
		Size: 159.4 MB (159387773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ec04f180c15e2525067ab2337135fd8acbff9f4b1e374d3ddf34bfaa814b24`  
		Last Modified: Fri, 21 Oct 2022 02:05:53 GMT  
		Size: 3.6 MB (3632363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392650e96195756083ae0cb190e885945eaa1f01ff8e78095155e652be04c144`  
		Last Modified: Fri, 21 Oct 2022 02:05:58 GMT  
		Size: 8.7 MB (8739492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4874140de48a8a53768f68ce743b8fb615ec6537be99e728b405858aba6770fc`  
		Last Modified: Fri, 21 Oct 2022 02:05:53 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b564371c212318f17f1a57f35b321664d08f2910a66088e919137e77657069`  
		Last Modified: Fri, 21 Oct 2022 02:05:53 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-19` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:b89a3ca24e2261aba3739e5afffccdc89cf2bc95ac0384d25ec9a309985144a6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.1 MB (234127494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16b9ecf77abc8974f382e2a769ab1581d27b12e615bf8772edb3c96b3fecf0e4`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 26 Oct 2022 15:27:06 GMT
ADD file:45362bc0bb55d35f704a938eb431f8accb86d1bb8e52b78f3ef34eb141c3ed82 in / 
# Wed, 26 Oct 2022 15:27:06 GMT
CMD ["/bin/bash"]
# Wed, 26 Oct 2022 18:56:09 GMT
ARG version=19.0.1.10-1
# Wed, 26 Oct 2022 18:56:32 GMT
# ARGS: version=19.0.1.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-19-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-19-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 26 Oct 2022 18:56:34 GMT
ENV LANG=C.UTF-8
# Wed, 26 Oct 2022 18:56:34 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-19-amazon-corretto
# Wed, 26 Oct 2022 19:23:58 GMT
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Wed, 26 Oct 2022 19:23:58 GMT
ARG MAVEN_VERSION=3.8.6
# Wed, 26 Oct 2022 19:23:58 GMT
ARG USER_HOME_DIR=/root
# Wed, 26 Oct 2022 19:23:58 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Wed, 26 Oct 2022 19:23:58 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Wed, 26 Oct 2022 19:24:06 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 26 Oct 2022 19:24:06 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 26 Oct 2022 19:24:06 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 26 Oct 2022 19:24:06 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 26 Oct 2022 19:24:06 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 26 Oct 2022 19:24:06 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 26 Oct 2022 19:24:06 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:d900cba9f9f55565485a1181c89317c2718b6232095971d67af440a33db15594`  
		Last Modified: Wed, 19 Oct 2022 18:11:20 GMT  
		Size: 63.9 MB (63919869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e48d5af71f1011c2a195007b5e77fe27cdf006eac9b0fe3b573d468ce6e7e0`  
		Last Modified: Wed, 26 Oct 2022 18:58:31 GMT  
		Size: 157.8 MB (157824019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3756abed46a012fe74b2564ef69674a01e4b3fcd9318e0f209f7867e59abee4e`  
		Last Modified: Wed, 26 Oct 2022 19:26:34 GMT  
		Size: 3.6 MB (3642895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c2f8078730798643d0b139216ddde6b70731bdc210b72e511099a66ea6330ea`  
		Last Modified: Wed, 26 Oct 2022 19:26:34 GMT  
		Size: 8.7 MB (8739502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d06ff5181b84935f136da5eca250d90ccf71135f999ac47c54cd7460bd9eeb`  
		Last Modified: Wed, 26 Oct 2022 19:26:33 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bcbd4d4500729e95d66edd3cdd649ef2bc10bac2be2304356c8bdca76107501`  
		Last Modified: Wed, 26 Oct 2022 19:26:33 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
