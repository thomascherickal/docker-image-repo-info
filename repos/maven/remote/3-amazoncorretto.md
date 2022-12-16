## `maven:3-amazoncorretto`

```console
$ docker pull maven@sha256:2031cc006400b5f87c8c29b6bca933cfdb834067ec6d182c36aaba8b3703c31b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto` - linux; amd64

```console
$ docker pull maven@sha256:ea3950751ee0bb51032bc420bb9f54c83a7e72bafec61f5cf7f7b72b5b5699fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.5 MB (222451935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2659cbf6c2d7c923cd490b10012d550994ff5f3c60da929661a8b0464bbda59`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 16 Dec 2022 01:19:49 GMT
ADD file:a69ca7a5499bcd9d6e4317fdbd7256e93be44364bb746f5da10b4268c090bda0 in / 
# Fri, 16 Dec 2022 01:19:50 GMT
CMD ["/bin/bash"]
# Fri, 16 Dec 2022 02:14:08 GMT
ARG version=11.0.17.8-1
# Fri, 16 Dec 2022 02:14:46 GMT
# ARGS: version=11.0.17.8-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 16 Dec 2022 02:14:47 GMT
ENV LANG=C.UTF-8
# Fri, 16 Dec 2022 02:14:47 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Fri, 16 Dec 2022 03:11:50 GMT
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Fri, 16 Dec 2022 03:11:51 GMT
ARG MAVEN_VERSION=3.8.6
# Fri, 16 Dec 2022 03:11:51 GMT
ARG USER_HOME_DIR=/root
# Fri, 16 Dec 2022 03:11:51 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Fri, 16 Dec 2022 03:11:51 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Fri, 16 Dec 2022 03:11:55 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 16 Dec 2022 03:11:55 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 16 Dec 2022 03:11:55 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 16 Dec 2022 03:11:56 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 16 Dec 2022 03:11:56 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 16 Dec 2022 03:11:56 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 16 Dec 2022 03:11:56 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:5b4a36b5b78f93a5f470cf722b313bb32cddb0f8e0fa0db348059b5c0881b04f`  
		Last Modified: Thu, 15 Dec 2022 23:08:20 GMT  
		Size: 62.3 MB (62328625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c4a50287c9345fabef12ad41b61e3450e3400fbe99f5d48281ceb781041ae3`  
		Last Modified: Fri, 16 Dec 2022 02:22:14 GMT  
		Size: 147.8 MB (147751328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a905e371765dc7ee0d62f082d44b999c781087a6898c007030d5af319d4baf`  
		Last Modified: Fri, 16 Dec 2022 03:14:49 GMT  
		Size: 3.6 MB (3631269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad9a1992ea4d21c2b45bf0b314bd677489dc0101da72e64b2757219d0d50ea3`  
		Last Modified: Fri, 16 Dec 2022 03:14:49 GMT  
		Size: 8.7 MB (8739502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1855a537828c4996b3b02556efaad9e15896161695ca29bcae435dc8a095fb3`  
		Last Modified: Fri, 16 Dec 2022 03:14:48 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e04effe89c6edc06495bc5104832f6f6a010949a9607f7ed6434922518eb84b3`  
		Last Modified: Fri, 16 Dec 2022 03:14:48 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:b30115ed998a5f308df27be48a7b6c341323c421cb46866a35963513fcfa7b06
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.3 MB (221260736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c4fff7644a190477867153a4142c8fa294884b4f0a8ac554343f9d3801402ae`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 16 Dec 2022 00:41:05 GMT
ADD file:26a6bf75c84c408d289e5569f13b1c65206966f875cdfc53ded0670cb85e35bf in / 
# Fri, 16 Dec 2022 00:41:07 GMT
CMD ["/bin/bash"]
# Fri, 16 Dec 2022 00:59:23 GMT
ARG version=11.0.17.8-1
# Fri, 16 Dec 2022 00:59:42 GMT
# ARGS: version=11.0.17.8-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 16 Dec 2022 00:59:44 GMT
ENV LANG=C.UTF-8
# Fri, 16 Dec 2022 00:59:44 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Fri, 16 Dec 2022 01:22:15 GMT
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Fri, 16 Dec 2022 01:22:15 GMT
ARG MAVEN_VERSION=3.8.6
# Fri, 16 Dec 2022 01:22:15 GMT
ARG USER_HOME_DIR=/root
# Fri, 16 Dec 2022 01:22:15 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Fri, 16 Dec 2022 01:22:15 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Fri, 16 Dec 2022 01:22:21 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 16 Dec 2022 01:22:21 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 16 Dec 2022 01:22:21 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 16 Dec 2022 01:22:21 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 16 Dec 2022 01:22:21 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 16 Dec 2022 01:22:21 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 16 Dec 2022 01:22:22 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:6cbfee25f0741b3d3f4d2474d904a200cd8404a01aa17813bf3fc3d4ebb551a4`  
		Last Modified: Thu, 15 Dec 2022 23:08:20 GMT  
		Size: 64.0 MB (63964214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0aade9a94f7c23d8fc79b4c11ce14d37b8569a6fec3017a295169ff500ec8d8`  
		Last Modified: Fri, 16 Dec 2022 01:03:43 GMT  
		Size: 144.9 MB (144905924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f97abaac636b83c48901a954aad2590cc61f80cced9b27aa8d43b44f43a9f30`  
		Last Modified: Fri, 16 Dec 2022 01:24:38 GMT  
		Size: 3.6 MB (3649884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33db164bd6b73340003cd55423a8dd5849cc7a487cc94c2bb357ccc1a8dc3ca1`  
		Last Modified: Fri, 16 Dec 2022 01:24:38 GMT  
		Size: 8.7 MB (8739505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1fbf8565a1c4b4d0234f157780196cad6f3c6da31c3715376cf33e20181ae58`  
		Last Modified: Fri, 16 Dec 2022 01:24:37 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeee5a1b81e9a2419e7b0709853995c8c8d8143e3577a8ad85dc85ba657e485`  
		Last Modified: Fri, 16 Dec 2022 01:24:37 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
