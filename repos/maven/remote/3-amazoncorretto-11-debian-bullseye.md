## `maven:3-amazoncorretto-11-debian-bullseye`

```console
$ docker pull maven@sha256:264d2d45769c13f4c9471bac208b87d0b63fa20fb0146c498c1c79d24b315bf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-11-debian-bullseye` - linux; amd64

```console
$ docker pull maven@sha256:12bef69bb310a0d7a460749918a113a41f9cb16ffd5b508a466419daccb79fd1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.2 MB (237223477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8684c90a8946af73d3cd6b4edb19924cc9c0d6bdce68e2013817e603a3c3455`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 26 Apr 2023 19:21:32 GMT
RUN apt-get update   && apt-get install -y curl gnupg   && export GNUPGHOME="$(mktemp -d)"   && curl -fL https://apt.corretto.aws/corretto.key | gpg --batch --import   && gpg --batch --export '6DC3636DAE534049C8B94623A122542AB04F24E3' > /usr/share/keyrings/corretto.gpg   && rm -r "$GNUPGHOME"   && unset GNUPGHOME   && echo "deb [signed-by=/usr/share/keyrings/corretto.gpg] https://apt.corretto.aws stable main" > /etc/apt/sources.list.d/corretto.list   && apt-get update   && apt-get remove --purge --autoremove -y curl gnupg   && apt-get install -y java-11-amazon-corretto-jdk   && rm -rf /var/lib/apt/lists/* # buildkit
# Wed, 26 Apr 2023 19:21:32 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 26 Apr 2023 19:21:32 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Wed, 26 Apr 2023 19:21:32 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Wed, 26 Apr 2023 19:21:32 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Wed, 26 Apr 2023 19:21:32 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Wed, 26 Apr 2023 19:21:32 GMT
ARG MAVEN_VERSION=3.9.1
# Wed, 26 Apr 2023 19:21:32 GMT
ARG USER_HOME_DIR=/root
# Wed, 26 Apr 2023 19:21:32 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 26 Apr 2023 19:21:32 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 26 Apr 2023 19:21:32 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6275ecddd8d56054abb6e93d2f337565cb684e69fb057d2f88259b45a8accb`  
		Last Modified: Sat, 15 Apr 2023 00:27:36 GMT  
		Size: 196.7 MB (196697714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd8a944dab6f62c6b5bfbac41aa380e9a67f12edf6db9ab68b5ee72735eb476`  
		Last Modified: Sat, 15 Apr 2023 00:27:24 GMT  
		Size: 9.1 MB (9106159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ffd0719d769956101c07a11e33378506e0bfb5b72b8c47d8872c677cc8f5150`  
		Last Modified: Sat, 15 Apr 2023 00:27:23 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51741c2254a045011b0a9253de27bfa8f314809c0844e7944e12c36532dc4f1f`  
		Last Modified: Sat, 15 Apr 2023 00:27:23 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09faaf07f7dca0315142fcff395661b25976d314a2b3a79678789c6a65d8916a`  
		Last Modified: Sat, 15 Apr 2023 00:27:23 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-11-debian-bullseye` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:5f7f5f3ec1efc4392649f432d66f6fafffb3812905e469a4ffb41e569c3ccf23
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.0 MB (232983388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac8857d455af23cb227253b31645a091da93083029f87446fb4fe04c7d71e0c1`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 26 Apr 2023 19:40:40 GMT
RUN apt-get update   && apt-get install -y curl gnupg   && export GNUPGHOME="$(mktemp -d)"   && curl -fL https://apt.corretto.aws/corretto.key | gpg --batch --import   && gpg --batch --export '6DC3636DAE534049C8B94623A122542AB04F24E3' > /usr/share/keyrings/corretto.gpg   && rm -r "$GNUPGHOME"   && unset GNUPGHOME   && echo "deb [signed-by=/usr/share/keyrings/corretto.gpg] https://apt.corretto.aws stable main" > /etc/apt/sources.list.d/corretto.list   && apt-get update   && apt-get remove --purge --autoremove -y curl gnupg   && apt-get install -y java-11-amazon-corretto-jdk   && rm -rf /var/lib/apt/lists/* # buildkit
# Wed, 26 Apr 2023 19:40:40 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 26 Apr 2023 19:40:40 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Wed, 26 Apr 2023 19:40:40 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Wed, 26 Apr 2023 19:40:40 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Wed, 26 Apr 2023 19:40:40 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Wed, 26 Apr 2023 19:40:40 GMT
ARG MAVEN_VERSION=3.9.1
# Wed, 26 Apr 2023 19:40:40 GMT
ARG USER_HOME_DIR=/root
# Wed, 26 Apr 2023 19:40:40 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 26 Apr 2023 19:40:40 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 26 Apr 2023 19:40:40 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd20c769dd5c44a68b8ca22d2a8001a74bfd46d6b01db225467cf80674d4253`  
		Last Modified: Sat, 15 Apr 2023 00:45:56 GMT  
		Size: 193.8 MB (193812037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276c012dd6046fdb1b0061b9d748ef2d82bbdcf9539a105b36e4d458d0bf0eef`  
		Last Modified: Sat, 15 Apr 2023 00:45:45 GMT  
		Size: 9.1 MB (9106150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5a25b1d1ac8f34b9c1af4e6e60699381f77b71d12abc17091ade9f0295ea9c`  
		Last Modified: Sat, 15 Apr 2023 00:45:44 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84e783ce599671d0b8e212cf3abd8e382c26734968f4341ea8f852de9dac5db`  
		Last Modified: Sat, 15 Apr 2023 00:45:44 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0d93af3f7dc0c263eae724f1caeaac954009d98ffdbe25fd680de021903370`  
		Last Modified: Sat, 15 Apr 2023 00:45:44 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
