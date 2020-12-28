## `openjdk:17-nanoserver`

```console
$ docker pull openjdk@sha256:8b454545673904462afb33bf0c01ae14ff5c027b3ee3bd145b396f93473ff658
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `openjdk:17-nanoserver` - windows version 10.0.17763.1637; amd64

```console
$ docker pull openjdk@sha256:c2250aa46db56158b93a7cd39fcd83d1f13c6417d8fb4caf37a7cf935953d6d1
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.3 MB (286274774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8668f7d793fe47c6bfc8d102a42a3371a8ea49cdcb38255bbc1249ccf1ff067c`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 03 Dec 2020 08:05:47 GMT
RUN Apply image 1809-amd64
# Wed, 09 Dec 2020 18:58:23 GMT
SHELL [cmd /s /c]
# Mon, 28 Dec 2020 21:51:26 GMT
ENV JAVA_HOME=C:\openjdk-17
# Mon, 28 Dec 2020 21:51:26 GMT
USER ContainerAdministrator
# Mon, 28 Dec 2020 21:51:37 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Mon, 28 Dec 2020 21:51:38 GMT
USER ContainerUser
# Mon, 28 Dec 2020 21:51:38 GMT
ENV JAVA_VERSION=17-ea+3
# Mon, 28 Dec 2020 21:52:13 GMT
COPY dir:ac0f69724fc6d98bdc88b341826ad988ebfb3eff56ad28893560a74f7eee0886 in C:\openjdk-17 
# Mon, 28 Dec 2020 21:52:41 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Mon, 28 Dec 2020 21:52:42 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:21be49aa856f07be4e0a677b988e43c04bd595a3c858e58b6c364477bbbf7222`  
		Size: 101.3 MB (101264827 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fe9a51a0164bd1c063cbda08c4e22dc4f5d04a8047a3951d7441f37fb93c57f2`  
		Last Modified: Wed, 09 Dec 2020 19:34:04 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b80aa1b697da500ba4c274df29d7d303143a959d616d7e5a4beedfbedf5cf7`  
		Last Modified: Mon, 28 Dec 2020 22:02:59 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7ce0b0fafcb9f312707c293e822c52606813545fdf01717b420b72e20faad3c`  
		Last Modified: Mon, 28 Dec 2020 22:02:58 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4721418f9519ff146e3e520e2b942e21b0f4b1a06863f2b3de99c48542b9cdbb`  
		Last Modified: Mon, 28 Dec 2020 22:02:59 GMT  
		Size: 66.0 KB (65967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b38aab677d2fe5ff72b09e4f69954a90189cd63516578596920b168c901728`  
		Last Modified: Mon, 28 Dec 2020 22:02:55 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50821a6cfcaa859af8d9d8ff61fbef51f7d1f0fa024ea7669e4e6ae672316f3`  
		Last Modified: Mon, 28 Dec 2020 22:02:55 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3766cc76418e865b25b28fde5b8931ebf619868e6155278812b6652ad6555ae6`  
		Last Modified: Mon, 28 Dec 2020 22:03:16 GMT  
		Size: 181.2 MB (181242635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a093441b1db5b8501cad9e4455eff6e88540023f10d846acffb0e1e4a19c347a`  
		Last Modified: Mon, 28 Dec 2020 22:02:57 GMT  
		Size: 3.7 MB (3696100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad6cbda0df7ac50b3f6b0c018e301006ef84d957dd6c8910795d11a08eee672`  
		Last Modified: Mon, 28 Dec 2020 22:02:56 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
