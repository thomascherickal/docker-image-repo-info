## `maven:3-amazoncorretto-11`

```console
$ docker pull maven@sha256:96014289aeb2b8ae6d8d909c164cda93ac122a722a7da145e7d0a96818789bc1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-11` - linux; amd64

```console
$ docker pull maven@sha256:e044fd00edcf7fabca822d0d09b7cbb56ad32695d0d77fe8c75a816b27141d10
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.6 MB (221629494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8f9e83ffe7190d0271eefa4f1e5dc7be41738fe0ecaf75dcdb26ce0eab1a8ff`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 24 Feb 2021 19:19:48 GMT
ADD file:40bc6ac9b95149d9077e8e692feea2208fcd1c5883673953b295e6acd014ea38 in / 
# Wed, 24 Feb 2021 19:19:48 GMT
CMD ["/bin/bash"]
# Thu, 18 Mar 2021 01:19:44 GMT
ARG version=11.0.10.9-1
# Thu, 18 Mar 2021 01:19:58 GMT
# ARGS: version=11.0.10.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 18 Mar 2021 01:19:59 GMT
ENV LANG=C.UTF-8
# Thu, 18 Mar 2021 01:19:59 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Thu, 18 Mar 2021 01:43:46 GMT
ARG MAVEN_VERSION=3.6.3
# Thu, 18 Mar 2021 01:43:46 GMT
ARG USER_HOME_DIR=/root
# Thu, 18 Mar 2021 01:43:46 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Thu, 18 Mar 2021 01:43:46 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Thu, 18 Mar 2021 01:43:53 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Thu, 18 Mar 2021 01:43:54 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 18 Mar 2021 01:43:55 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 18 Mar 2021 01:43:55 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 18 Mar 2021 01:43:55 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 18 Mar 2021 01:43:55 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 18 Mar 2021 01:43:55 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 18 Mar 2021 01:43:56 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:9da98c321efd693e1dc19cc24c7c2cfa365c649f178da8ebdfdc5243d0b2f91a`  
		Last Modified: Wed, 24 Feb 2021 10:37:31 GMT  
		Size: 61.9 MB (61935160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf985284f9fa24b184b0d16544b81abd2ea6dc25403e2d928da2ec487277b821`  
		Last Modified: Thu, 18 Mar 2021 01:23:26 GMT  
		Size: 146.5 MB (146540033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64d1afc3eb617ac95c44dc78db844bc9f6e9912748fa074dbac0568ab8ed6f9`  
		Last Modified: Thu, 18 Mar 2021 01:46:51 GMT  
		Size: 3.6 MB (3571902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e681b08ea70527a548b97801c95e77bc8b659eb42403b2e6b0840fbea30feb2`  
		Last Modified: Thu, 18 Mar 2021 01:46:51 GMT  
		Size: 9.6 MB (9581188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c465c9354680d18cb16e8e4e72a1bfe1fe89a4faa6ed6d39564231e8d42401`  
		Last Modified: Thu, 18 Mar 2021 01:46:49 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6530b99586fc746ff1892d23c5fba4aedce77bf93506e3a3f8460da5b14b49`  
		Last Modified: Thu, 18 Mar 2021 01:46:50 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-11` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:2485112ff4e5f21ea2a15420a60078be7780f4fb4fffcd24848806d47c7e3386
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.4 MB (221406093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f8687e618205fd83f514e012ec80eb8a6573e97f797a76924cb43d69d9b658d`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 24 Feb 2021 18:44:28 GMT
ADD file:e57e27bb2d338405f702e133eb22bfd61d172471ce8bad647c7f7d9b0b30bf7b in / 
# Wed, 24 Feb 2021 18:44:32 GMT
CMD ["/bin/bash"]
# Wed, 24 Feb 2021 19:35:39 GMT
ARG version=11.0.10.9-1
# Wed, 24 Feb 2021 19:36:08 GMT
# ARGS: version=11.0.10.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 24 Feb 2021 19:36:10 GMT
ENV LANG=C.UTF-8
# Wed, 24 Feb 2021 19:36:10 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Wed, 24 Feb 2021 20:22:00 GMT
ARG MAVEN_VERSION=3.6.3
# Wed, 24 Feb 2021 20:22:01 GMT
ARG USER_HOME_DIR=/root
# Wed, 24 Feb 2021 20:22:02 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Wed, 24 Feb 2021 20:22:02 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Wed, 24 Feb 2021 20:22:14 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Wed, 24 Feb 2021 20:22:17 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 24 Feb 2021 20:22:18 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 24 Feb 2021 20:22:19 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 24 Feb 2021 20:22:19 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 24 Feb 2021 20:22:20 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 24 Feb 2021 20:22:21 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 24 Feb 2021 20:22:21 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:c669744e929468ab3571a83e2386710816116036b648ebd90ecc44d86705b51e`  
		Last Modified: Wed, 24 Feb 2021 18:45:40 GMT  
		Size: 63.6 MB (63624537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc87855b7feac70ec7389ae01e43d02841e30c1d550b99eeb4c599b63471ff1`  
		Last Modified: Wed, 24 Feb 2021 19:38:16 GMT  
		Size: 144.6 MB (144607927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a79ac1a865397b599f57b55b5a96a9d90331b7fa0ab823551eef5c111832e1`  
		Last Modified: Wed, 24 Feb 2021 20:25:08 GMT  
		Size: 3.6 MB (3591220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd368e3b318752fd332797ee1ff76fc56dd03c5fe3899d5c7c0e8d9475fab63`  
		Last Modified: Wed, 24 Feb 2021 20:25:08 GMT  
		Size: 9.6 MB (9581200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9059f04753eec3c50a343af072283421343fcf67d33c4547131e5e966d7d31b5`  
		Last Modified: Wed, 24 Feb 2021 20:25:07 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468830ef11f1e4941afa558ba43714faf9ec4f3749fd06d2aa48feb84065c526`  
		Last Modified: Wed, 24 Feb 2021 20:25:07 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
