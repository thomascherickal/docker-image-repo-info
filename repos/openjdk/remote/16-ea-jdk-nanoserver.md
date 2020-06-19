## `openjdk:16-ea-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:8378d6b8dd3cd21f1ba91b1f64d5680b7a0556fee4b26314c98fc35febac2c0a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `openjdk:16-ea-jdk-nanoserver` - windows version 10.0.17763.1282; amd64

```console
$ docker pull openjdk@sha256:48625450a632cc01a68333dd7d3695d5ee4aa47d6fd1738e2469ca96809ed323
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.0 MB (295985812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86c360efb7f899de6be11e2e6d0d868048a6df493998c50dfa92f4a914fb8be0`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 03 Jun 2020 11:12:32 GMT
RUN Apply image 1809-amd64
# Tue, 09 Jun 2020 22:42:44 GMT
SHELL [cmd /s /c]
# Thu, 18 Jun 2020 21:20:54 GMT
ENV JAVA_HOME=C:\openjdk-16
# Thu, 18 Jun 2020 21:20:55 GMT
USER ContainerAdministrator
# Thu, 18 Jun 2020 21:21:11 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Thu, 18 Jun 2020 21:21:11 GMT
USER ContainerUser
# Thu, 18 Jun 2020 21:21:12 GMT
ENV JAVA_VERSION=16-ea+1
# Thu, 18 Jun 2020 21:22:07 GMT
COPY dir:8a29c4e7df6771bf6f3ea27a853c2d4e6c6b9bf4ace58aae89311996bf0156fe in C:\openjdk-16 
# Thu, 18 Jun 2020 21:22:27 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Thu, 18 Jun 2020 21:22:28 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:c7d6d47ff7dfb2aa4d4e819641b93ec971e8541978dff0ffc24c193babeb8c07`  
		Size: 101.0 MB (101043386 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b390ee94e41353252b153770fa99d748992b90bdaf9abf7c785d93be52ee02c`  
		Last Modified: Tue, 09 Jun 2020 23:19:14 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6735890902f0d30df68ef896ea73cd7d60bdd05747cff4957193c1e609fff89a`  
		Last Modified: Thu, 18 Jun 2020 21:28:21 GMT  
		Size: 864.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee48b3407ba988368d7894a7733194fa4aa014b7f58f2d8c7fcaef8e2671a28`  
		Last Modified: Thu, 18 Jun 2020 21:28:21 GMT  
		Size: 876.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6045b891a8218b59a2fddf2b6cac14838a3415c9d2d3092bc26b5e034902d9a`  
		Last Modified: Thu, 18 Jun 2020 21:28:21 GMT  
		Size: 67.2 KB (67242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f442edf533cb5c66c3872015a3894f657674d730051b398dd331afcfe90617`  
		Last Modified: Thu, 18 Jun 2020 21:28:18 GMT  
		Size: 910.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ff8578eef166064a393f476f31fa4b4c22ed8fbf9b2a3be6b28c9f8f80b161`  
		Last Modified: Thu, 18 Jun 2020 21:28:19 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10de05c2268525b0b98bedb1a279480c75e1b44d7c7405ff6aa563b4f0a7e8e3`  
		Last Modified: Thu, 18 Jun 2020 21:28:38 GMT  
		Size: 191.4 MB (191387688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a1bbb169e89bc4616bcea4775b7e2fb4bac20fd617759b7ca0f8e1f36b60f9`  
		Last Modified: Thu, 18 Jun 2020 21:28:19 GMT  
		Size: 3.5 MB (3482200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03da272a37e3d093040b50a728eef6f8cdd728fc4b232402825f960be7035a43`  
		Last Modified: Thu, 18 Jun 2020 21:28:19 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
