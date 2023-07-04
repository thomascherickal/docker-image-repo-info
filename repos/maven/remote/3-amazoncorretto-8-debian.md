## `maven:3-amazoncorretto-8-debian`

```console
$ docker pull maven@sha256:11c2ef9ba794f85fff21f8c8c0c259a28f41e9b106ed5e92dd263afc96e7088a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-8-debian` - linux; amd64

```console
$ docker pull maven@sha256:60565f6c184803808c912157c74f8c1692ab379471c9b3b3734483b41d7178da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.4 MB (160351049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af3436e768c3032eb076fff5839ebb90634b99cabbd637c888c6140a3ccfed32`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:58 GMT
ADD file:bd80a4461150784e5f2f5a1faa720cc347ad3e30ee0969adbfad574c316f5aef in / 
# Tue, 04 Jul 2023 01:19:58 GMT
CMD ["bash"]
# Mon, 26 Jun 2023 13:48:06 GMT
RUN apt-get update   && apt-get install -y curl gnupg   && export GNUPGHOME="$(mktemp -d)"   && curl -fL https://apt.corretto.aws/corretto.key | gpg --batch --import   && gpg --batch --export '6DC3636DAE534049C8B94623A122542AB04F24E3' > /usr/share/keyrings/corretto.gpg   && rm -r "$GNUPGHOME"   && unset GNUPGHOME   && echo "deb [signed-by=/usr/share/keyrings/corretto.gpg] https://apt.corretto.aws stable main" > /etc/apt/sources.list.d/corretto.list   && apt-get update   && apt-get remove --purge --autoremove -y curl gnupg   && apt-get install -y java-1.8.0-amazon-corretto-jdk   && rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
ENV MAVEN_HOME=/usr/share/maven
# Mon, 26 Jun 2023 13:48:06 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
ARG MAVEN_VERSION=3.9.3
# Mon, 26 Jun 2023 13:48:06 GMT
ARG USER_HOME_DIR=/root
# Mon, 26 Jun 2023 13:48:06 GMT
ENV MAVEN_CONFIG=/root/.m2
# Mon, 26 Jun 2023 13:48:06 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Mon, 26 Jun 2023 13:48:06 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:faef57eae888cbe4a5613eca6741b5e48d768b83f6088858aee9a5a2834f8151`  
		Last Modified: Tue, 04 Jul 2023 01:25:03 GMT  
		Size: 29.1 MB (29124829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8b9c181308a5e4df7c026da93d6d879611826ee10a08d319c37a1c07c478c9`  
		Last Modified: Tue, 04 Jul 2023 12:56:16 GMT  
		Size: 121.9 MB (121897283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb6061ce30068d711134b194719a85e919f4841241d4ce736379c30ea6b84bb`  
		Last Modified: Tue, 04 Jul 2023 12:56:08 GMT  
		Size: 9.3 MB (9327560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b73c558b58d2c649729cf189767f0111cace78b160b7843123121b8d788dec`  
		Last Modified: Tue, 04 Jul 2023 12:56:07 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94001d24726f434108ca810b6e86ba22d80a9d96a7f4fc18a1ee658494033774`  
		Last Modified: Tue, 04 Jul 2023 12:56:07 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556fd8477c3120606318c22f7b0e91bf553ebc63a2c9a6031d985d7c67608980`  
		Last Modified: Tue, 04 Jul 2023 12:56:07 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-8-debian` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:e38e5ebafc541af62605084ea4eb4a9288eb3b0ab0eb8f92b4edcfdefe228c3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.2 MB (144187579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73d9fd67a0b79f80d1fb8328a159d7f6de1b33a83c45f71476c35d2be6dd44ae`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:35 GMT
ADD file:71fd66666294148382f2e6a09ae5e277d4c4e9c74402ab64b693a79387b67a09 in / 
# Tue, 04 Jul 2023 01:57:36 GMT
CMD ["bash"]
# Mon, 26 Jun 2023 13:48:06 GMT
RUN apt-get update   && apt-get install -y curl gnupg   && export GNUPGHOME="$(mktemp -d)"   && curl -fL https://apt.corretto.aws/corretto.key | gpg --batch --import   && gpg --batch --export '6DC3636DAE534049C8B94623A122542AB04F24E3' > /usr/share/keyrings/corretto.gpg   && rm -r "$GNUPGHOME"   && unset GNUPGHOME   && echo "deb [signed-by=/usr/share/keyrings/corretto.gpg] https://apt.corretto.aws stable main" > /etc/apt/sources.list.d/corretto.list   && apt-get update   && apt-get remove --purge --autoremove -y curl gnupg   && apt-get install -y java-1.8.0-amazon-corretto-jdk   && rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
ENV MAVEN_HOME=/usr/share/maven
# Mon, 26 Jun 2023 13:48:06 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
ARG MAVEN_VERSION=3.9.3
# Mon, 26 Jun 2023 13:48:06 GMT
ARG USER_HOME_DIR=/root
# Mon, 26 Jun 2023 13:48:06 GMT
ENV MAVEN_CONFIG=/root/.m2
# Mon, 26 Jun 2023 13:48:06 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Mon, 26 Jun 2023 13:48:06 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:3ae0c06b4d3aa97d7e0829233dd36cea1666b87074e55fea6bd1ecae066693c7`  
		Last Modified: Tue, 04 Jul 2023 02:01:20 GMT  
		Size: 29.2 MB (29152458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b4facb21a406419b99640d49ead72043d12688abe7a626adb7dc58e06c6976`  
		Last Modified: Tue, 04 Jul 2023 06:34:02 GMT  
		Size: 105.7 MB (105706177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0286e7fc9c206badbe9be0ae15079f7532dfc39d5fa30329988e1938a8fe6358`  
		Last Modified: Tue, 04 Jul 2023 06:33:55 GMT  
		Size: 9.3 MB (9327566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e355351b431aaf4fd40323ae9ddd3142b36b1d37ead6d9e73f995e2a58f4f1`  
		Last Modified: Tue, 04 Jul 2023 06:33:55 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834e6706efc97927afc03601bd6fad90f31a89f36b86e1f9f7ce59aba81d0e2a`  
		Last Modified: Tue, 04 Jul 2023 06:33:55 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ec57076064d6c69d20bc9965e364cec08c498b03bd96b7b9aed4225ffd6d67`  
		Last Modified: Tue, 04 Jul 2023 06:33:55 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
