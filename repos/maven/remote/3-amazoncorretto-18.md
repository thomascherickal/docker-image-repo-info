## `maven:3-amazoncorretto-18`

```console
$ docker pull maven@sha256:60fa1d8666b969418fda85aacfa6d8f3934b3a4b667f1a741709aa6942c2dae9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-18` - linux; amd64

```console
$ docker pull maven@sha256:464c3d2b4dedf6c637985616cd18e3a31b280661f7d2f58d0387981b701c6382
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.4 MB (227371982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aca813cba723b0b6b7a0c88d9de41b39f6f46f2f04cfa15d8cc02d7d97cad829`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 22 Sep 2022 19:19:21 GMT
ADD file:99847692b0f2dee43b50f306ad92fbc13ccb0541af21c6d3040f72d3184aabac in / 
# Thu, 22 Sep 2022 19:19:21 GMT
CMD ["/bin/bash"]
# Thu, 22 Sep 2022 20:11:28 GMT
ARG version=18.0.2.9-1
# Thu, 22 Sep 2022 20:11:50 GMT
# ARGS: version=18.0.2.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-18-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-18-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 22 Sep 2022 20:11:51 GMT
ENV LANG=C.UTF-8
# Thu, 22 Sep 2022 20:11:51 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-18-amazon-corretto
# Thu, 22 Sep 2022 20:45:23 GMT
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Thu, 22 Sep 2022 20:45:23 GMT
ARG MAVEN_VERSION=3.8.6
# Thu, 22 Sep 2022 20:45:23 GMT
ARG USER_HOME_DIR=/root
# Thu, 22 Sep 2022 20:45:23 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Thu, 22 Sep 2022 20:45:23 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Thu, 22 Sep 2022 20:45:26 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 22 Sep 2022 20:45:26 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 22 Sep 2022 20:45:26 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 22 Sep 2022 20:45:26 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 22 Sep 2022 20:45:26 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 22 Sep 2022 20:45:26 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 22 Sep 2022 20:45:26 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:e80285ff599e329e689e4689be05885456823b7f6233486aa419541ae8e98c62`  
		Last Modified: Wed, 21 Sep 2022 22:07:12 GMT  
		Size: 62.3 MB (62303269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c7563ff25a717e7a3eb2f4b1dbcabfcc1a74f134db85ad74d540cd835d32fef`  
		Last Modified: Thu, 22 Sep 2022 20:16:19 GMT  
		Size: 152.7 MB (152697078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce34326d34fc1c2c529d1cf1b4c8addb9d16e5144c8f4702698df1886c6310b2`  
		Last Modified: Thu, 22 Sep 2022 20:48:45 GMT  
		Size: 3.6 MB (3630924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d34ba9cb18cbd24bb9fe84ad39962cd6fc01d3b5c9d58e30b42e7ca8b2529b`  
		Last Modified: Thu, 22 Sep 2022 20:48:45 GMT  
		Size: 8.7 MB (8739499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb94b6437872e1baecbde47605d63c80c73776291ff68cd2628a427048b9eedb`  
		Last Modified: Thu, 22 Sep 2022 20:48:44 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6289f2daf1686534007832b8b8c802a4b4957d862e60831a386a35d25ef0959f`  
		Last Modified: Thu, 22 Sep 2022 20:48:45 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-18` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:6b8df6daf69c053349c9728933f3f52523dde963c4b53cb150601f61ffe2f620
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.6 MB (227646740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fae223fabaf029701c25d676887b8c234127c7de647485a9937679b8b78ea14b`
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
# Fri, 21 Oct 2022 00:57:56 GMT
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Fri, 21 Oct 2022 00:57:56 GMT
ARG MAVEN_VERSION=3.8.6
# Fri, 21 Oct 2022 00:57:57 GMT
ARG USER_HOME_DIR=/root
# Fri, 21 Oct 2022 00:57:58 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Fri, 21 Oct 2022 00:57:59 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Fri, 21 Oct 2022 00:58:09 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 21 Oct 2022 00:58:10 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 21 Oct 2022 00:58:11 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 21 Oct 2022 00:58:13 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 21 Oct 2022 00:58:14 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 21 Oct 2022 00:58:14 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 21 Oct 2022 00:58:15 GMT
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
	-	`sha256:f3ae53007402dcc0b4df6fab877e10d2b090bca30257222b8af8d1fdd57e3ba5`  
		Last Modified: Fri, 21 Oct 2022 01:02:23 GMT  
		Size: 3.6 MB (3641658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5ff33a8da0ac16cab8075f0678ebbd20030841345bf1476f97f5e4500356b9`  
		Last Modified: Fri, 21 Oct 2022 01:02:23 GMT  
		Size: 8.7 MB (8739466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:188d597555febf9e5c5e7ce319b15dc5c8e3e5321336717913f91199a1f64946`  
		Last Modified: Fri, 21 Oct 2022 01:02:22 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1e96ca701fd6dbab8b9cfcfe5bed3c3db3c5a3b2e0fa44cb8c7aacb7630fa2`  
		Last Modified: Fri, 21 Oct 2022 01:02:22 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
