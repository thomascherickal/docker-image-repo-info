## `maven:amazoncorretto`

```console
$ docker pull maven@sha256:0a627a1ca5970ad660e4d7f1c481fa84b4b38e0cabdbacf0fa4c07d22f03216b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:amazoncorretto` - linux; amd64

```console
$ docker pull maven@sha256:98d0f20380c60ad276e921f64581eb1720d61d3437ba9955bdcbe5c267836d0f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.8 MB (221839516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9169784aef41d0c622ef2d14cbdcd536b06e2f647c8b3f0cd104a2f5b9b5f779`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 04 Feb 2022 23:40:28 GMT
ADD file:871c80292a1347a65a30c9d2cd343d927528a61b8d89fd82f268d5f8ad4d2944 in / 
# Fri, 04 Feb 2022 23:40:29 GMT
CMD ["/bin/bash"]
# Sat, 05 Feb 2022 06:32:30 GMT
ARG version=11.0.14.9-1
# Sat, 05 Feb 2022 06:32:55 GMT
# ARGS: version=11.0.14.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Sat, 05 Feb 2022 06:32:56 GMT
ENV LANG=C.UTF-8
# Sat, 05 Feb 2022 06:32:56 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Mon, 14 Feb 2022 20:25:11 GMT
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Mon, 14 Feb 2022 20:25:12 GMT
ARG MAVEN_VERSION=3.8.4
# Mon, 14 Feb 2022 20:25:12 GMT
ARG USER_HOME_DIR=/root
# Mon, 14 Feb 2022 20:25:12 GMT
ARG SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8
# Mon, 14 Feb 2022 20:25:12 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries
# Mon, 14 Feb 2022 20:25:14 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Mon, 14 Feb 2022 20:25:14 GMT
ENV MAVEN_HOME=/usr/share/maven
# Mon, 14 Feb 2022 20:25:15 GMT
ENV MAVEN_CONFIG=/root/.m2
# Mon, 14 Feb 2022 20:25:15 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Mon, 14 Feb 2022 20:25:15 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Mon, 14 Feb 2022 20:25:15 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Mon, 14 Feb 2022 20:25:15 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:f964900200fc1f8473ac70d9da14cde8bae251ffb4a8f4792e2bf9baf6aaac70`  
		Last Modified: Thu, 27 Jan 2022 23:12:55 GMT  
		Size: 62.2 MB (62237845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c6cf8541f1bf614954d9904dbfc3395eec63297d0f089d94cc13165c458b49`  
		Last Modified: Sat, 05 Feb 2022 06:35:59 GMT  
		Size: 146.9 MB (146871660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adcfec41429d7c2e0e01718ffcc28ac8214b2286effccafa14f3f853088ce6ae`  
		Last Modified: Mon, 14 Feb 2022 20:33:30 GMT  
		Size: 3.6 MB (3618966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d423c86b1686a030cefaff29ced5fae2874a10e85d9dfb47de6f3370017f6d`  
		Last Modified: Mon, 14 Feb 2022 20:33:31 GMT  
		Size: 9.1 MB (9109830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112b24272598fb54137c7a6351de963410c6edddc4092e4735b04952d71a9707`  
		Last Modified: Mon, 14 Feb 2022 20:33:30 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182afe549fd7c9150b6d84fdb9cc791134c582af5238edb85f28be127f5c062c`  
		Last Modified: Mon, 14 Feb 2022 20:33:30 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:amazoncorretto` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:2a1408480a65dfc28d550f4c549e688ee8a572e155f8a56d2ea45979886b82af
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.6 MB (220625779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cb9493e065302bef2919bf8b87a124926e8f2647a653fca826596ecf301fb5e`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 04 Mar 2022 02:54:31 GMT
ADD file:d8fe7ad66f762a8aad81401877fc5d61f1a4b58eac91f47145e6e443aa3ac8ee in / 
# Fri, 04 Mar 2022 02:54:32 GMT
CMD ["/bin/bash"]
# Fri, 04 Mar 2022 03:12:21 GMT
ARG version=11.0.14.9-1
# Fri, 04 Mar 2022 03:12:40 GMT
# ARGS: version=11.0.14.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 04 Mar 2022 03:12:40 GMT
ENV LANG=C.UTF-8
# Fri, 04 Mar 2022 03:12:41 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Fri, 04 Mar 2022 03:32:04 GMT
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Fri, 04 Mar 2022 03:32:05 GMT
ARG MAVEN_VERSION=3.8.4
# Fri, 04 Mar 2022 03:32:06 GMT
ARG USER_HOME_DIR=/root
# Fri, 04 Mar 2022 03:32:07 GMT
ARG SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8
# Fri, 04 Mar 2022 03:32:08 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries
# Fri, 04 Mar 2022 03:32:12 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 04 Mar 2022 03:32:13 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 04 Mar 2022 03:32:14 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 04 Mar 2022 03:32:16 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 04 Mar 2022 03:32:17 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 04 Mar 2022 03:32:17 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 04 Mar 2022 03:32:18 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:12990ee66856745f12f3a508d82e3d48a09d0378d91aaca8ca153c3819e7a686`  
		Last Modified: Thu, 03 Mar 2022 02:21:31 GMT  
		Size: 63.8 MB (63816961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f654940bcc99e1ac80006b2a195711b051e1b2da5aa7f4af2a9b6fd3b06f58d5`  
		Last Modified: Fri, 04 Mar 2022 03:14:32 GMT  
		Size: 144.1 MB (144074025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7adb8d669eaa5012c0e7140c87a159f17f9a34b9690ed39c7a24f1d132b0ee7`  
		Last Modified: Fri, 04 Mar 2022 03:37:23 GMT  
		Size: 3.6 MB (3623803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21089e95d1e2d164fe9b6a555610a1c22a5a955240e429fc3523c7b992c049fd`  
		Last Modified: Fri, 04 Mar 2022 03:37:23 GMT  
		Size: 9.1 MB (9109778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c98baca7f548edeb51136da72daf76d2e1dc3d7d0f5ee770835c019117f4592`  
		Last Modified: Fri, 04 Mar 2022 03:37:22 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0359be8c0cf16d89489739e4ef39b553bb6ab64c9f4062f8951e3b94e16d26`  
		Last Modified: Fri, 04 Mar 2022 03:37:22 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
