## `maven:amazoncorretto`

```console
$ docker pull maven@sha256:8f4dc83182260f267808f6dbb05db4fa041955e35d77d058793b78aa75ad28d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:amazoncorretto` - linux; amd64

```console
$ docker pull maven@sha256:7b712a8292029adde613894e0ed7b4bd4b5a6445a1487d2007537aff3e2b54db
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.6 MB (221635812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:620cf51e78103943ea69f6f90ca7df3245add27b916307dff6c7acca24ac41bd`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 27 Jan 2021 22:19:43 GMT
ADD file:bcd0b903093ee2c81a54e8bdc50176f4038662ab936aa0d94af08458d508aef6 in / 
# Wed, 27 Jan 2021 22:19:43 GMT
CMD ["/bin/bash"]
# Wed, 27 Jan 2021 22:38:16 GMT
ARG version=11.0.10.9-1
# Wed, 27 Jan 2021 22:38:33 GMT
# ARGS: version=11.0.10.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 27 Jan 2021 22:38:34 GMT
ENV LANG=C.UTF-8
# Wed, 27 Jan 2021 22:38:34 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Wed, 27 Jan 2021 22:57:40 GMT
ARG MAVEN_VERSION=3.6.3
# Wed, 27 Jan 2021 22:57:40 GMT
ARG USER_HOME_DIR=/root
# Wed, 27 Jan 2021 22:57:40 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Wed, 27 Jan 2021 22:57:40 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Wed, 27 Jan 2021 22:57:47 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Wed, 27 Jan 2021 22:57:48 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 27 Jan 2021 22:57:48 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 27 Jan 2021 22:57:49 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 27 Jan 2021 22:57:49 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 27 Jan 2021 22:57:49 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 27 Jan 2021 22:57:49 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 27 Jan 2021 22:57:50 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:62350c28fdb7b7cbd0e199dd893555ed129ed85da482d882b1eeb574988ea7d6`  
		Last Modified: Wed, 27 Jan 2021 22:21:18 GMT  
		Size: 62.0 MB (61996576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:383b03c8da6a748602d2579040e3d1b907c0c4c0b6d59b586e8e41c342acace6`  
		Last Modified: Wed, 27 Jan 2021 22:40:22 GMT  
		Size: 146.5 MB (146517618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593d8a06a95f33e4b86c01a0a5f59257a19f5a453e1de0ee334b5c74372e0125`  
		Last Modified: Wed, 27 Jan 2021 23:00:11 GMT  
		Size: 3.5 MB (3539214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09298528a2c1162f4cbf86208d4d52b5fb8e32bed3c7d9ac27ded8dee29e6a2c`  
		Last Modified: Wed, 27 Jan 2021 23:00:11 GMT  
		Size: 9.6 MB (9581193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330e0d278e579ce55fe9b138fcba85d76487f39828f7d6ec1b600329145c2a2f`  
		Last Modified: Wed, 27 Jan 2021 23:00:10 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c75f22558ff120d1c00c3c9713314590e057fe400d6dbac78998c3e37ac4c59`  
		Last Modified: Wed, 27 Jan 2021 23:00:10 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:amazoncorretto` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:6048cf14fe0f7afdcc26d6590bd5ca23aabffd234cd9e4bbdac915473bccf808
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.5 MB (221453412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:428e0a7fb0a2d080f79c2d24cced6ed81128127815f44a260ac186a068e8c3c0`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 27 Jan 2021 23:09:56 GMT
ADD file:7f69686262e0e0e5415d42ac0371f7d0df0330bc4f0556e5d4b73dd78ceb1197 in / 
# Wed, 27 Jan 2021 23:10:02 GMT
CMD ["/bin/bash"]
# Wed, 27 Jan 2021 23:48:47 GMT
ARG version=11.0.10.9-1
# Wed, 27 Jan 2021 23:49:16 GMT
# ARGS: version=11.0.10.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 27 Jan 2021 23:49:18 GMT
ENV LANG=C.UTF-8
# Wed, 27 Jan 2021 23:49:19 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Thu, 28 Jan 2021 00:25:07 GMT
ARG MAVEN_VERSION=3.6.3
# Thu, 28 Jan 2021 00:25:08 GMT
ARG USER_HOME_DIR=/root
# Thu, 28 Jan 2021 00:25:08 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Thu, 28 Jan 2021 00:25:09 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Thu, 28 Jan 2021 00:25:21 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Thu, 28 Jan 2021 00:25:24 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 28 Jan 2021 00:25:25 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 28 Jan 2021 00:25:26 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 28 Jan 2021 00:25:26 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 28 Jan 2021 00:25:27 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 28 Jan 2021 00:25:28 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 28 Jan 2021 00:25:29 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:c6741bcf27a42820ff66e35cc842cec9a845e9e9dba4ff7bd465fc6161442a86`  
		Last Modified: Wed, 27 Jan 2021 23:11:10 GMT  
		Size: 63.7 MB (63704713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1123d55f3d235ec0542a1258da4a2e172d991fd0ea8ad44352d7a764fa34461e`  
		Last Modified: Wed, 27 Jan 2021 23:51:20 GMT  
		Size: 144.6 MB (144591090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcae9878e737ca09618e832881646cfa50a133700211822262c90ad197125971`  
		Last Modified: Thu, 28 Jan 2021 00:28:22 GMT  
		Size: 3.6 MB (3575205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e5425cb70d1f14c5a14a94691f3609bc4d3a2898ac6a9e012e2307bed6dd74`  
		Last Modified: Thu, 28 Jan 2021 00:28:21 GMT  
		Size: 9.6 MB (9581195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4528b865157a815bd42888163cad836b9f91219041d4ab63545437907e98d9e2`  
		Last Modified: Thu, 28 Jan 2021 00:28:20 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a010122a79488f7e0818a4d337073c180f044b393313886144e7f4081f9f59`  
		Last Modified: Thu, 28 Jan 2021 00:28:20 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
