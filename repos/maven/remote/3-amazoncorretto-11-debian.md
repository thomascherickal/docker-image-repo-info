## `maven:3-amazoncorretto-11-debian`

```console
$ docker pull maven@sha256:1bed34c8d9111c7b02958844be60610abf248c7004dee146f8681a7cd01a5632
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-11-debian` - linux; amd64

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

### `maven:3-amazoncorretto-11-debian` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:096ebaba5efccc44b0cf2fcdc2c8ef3aa6209fb8f4892f7674a8751d95f9f6ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.0 MB (232960330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03ff8f12f696e3e4ced5edc0fbc5337fa48849d7b91f37039d376bd03ebe24ac`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 00:22:50 GMT
RUN apt-get update   && apt-get install -y curl gnupg   && export GNUPGHOME="$(mktemp -d)"   && curl -fL https://apt.corretto.aws/corretto.key | gpg --batch --import   && gpg --batch --export '6DC3636DAE534049C8B94623A122542AB04F24E3' > /usr/share/keyrings/corretto.gpg   && rm -r "$GNUPGHOME"   && unset GNUPGHOME   && echo "deb [signed-by=/usr/share/keyrings/corretto.gpg] https://apt.corretto.aws stable main" > /etc/apt/sources.list.d/corretto.list   && apt-get update   && apt-get remove --purge --autoremove -y curl gnupg   && apt-get install -y java-11-amazon-corretto-jdk   && rm -rf /var/lib/apt/lists/* # buildkit
# Wed, 03 May 2023 00:22:50 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 03 May 2023 00:22:50 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Wed, 03 May 2023 00:22:50 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Wed, 03 May 2023 00:22:50 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Wed, 03 May 2023 00:22:50 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Wed, 03 May 2023 00:22:50 GMT
ARG MAVEN_VERSION=3.9.1
# Wed, 03 May 2023 00:22:50 GMT
ARG USER_HOME_DIR=/root
# Wed, 03 May 2023 00:22:50 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 03 May 2023 00:22:50 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 03 May 2023 00:22:50 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac533b7d78e0df7450630815064f67a7608408f9c23a341f451e4d2101578bb`  
		Last Modified: Wed, 03 May 2023 19:45:05 GMT  
		Size: 193.8 MB (193800065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e92ca0a684d61fc5c28fafe7b0508bec113a1c387dbf24c6ca0b5bd56130172`  
		Last Modified: Wed, 03 May 2023 19:44:55 GMT  
		Size: 9.1 MB (9106156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6110a0fe7cc85767d36b11b75ce0aae0da7035acaece61f7f7ca570ce54031`  
		Last Modified: Wed, 03 May 2023 19:44:54 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec00068cb7ad47ae1b5571f77cc0b10f308b5694756636d872fc00975665f3d`  
		Last Modified: Wed, 03 May 2023 19:44:54 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdaa52f8d95c2024e374c3cf371987aecdab1bd641f020828823f56b051fad0f`  
		Last Modified: Wed, 03 May 2023 19:44:54 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
