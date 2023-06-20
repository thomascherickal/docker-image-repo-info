## `maven:3-amazoncorretto-8-debian`

```console
$ docker pull maven@sha256:1e557ae053409f4d5035b733b7380b4617754586c205491e3e4dfec37d286d0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-8-debian` - linux; amd64

```console
$ docker pull maven@sha256:7af9b8b4818ab89fe9bc053040e722541581b1b59c8029427a04300d9099d719
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.3 MB (160337698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07ca276f3f982ee1932a92345b4971c3817a841e740c0d4b0f59b8f7743651da`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:42 GMT
ADD file:ba1250b6ecd5dd09d4914189d72741c2817988994e7da514bf62be439a34bdb5 in / 
# Mon, 12 Jun 2023 23:20:42 GMT
CMD ["bash"]
# Sat, 17 Jun 2023 08:38:16 GMT
RUN apt-get update   && apt-get install -y curl gnupg   && export GNUPGHOME="$(mktemp -d)"   && curl -fL https://apt.corretto.aws/corretto.key | gpg --batch --import   && gpg --batch --export '6DC3636DAE534049C8B94623A122542AB04F24E3' > /usr/share/keyrings/corretto.gpg   && rm -r "$GNUPGHOME"   && unset GNUPGHOME   && echo "deb [signed-by=/usr/share/keyrings/corretto.gpg] https://apt.corretto.aws stable main" > /etc/apt/sources.list.d/corretto.list   && apt-get update   && apt-get remove --purge --autoremove -y curl gnupg   && apt-get install -y java-1.8.0-amazon-corretto-jdk   && rm -rf /var/lib/apt/lists/* # buildkit
# Sat, 17 Jun 2023 08:38:16 GMT
ENV MAVEN_HOME=/usr/share/maven
# Sat, 17 Jun 2023 08:38:16 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Sat, 17 Jun 2023 08:38:16 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Sat, 17 Jun 2023 08:38:16 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Sat, 17 Jun 2023 08:38:16 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Sat, 17 Jun 2023 08:38:16 GMT
ARG MAVEN_VERSION=3.9.2
# Sat, 17 Jun 2023 08:38:16 GMT
ARG USER_HOME_DIR=/root
# Sat, 17 Jun 2023 08:38:16 GMT
ENV MAVEN_CONFIG=/root/.m2
# Sat, 17 Jun 2023 08:38:16 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Sat, 17 Jun 2023 08:38:16 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:5b5fe70539cd6989aa19f25826309f9715a9489cf1c057982d6a84c1ad8975c7`  
		Last Modified: Mon, 12 Jun 2023 23:25:49 GMT  
		Size: 29.1 MB (29124744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da994f298c5af7a0d18367bd8159714302efa6c9a3e9fba1555a81a935b51a6c`  
		Last Modified: Tue, 20 Jun 2023 22:46:50 GMT  
		Size: 121.9 MB (121897148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fcc891f85312726a741baf75e8ccbf7c7a861aa1818c4a3cec0533aabc35eb6`  
		Last Modified: Tue, 20 Jun 2023 22:46:42 GMT  
		Size: 9.3 MB (9314426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b4705eb5f5f1494fbb15aef428d35d673a1aa2bd66cd8c362401920fde045f`  
		Last Modified: Tue, 20 Jun 2023 22:46:41 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1a821a4178fb9b98dac0c90b9fdeca823c9b33e6dcaf05a6c588d2074a0789`  
		Last Modified: Tue, 20 Jun 2023 22:46:41 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15da565be7a7fcb154b08ccc0fb0030ee1f6720ce1b00d791c6ace270ba11fb`  
		Last Modified: Tue, 20 Jun 2023 22:46:41 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-8-debian` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:efaa86bd43ec99663ae9b0bcabd910c12e4fe0aaabe0e31a1f7667e6cb9eef9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.2 MB (144174517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8879a6552d420e5b6fd60fcbead547d1ba958542ecae396d0dfd4323e8066e3a`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:13 GMT
ADD file:f75c3fe22fec548b35a86a9a5802fdc97497f5d253cf630d65f13282169d3f3f in / 
# Mon, 12 Jun 2023 23:40:14 GMT
CMD ["bash"]
# Sat, 17 Jun 2023 08:38:16 GMT
RUN apt-get update   && apt-get install -y curl gnupg   && export GNUPGHOME="$(mktemp -d)"   && curl -fL https://apt.corretto.aws/corretto.key | gpg --batch --import   && gpg --batch --export '6DC3636DAE534049C8B94623A122542AB04F24E3' > /usr/share/keyrings/corretto.gpg   && rm -r "$GNUPGHOME"   && unset GNUPGHOME   && echo "deb [signed-by=/usr/share/keyrings/corretto.gpg] https://apt.corretto.aws stable main" > /etc/apt/sources.list.d/corretto.list   && apt-get update   && apt-get remove --purge --autoremove -y curl gnupg   && apt-get install -y java-1.8.0-amazon-corretto-jdk   && rm -rf /var/lib/apt/lists/* # buildkit
# Sat, 17 Jun 2023 08:38:16 GMT
ENV MAVEN_HOME=/usr/share/maven
# Sat, 17 Jun 2023 08:38:16 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Sat, 17 Jun 2023 08:38:16 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Sat, 17 Jun 2023 08:38:16 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Sat, 17 Jun 2023 08:38:16 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Sat, 17 Jun 2023 08:38:16 GMT
ARG MAVEN_VERSION=3.9.2
# Sat, 17 Jun 2023 08:38:16 GMT
ARG USER_HOME_DIR=/root
# Sat, 17 Jun 2023 08:38:16 GMT
ENV MAVEN_CONFIG=/root/.m2
# Sat, 17 Jun 2023 08:38:16 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Sat, 17 Jun 2023 08:38:16 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:95039a22a7cc3ae41d71f075e6e09e91e8da850fb5f80aba2f4a09f254520539`  
		Last Modified: Mon, 12 Jun 2023 23:44:08 GMT  
		Size: 29.2 MB (29152534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d837f34cc88c39a31ec0ce051f555bd32609987d1cbc01297e96ee883f37a1`  
		Last Modified: Tue, 20 Jun 2023 23:03:40 GMT  
		Size: 105.7 MB (105706194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c16f298ea2b9db7cb85b0aa7af40d41bec0d025ff7209d5697f1f9073fcbad`  
		Last Modified: Tue, 20 Jun 2023 23:03:33 GMT  
		Size: 9.3 MB (9314414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f877a67a48f1d4e1c436c0be96ff17b47d576b09ab58d30eb06a2622d27ede`  
		Last Modified: Tue, 20 Jun 2023 23:03:32 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836186f2aa07281ee69e43f66e254ca47bb7e67ae4ba47af48e88acd2175a5fd`  
		Last Modified: Tue, 20 Jun 2023 23:03:33 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d47f15fed6fdf442a440befdd51051b2961f3888b05631eb62f551854d2280b`  
		Last Modified: Tue, 20 Jun 2023 23:03:32 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
