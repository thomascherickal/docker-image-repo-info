## `maven:3-amazoncorretto-11`

```console
$ docker pull maven@sha256:ad69ee850532cb0ce66c32e8de314d9a24e28a7b16cc2bc34a021f65d7a1fde1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-11` - linux; amd64

```console
$ docker pull maven@sha256:31ea9180d84100a0623ab8dcabd8ae4abbd4287bb3299767a90fe86117dab112
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **352.8 MB (352794799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa6db1e8831f3e9b68b4bbe513088d2bb85c2f3d5d252516d74198153fd8fea5`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 21 Apr 2020 18:22:56 GMT
ADD file:c64a7d77d1e9f4364c8d2009059cb8668697d61f54f457215b6be6f0c9cded5b in / 
# Tue, 21 Apr 2020 18:22:56 GMT
CMD ["/bin/bash"]
# Tue, 21 Apr 2020 18:51:29 GMT
ARG version=11.0.7.10-1
# Tue, 21 Apr 2020 18:51:52 GMT
# ARGS: version=11.0.7.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && yum install -y fontconfig     && yum clean all
# Tue, 21 Apr 2020 18:51:52 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Tue, 21 Apr 2020 19:20:59 GMT
ARG MAVEN_VERSION=3.6.3
# Tue, 21 Apr 2020 19:20:59 GMT
ARG USER_HOME_DIR=/root
# Tue, 21 Apr 2020 19:21:00 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Tue, 21 Apr 2020 19:21:00 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Tue, 21 Apr 2020 19:21:11 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN yum install -y tar which gzip
# Tue, 21 Apr 2020 19:21:14 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 21 Apr 2020 19:21:14 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 21 Apr 2020 19:21:14 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 21 Apr 2020 19:21:15 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 21 Apr 2020 19:21:15 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Tue, 21 Apr 2020 19:21:15 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 21 Apr 2020 19:21:15 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:a3f8e652bdc470bbea38766fe41f8f12b9e4d44e9ce4037eb502839754b06b9c`  
		Last Modified: Tue, 21 Apr 2020 18:23:48 GMT  
		Size: 61.6 MB (61619066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b8895c8298f706ca1c28f7501761d81a75f5c4c4f92866c8e4953fb2f85f745`  
		Last Modified: Tue, 21 Apr 2020 18:52:41 GMT  
		Size: 197.1 MB (197089493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ac4a86c3a5631a7249ac8f12af1553ce13bdbce0c7b10324fd3e90f177987e`  
		Last Modified: Tue, 21 Apr 2020 19:22:56 GMT  
		Size: 84.5 MB (84503812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000318dd0a282b16b2028f7199eda5c372c17dd61567fe45e0b25aca33a1a9f8`  
		Last Modified: Tue, 21 Apr 2020 19:22:47 GMT  
		Size: 9.6 MB (9581218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:086d88344684ca7ac6de832b73a760c02621ba73e628fd54bf06902850c0199f`  
		Last Modified: Tue, 21 Apr 2020 19:22:46 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fcb1ef1e2a31ddc5c2d0bf3cb41e4d43954c4f15f0e01759e7a050c6229deeb`  
		Last Modified: Tue, 21 Apr 2020 19:22:47 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-11` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:22bb0b03911082dd7e21915b2d60d69ec2c6bbd3cc9616bb14ddde2b3e1001ae
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.7 MB (319706431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf33878bda491589c204c2390fa347ba2aec97f0428443166dc323ec3f17ffef`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 21 Apr 2020 18:58:16 GMT
ADD file:85fc0908f460f80c41755d2b5ab9ff6a025bb2726628ccc4edceb21d2e3f8edf in / 
# Tue, 21 Apr 2020 18:58:18 GMT
CMD ["/bin/bash"]
# Tue, 21 Apr 2020 19:26:46 GMT
ARG version=11.0.7.10-1
# Tue, 21 Apr 2020 19:27:27 GMT
# ARGS: version=11.0.7.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && yum install -y fontconfig     && yum clean all
# Tue, 21 Apr 2020 19:27:29 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Tue, 21 Apr 2020 20:10:35 GMT
ARG MAVEN_VERSION=3.6.3
# Tue, 21 Apr 2020 20:10:36 GMT
ARG USER_HOME_DIR=/root
# Tue, 21 Apr 2020 20:10:37 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Tue, 21 Apr 2020 20:10:38 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Tue, 21 Apr 2020 20:10:54 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN yum install -y tar which gzip
# Tue, 21 Apr 2020 20:11:09 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 21 Apr 2020 20:11:10 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 21 Apr 2020 20:11:11 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 21 Apr 2020 20:11:12 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 21 Apr 2020 20:11:12 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Tue, 21 Apr 2020 20:11:13 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 21 Apr 2020 20:11:14 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:0a37a5cd26f245ce54aff575389ef7765520d37d3ea7c437144c936c6adffc8a`  
		Last Modified: Tue, 21 Apr 2020 18:59:54 GMT  
		Size: 63.1 MB (63079760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64c950fe960e43578caf850fca203e641f2b3deeb231129de3a6803c1538561`  
		Last Modified: Tue, 21 Apr 2020 19:28:58 GMT  
		Size: 195.9 MB (195897191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968c6265639935eb6ec88aa10b0d361c25eea3527d8b18449fd5da8ca8388548`  
		Last Modified: Tue, 21 Apr 2020 20:12:42 GMT  
		Size: 51.1 MB (51147055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f89d4b043083604c524b848b430eeb5422e38df5cc8141d6a7b82abd7e4fac`  
		Last Modified: Tue, 21 Apr 2020 20:12:32 GMT  
		Size: 9.6 MB (9581210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5fe4151f981a190b9a29136ba6275da509e91a595699eec6defa75efe4ca231`  
		Last Modified: Tue, 21 Apr 2020 20:12:30 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827c7ee36236925ab618be5ba951337ec2f0a99bf52145ba2efda23143ae8db9`  
		Last Modified: Tue, 21 Apr 2020 20:12:30 GMT  
		Size: 364.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
