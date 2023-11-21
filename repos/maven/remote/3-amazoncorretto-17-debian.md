## `maven:3-amazoncorretto-17-debian`

```console
$ docker pull maven@sha256:57b5a50e99e1ff081f9539a4b00ee6328fa1810605772ab77c649c233707baf9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-17-debian` - linux; amd64

```console
$ docker pull maven@sha256:4bcf87e0584e83e2c8011922f2248c3654e83bb2daf8fd32dcdaa50f2c1c042e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.3 MB (236346055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f9ec4f6f7c1bf70dbd372a991fb1eebcc04b0c86b4d5d2d847df6ffe010c893`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Thu, 19 Oct 2023 09:04:18 GMT
RUN apt-get update   && apt-get install -y curl gnupg   && export GNUPGHOME="$(mktemp -d)"   && curl -fL https://apt.corretto.aws/corretto.key | gpg --batch --import   && gpg --batch --export '6DC3636DAE534049C8B94623A122542AB04F24E3' > /usr/share/keyrings/corretto.gpg   && rm -r "$GNUPGHOME"   && unset GNUPGHOME   && echo "deb [signed-by=/usr/share/keyrings/corretto.gpg] https://apt.corretto.aws stable main" > /etc/apt/sources.list.d/corretto.list   && apt-get update   && apt-get remove --purge --autoremove -y curl gnupg   && apt-get install -y java-17-amazon-corretto-jdk   && rm -rf /var/lib/apt/lists/* # buildkit
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
	-	`sha256:9e966467b38cccdfb68545d2f33aa75c5105e0495c9e19bed8dc02c557a13e41`  
		Last Modified: Tue, 21 Nov 2023 13:34:57 GMT  
		Size: 197.8 MB (197765261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2c20ef83cc83147029e0e5a3a57411a0f09d61493bfb8960c098a35bcd8fd5`  
		Last Modified: Tue, 21 Nov 2023 13:34:44 GMT  
		Size: 9.4 MB (9429516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55210ee652ac982aba0d39c51edb0962f2c99d7f939eb9b420163934d9e0bbe9`  
		Last Modified: Tue, 21 Nov 2023 13:34:43 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b80206d4060cf2ed2e273299366df835b3975df7b0d4b644b7ea3a99373739`  
		Last Modified: Tue, 21 Nov 2023 13:34:43 GMT  
		Size: 355.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275d75b26542bbbfac7b648607b67a4d4069a02243013d47e9cd62a2a1d62f5c`  
		Last Modified: Tue, 21 Nov 2023 13:34:43 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-17-debian` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:ca1837e8ef303fb9a841c36935c8d36b0244852bbed7a278b21bf1bd76a26b36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.7 MB (234710707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff269eb45fd7080dba4c612a7c176824a4925b321e3bf54289239479894a322d`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Thu, 19 Oct 2023 09:04:18 GMT
RUN apt-get update   && apt-get install -y curl gnupg   && export GNUPGHOME="$(mktemp -d)"   && curl -fL https://apt.corretto.aws/corretto.key | gpg --batch --import   && gpg --batch --export '6DC3636DAE534049C8B94623A122542AB04F24E3' > /usr/share/keyrings/corretto.gpg   && rm -r "$GNUPGHOME"   && unset GNUPGHOME   && echo "deb [signed-by=/usr/share/keyrings/corretto.gpg] https://apt.corretto.aws stable main" > /etc/apt/sources.list.d/corretto.list   && apt-get update   && apt-get remove --purge --autoremove -y curl gnupg   && apt-get install -y java-17-amazon-corretto-jdk   && rm -rf /var/lib/apt/lists/* # buildkit
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
	-	`sha256:a918093cd5a68a168081d7b498735d07116173bb3ef0da24e003c0b230eadd40`  
		Last Modified: Tue, 21 Nov 2023 08:19:54 GMT  
		Size: 196.1 MB (196100551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e7d49fb5f8b9d585ba01c4eed4c8447ecc2e2153002eabbc6af27db03d735b`  
		Last Modified: Tue, 21 Nov 2023 08:19:44 GMT  
		Size: 9.4 MB (9429502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceefc8082c5bd31959ce842448f3ffe403ed88272623e8d910e4c9fbd7c9ea50`  
		Last Modified: Tue, 21 Nov 2023 08:19:43 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5679333b94b98a29b6aed6e3808b217915e6de9eb3027e7a5b6ed8adc6f7ac02`  
		Last Modified: Tue, 21 Nov 2023 08:19:43 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3860ae7fd8a2a626a4898651c3bf761f26b7d62ec6d7f8cfc543743be894caa`  
		Last Modified: Tue, 21 Nov 2023 08:19:43 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
