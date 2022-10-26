## `maven:3-amazoncorretto-18`

```console
$ docker pull maven@sha256:9d6bcf34001518676d61358485b70382f53ef8619e8c1fccb1c33903caafc355
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-18` - linux; amd64

```console
$ docker pull maven@sha256:1b9bfe76e8538572ff75a89cfef13dc664b4c4cde90985205f581ce2b117988b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.4 MB (227366028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6937b6cec153e040022eda9eb67cdb1b3e4f5fa33d06c24729699dc0b8a091a`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 21 Oct 2022 00:19:49 GMT
ADD file:33ce740675602f8911c110c617b08d74ebe9c26c82226b4815019d8c2d0a2263 in / 
# Fri, 21 Oct 2022 00:19:50 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 01:10:09 GMT
ARG version=18.0.2.9-1
# Fri, 21 Oct 2022 01:10:34 GMT
# ARGS: version=18.0.2.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-18-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-18-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 21 Oct 2022 01:10:35 GMT
ENV LANG=C.UTF-8
# Fri, 21 Oct 2022 01:10:35 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-18-amazon-corretto
# Fri, 21 Oct 2022 02:02:24 GMT
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Fri, 21 Oct 2022 02:02:24 GMT
ARG MAVEN_VERSION=3.8.6
# Fri, 21 Oct 2022 02:02:24 GMT
ARG USER_HOME_DIR=/root
# Fri, 21 Oct 2022 02:02:25 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Fri, 21 Oct 2022 02:02:25 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Fri, 21 Oct 2022 02:02:33 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 21 Oct 2022 02:02:33 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 21 Oct 2022 02:02:33 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 21 Oct 2022 02:02:33 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 21 Oct 2022 02:02:33 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 21 Oct 2022 02:02:33 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 21 Oct 2022 02:02:33 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:e3cfe889ce0a44ace07ec174bd2a7e9022e493956fba0069812a53f81a6040e2`  
		Last Modified: Wed, 19 Oct 2022 18:11:43 GMT  
		Size: 62.3 MB (62306642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fdd810cad0bdf6453bee2dabf5abe8def538559a37f10dd606b86c1a61d9247`  
		Last Modified: Fri, 21 Oct 2022 01:15:45 GMT  
		Size: 152.7 MB (152698907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6be694ed44843398d93b774f866c3e735cd4e8e2933063ece9e1fae01ad65f`  
		Last Modified: Fri, 21 Oct 2022 02:05:41 GMT  
		Size: 3.6 MB (3619753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d6310748bf4f3b0278bab92a0e7259bd2d628b52e6bcbd600cfec7c140ce0f1`  
		Last Modified: Fri, 21 Oct 2022 02:05:41 GMT  
		Size: 8.7 MB (8739514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10170ff4e45e3dd2e3891896ff3103e5a12a6f66535879fe656d243f999e88aa`  
		Last Modified: Fri, 21 Oct 2022 02:05:40 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e10688a22756eacdb4385f8a99fcd4cbd13893b0dabf53f47ed3eab90c24bf`  
		Last Modified: Fri, 21 Oct 2022 02:05:40 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-18` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:3c3c3ff5c140a2d12f46f78de3366f932baebb988af0d7f147357368c75da505
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.6 MB (227647789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faffc4083ffb6db6ed6ba420b41bc25ecbff68d76d4c54c8e7fe1d84e3068e51`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 20 Oct 2022 23:39:31 GMT
ADD file:45362bc0bb55d35f704a938eb431f8accb86d1bb8e52b78f3ef34eb141c3ed82 in / 
# Thu, 20 Oct 2022 23:39:32 GMT
CMD ["/bin/bash"]
# Thu, 20 Oct 2022 23:57:52 GMT
ARG version=18.0.2.9-1
# Thu, 20 Oct 2022 23:58:04 GMT
# ARGS: version=18.0.2.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-18-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-18-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 20 Oct 2022 23:58:05 GMT
ENV LANG=C.UTF-8
# Thu, 20 Oct 2022 23:58:06 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-18-amazon-corretto
# Wed, 26 Oct 2022 15:20:26 GMT
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Wed, 26 Oct 2022 15:20:26 GMT
ARG MAVEN_VERSION=3.8.6
# Wed, 26 Oct 2022 15:20:26 GMT
ARG USER_HOME_DIR=/root
# Wed, 26 Oct 2022 15:20:26 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Wed, 26 Oct 2022 15:20:26 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Wed, 26 Oct 2022 15:20:28 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 26 Oct 2022 15:20:28 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 26 Oct 2022 15:20:28 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 26 Oct 2022 15:20:28 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 26 Oct 2022 15:20:28 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 26 Oct 2022 15:20:28 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 26 Oct 2022 15:20:28 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:d900cba9f9f55565485a1181c89317c2718b6232095971d67af440a33db15594`  
		Last Modified: Wed, 19 Oct 2022 18:11:20 GMT  
		Size: 63.9 MB (63919869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5d79b74e04609c53b3251846bbfc91daae1e1e0143fa7547e36c706d8b4c63c`  
		Last Modified: Fri, 21 Oct 2022 00:01:21 GMT  
		Size: 151.3 MB (151344534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad2f96153728af32b52ef2c3bcee44cebc05ea298ed9b6dfed850bf0af3da1f`  
		Last Modified: Wed, 26 Oct 2022 15:26:19 GMT  
		Size: 3.6 MB (3642668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6e45e7ab6d93837f402c21090cfa2f704554112af8e479c4fc889d15446ca6`  
		Last Modified: Wed, 26 Oct 2022 15:26:20 GMT  
		Size: 8.7 MB (8739510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442bb3c0353f8a377e66eaee70be4d4916eca91c8fbbbe2524e27f8f824fe09f`  
		Last Modified: Wed, 26 Oct 2022 15:26:18 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4593b00be7e0f4279cffded7c3e04b5303642c63d1cf011e7064c2bbe1d68b0a`  
		Last Modified: Wed, 26 Oct 2022 15:26:18 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
