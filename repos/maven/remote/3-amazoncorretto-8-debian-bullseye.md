## `maven:3-amazoncorretto-8-debian-bullseye`

```console
$ docker pull maven@sha256:a675e1381ad5e6c480469c66a4d182a242783aa6b52327ab77f1299a17beadec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-8-debian-bullseye` - linux; amd64

```console
$ docker pull maven@sha256:758f499434eae75d549faee352753802945d2ec5bd0a56f8f670fdb8d5ebb032
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.0 MB (160023029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c177b69b3aadd22cdae3ab614a6ca3bf8016c0d7b77cb8396bddba24f37f0006`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 26 Apr 2023 19:21:32 GMT
RUN apt-get update   && apt-get install -y curl gnupg   && export GNUPGHOME="$(mktemp -d)"   && curl -fL https://apt.corretto.aws/corretto.key | gpg --batch --import   && gpg --batch --export '6DC3636DAE534049C8B94623A122542AB04F24E3' > /usr/share/keyrings/corretto.gpg   && rm -r "$GNUPGHOME"   && unset GNUPGHOME   && echo "deb [signed-by=/usr/share/keyrings/corretto.gpg] https://apt.corretto.aws stable main" > /etc/apt/sources.list.d/corretto.list   && apt-get update   && apt-get remove --purge --autoremove -y curl gnupg   && apt-get install -y java-1.8.0-amazon-corretto-jdk   && rm -rf /var/lib/apt/lists/* # buildkit
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
	-	`sha256:103cac1fd33a918c30fdfaec3839d173741cbe2b77427f1d493bcebabb56b959`  
		Last Modified: Sat, 15 Apr 2023 00:29:38 GMT  
		Size: 119.5 MB (119497257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa86c4c2ca85684a80ea1b22c9d4f009f637d325202835c1d64c74ea2b4112ea`  
		Last Modified: Sat, 15 Apr 2023 00:29:31 GMT  
		Size: 9.1 MB (9106161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925936e670c055cbf8812e2dd4e400f10a8c6bd210f3c76c217a62a9ac6b9ed6`  
		Last Modified: Sat, 15 Apr 2023 00:29:29 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c7c1c0aca589aa874c174590c558c536f00b067bc9bc658a9969c5f6405211f`  
		Last Modified: Sat, 15 Apr 2023 00:29:29 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b094d8aa453b19f16a9f576fe930f7a59163b00202b0f705b4d1f8c76bc0def`  
		Last Modified: Sat, 15 Apr 2023 00:29:29 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-8-debian-bullseye` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:769de0f7ba5cf735eb14b020d47540fc0b90941f1d254634d456811a63da0e4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.6 MB (142620636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41f592071ea825f9b90c10641a8f04d528e914971876ec147e5e746aab5909db`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 00:22:50 GMT
RUN apt-get update   && apt-get install -y curl gnupg   && export GNUPGHOME="$(mktemp -d)"   && curl -fL https://apt.corretto.aws/corretto.key | gpg --batch --import   && gpg --batch --export '6DC3636DAE534049C8B94623A122542AB04F24E3' > /usr/share/keyrings/corretto.gpg   && rm -r "$GNUPGHOME"   && unset GNUPGHOME   && echo "deb [signed-by=/usr/share/keyrings/corretto.gpg] https://apt.corretto.aws stable main" > /etc/apt/sources.list.d/corretto.list   && apt-get update   && apt-get remove --purge --autoremove -y curl gnupg   && apt-get install -y java-1.8.0-amazon-corretto-jdk   && rm -rf /var/lib/apt/lists/* # buildkit
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
	-	`sha256:eb45b4d6424f642b0b69222bec2c002c21337d17bdd9115fb9d95ecf36984ee6`  
		Last Modified: Wed, 03 May 2023 19:46:54 GMT  
		Size: 103.5 MB (103460363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c63cba9d8a53f7f9c04d766313b8b4efc35bdd0c802b09ea9ec5c572831a4a`  
		Last Modified: Wed, 03 May 2023 19:46:48 GMT  
		Size: 9.1 MB (9106165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ea64d3c30a052654031fbdf2ca10df026953d30cae4fb09388699074c57cf1`  
		Last Modified: Wed, 03 May 2023 19:46:47 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867e8a10ec42c4a1964349f59595d99681f12436b6593318eab1f6f0cbc69cb3`  
		Last Modified: Wed, 03 May 2023 19:46:47 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0878c868d2c74e0249716bd64540135724b6c576a592bfc242ea71542280d5f4`  
		Last Modified: Wed, 03 May 2023 19:46:47 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
