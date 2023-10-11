## `eclipse-temurin:11-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:cb51bbe41517ccff48841f4b1598ebef04a9039b1d11ebab152a7953f8243ad0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.2031; amd64
	-	windows version 10.0.17763.4974; amd64

### `eclipse-temurin:11-nanoserver` - windows version 10.0.20348.2031; amd64

```console
$ docker pull eclipse-temurin@sha256:a9e6482103fce6e650c50b4215e2cc84b2aaa83609a56660d7d6f6c445d1c258
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.9 MB (313860657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5659fc791893c465144d7f6e435d174bade342865b4d73d02f6ded65772fb7fe`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 06 Oct 2023 21:30:39 GMT
RUN Apply image 10.0.20348.2031
# Wed, 11 Oct 2023 02:14:39 GMT
SHELL [cmd /s /c]
# Wed, 11 Oct 2023 02:15:48 GMT
ENV JAVA_VERSION=jdk-11.0.20.1+1
# Wed, 11 Oct 2023 02:15:49 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 11 Oct 2023 02:15:50 GMT
USER ContainerAdministrator
# Wed, 11 Oct 2023 02:15:58 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 11 Oct 2023 02:15:59 GMT
USER ContainerUser
# Wed, 11 Oct 2023 02:16:13 GMT
COPY dir:bc17122f89ccac6825b72157f71faf8ee914101def60109a37803e17ec7fe7f6 in C:\openjdk-11 
# Wed, 11 Oct 2023 02:16:26 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 11 Oct 2023 02:16:26 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:fff54800e03713ba81736f43d985319592fc643a1a32b62dbd5c0ec36549de00`  
		Last Modified: Tue, 10 Oct 2023 17:30:43 GMT  
		Size: 120.6 MB (120604344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142fccf33f15e2c503ce4023e2e496d7a99bd036e8b83264772e9dab49c325b3`  
		Last Modified: Wed, 11 Oct 2023 07:29:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5b30c660e7f95ab2f09973c8367da0af150cd9e09bee428e61415cbeafef83`  
		Last Modified: Wed, 11 Oct 2023 07:30:13 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99da9dc14e7b0500712ab9187495d6098529b4967951b59228b07afb096df440`  
		Last Modified: Wed, 11 Oct 2023 07:30:13 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e02f7922ddee5615f25e8c52c728cc5f139aac0be11956f7a7d0074c3747968`  
		Last Modified: Wed, 11 Oct 2023 07:30:13 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6eb8225ff2b985a7ecf4ab61f0858e37359afccb00bb112e6ffc485cf72b5fc`  
		Last Modified: Wed, 11 Oct 2023 07:30:11 GMT  
		Size: 79.6 KB (79631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85dda70c55c8e83cc305bb2d3765daaf5a54aec316b3aff8d16c649e19f7c1cf`  
		Last Modified: Wed, 11 Oct 2023 07:30:11 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bafa02ff7f84c343941558226c6b8017d7e951ee61e1f78af0e57f2149c780`  
		Last Modified: Wed, 11 Oct 2023 07:30:30 GMT  
		Size: 193.1 MB (193107593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:044b488fd1ee2bfdfac13b9bb1d1c351f556245ef98bc2164e10d7017d097b8e`  
		Last Modified: Wed, 11 Oct 2023 07:30:11 GMT  
		Size: 62.2 KB (62191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be619e2337c31180d5dc8c7d98c94a23248d504c3fc51ac14a06617982ecb9e`  
		Last Modified: Wed, 11 Oct 2023 07:30:11 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-nanoserver` - windows version 10.0.17763.4974; amd64

```console
$ docker pull eclipse-temurin@sha256:c5b2534b2d6b42fc798f206926d04df9080b63a5ae1d08380bb1db960eecc5b3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.7 MB (297732688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab75f067a9740ec47908aeb8e2638b72f75bccc787e32815be144badab0e0673`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 01:39:37 GMT
SHELL [cmd /s /c]
# Wed, 11 Oct 2023 01:49:23 GMT
ENV JAVA_VERSION=jdk-11.0.20.1+1
# Wed, 11 Oct 2023 01:49:24 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 11 Oct 2023 01:49:24 GMT
USER ContainerAdministrator
# Wed, 11 Oct 2023 01:49:32 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 11 Oct 2023 01:49:33 GMT
USER ContainerUser
# Wed, 11 Oct 2023 01:49:45 GMT
COPY dir:bc17122f89ccac6825b72157f71faf8ee914101def60109a37803e17ec7fe7f6 in C:\openjdk-11 
# Wed, 11 Oct 2023 01:49:58 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 11 Oct 2023 01:49:59 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5f8edc2588edb9971a52d53cd4265062614ebb25e94063a4d235376797b0e57a`  
		Last Modified: Tue, 10 Oct 2023 17:24:08 GMT  
		Size: 104.5 MB (104464580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c11581d9ee9ea19d58c6cbb415dd809a51b56502169a7a5b301da76d79f63b`  
		Last Modified: Wed, 11 Oct 2023 03:57:05 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79bb5cbcd90cb21698de7c69789381417eaad786834ad21b4d7387014f3e357d`  
		Last Modified: Wed, 11 Oct 2023 07:22:48 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93cc24fa84d82691bd5a980e6c7b024255c6829f71ce64b7f4f93734979cd03`  
		Last Modified: Wed, 11 Oct 2023 07:22:48 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74df6c958ac9563a101d31a35c6a87b7821c26eec9ddaa8b857cf452d3ee6486`  
		Last Modified: Wed, 11 Oct 2023 07:22:48 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38cb4de6d0643b85e9aa6dcbe1b035b2092f56ee00f2f4fd2cc9a5843c78162`  
		Last Modified: Wed, 11 Oct 2023 07:22:46 GMT  
		Size: 65.9 KB (65911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15255fe66122229fa09945bfa11e89e9f85c6c59b0e6885e50fb891fcf98c729`  
		Last Modified: Wed, 11 Oct 2023 07:22:46 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5f3a51dbb0f14d06408e9244c786c4595b86135328abb5440e5f9db019e814`  
		Last Modified: Wed, 11 Oct 2023 07:23:04 GMT  
		Size: 193.1 MB (193107565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba501b0ec4e39e67138f240b7f0db26c37fb198ce41eeb0c7cd780cede007f7`  
		Last Modified: Wed, 11 Oct 2023 07:22:46 GMT  
		Size: 87.7 KB (87744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758144f20f90ef9c8b6436edb159673f0bd85e2312ec2061600b645b0a8025a9`  
		Last Modified: Wed, 11 Oct 2023 07:22:46 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
