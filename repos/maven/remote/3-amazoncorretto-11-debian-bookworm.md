## `maven:3-amazoncorretto-11-debian-bookworm`

```console
$ docker pull maven@sha256:2f4489e21efe88022d67458bd752db2f3827204f2036411a1e6bc91cabe86d84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-11-debian-bookworm` - linux; amd64

```console
$ docker pull maven@sha256:0b11cec4f2f7b080d6dc91f710f9dc8459997f007681ed1631f6d255ca057ba7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.9 MB (237881678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06091b78344f0825efad4000755c3b76bfa5d62e9d82b078e12e27daaaed6d98`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Thu, 19 Oct 2023 09:04:18 GMT
RUN apt-get update   && apt-get install -y curl gnupg   && export GNUPGHOME="$(mktemp -d)"   && curl -fL https://apt.corretto.aws/corretto.key | gpg --batch --import   && gpg --batch --export '6DC3636DAE534049C8B94623A122542AB04F24E3' > /usr/share/keyrings/corretto.gpg   && rm -r "$GNUPGHOME"   && unset GNUPGHOME   && echo "deb [signed-by=/usr/share/keyrings/corretto.gpg] https://apt.corretto.aws stable main" > /etc/apt/sources.list.d/corretto.list   && apt-get update   && apt-get remove --purge --autoremove -y curl gnupg   && apt-get install -y java-11-amazon-corretto-jdk   && rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 19 Oct 2023 09:04:18 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 19 Oct 2023 09:04:18 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Thu, 19 Oct 2023 09:04:18 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Thu, 19 Oct 2023 09:04:18 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Thu, 19 Oct 2023 09:04:18 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Thu, 19 Oct 2023 09:04:18 GMT
ARG MAVEN_VERSION=3.9.5
# Thu, 19 Oct 2023 09:04:18 GMT
ARG USER_HOME_DIR=/root
# Thu, 19 Oct 2023 09:04:18 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 19 Oct 2023 09:04:18 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 19 Oct 2023 09:04:18 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd124f96dd28886747affbd22c9f50ac1f01efd5a29a089231d6e1225181c07`  
		Last Modified: Tue, 21 Nov 2023 13:34:22 GMT  
		Size: 199.3 MB (199300891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12917f89030a72c9938e60f8c4a378f88cf8216bbdd9b084ed94cf0e85f344f`  
		Last Modified: Tue, 21 Nov 2023 13:34:10 GMT  
		Size: 9.4 MB (9429504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689b0130da64723ccf06f3e8a6b9e789e0a771aa708c32e07433eb7a08905774`  
		Last Modified: Tue, 21 Nov 2023 13:34:09 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3d9075194d039750dfdfaf88ed6366c5eb6df5ef2a4707daedcb0298733456`  
		Last Modified: Tue, 21 Nov 2023 13:34:09 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8f465745df98b1235c709b7e33a1742ffdec8ce1ef8e3aed760c9f09c65d1f`  
		Last Modified: Tue, 21 Nov 2023 13:34:09 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-11-debian-bookworm` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:77ec15622b577e3a334cbc3a22d5ecc95451c76bd71521b9491943d0f23c2493
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.8 MB (234761372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1a5f60bf569559054d6380887404e1eb3a0da97b7c56d32ef5f8190bcb05c19`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Thu, 19 Oct 2023 09:04:18 GMT
RUN apt-get update   && apt-get install -y curl gnupg   && export GNUPGHOME="$(mktemp -d)"   && curl -fL https://apt.corretto.aws/corretto.key | gpg --batch --import   && gpg --batch --export '6DC3636DAE534049C8B94623A122542AB04F24E3' > /usr/share/keyrings/corretto.gpg   && rm -r "$GNUPGHOME"   && unset GNUPGHOME   && echo "deb [signed-by=/usr/share/keyrings/corretto.gpg] https://apt.corretto.aws stable main" > /etc/apt/sources.list.d/corretto.list   && apt-get update   && apt-get remove --purge --autoremove -y curl gnupg   && apt-get install -y java-11-amazon-corretto-jdk   && rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 19 Oct 2023 09:04:18 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 19 Oct 2023 09:04:18 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Thu, 19 Oct 2023 09:04:18 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Thu, 19 Oct 2023 09:04:18 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Thu, 19 Oct 2023 09:04:18 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Thu, 19 Oct 2023 09:04:18 GMT
ARG MAVEN_VERSION=3.9.5
# Thu, 19 Oct 2023 09:04:18 GMT
ARG USER_HOME_DIR=/root
# Thu, 19 Oct 2023 09:04:18 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 19 Oct 2023 09:04:18 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 19 Oct 2023 09:04:18 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041fc86ad1aabd905d70457415de19d70040bc257d7a81d831f453b7810e5f3b`  
		Last Modified: Tue, 21 Nov 2023 08:19:25 GMT  
		Size: 196.2 MB (196151219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f57d8a569aab8b7777e8d84d72c748c819b8bb52e03258a006430af558e335`  
		Last Modified: Tue, 21 Nov 2023 08:19:15 GMT  
		Size: 9.4 MB (9429502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052032517de03bf9aec56394652d0f8078460396f2ef2ce96b05550dc662894e`  
		Last Modified: Tue, 21 Nov 2023 08:19:14 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0753623cc46816e0ec163c52c1a9cf4a90644bd3cf48187be7471c81b11aea`  
		Last Modified: Tue, 21 Nov 2023 08:19:14 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f0127e17d05e8c963ed45fd45187b3f0bd71e31d82c5d090fee345b03329db`  
		Last Modified: Tue, 21 Nov 2023 08:19:14 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
