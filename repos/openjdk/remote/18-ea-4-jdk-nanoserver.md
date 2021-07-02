## `openjdk:18-ea-4-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:4708ab0efb690474dd36580eb168f88c0fce8e8f44e5ace99f02b72cbcd94337
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `openjdk:18-ea-4-jdk-nanoserver` - windows version 10.0.17763.1999; amd64

```console
$ docker pull openjdk@sha256:aea0f9576004e1a90470841346d0cee6e5f025f43d9b2d6424ab9545b3f2b712
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289274615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19d2abd021bb3cbb071ae9da3b3149f1d1bebace9d4838ceb86009682c4d9342`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 16:52:42 GMT
SHELL [cmd /s /c]
# Mon, 14 Jun 2021 21:23:18 GMT
ENV JAVA_HOME=C:\openjdk-18
# Mon, 14 Jun 2021 21:23:21 GMT
USER ContainerAdministrator
# Mon, 14 Jun 2021 21:23:47 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Mon, 14 Jun 2021 21:23:49 GMT
USER ContainerUser
# Fri, 02 Jul 2021 19:31:33 GMT
ENV JAVA_VERSION=18-ea+4
# Fri, 02 Jul 2021 19:31:51 GMT
COPY dir:9a426469438df1b6e8a60165efb364f20b0a4093f5d057c48f16dc25c5e1e2f8 in C:\openjdk-18 
# Fri, 02 Jul 2021 19:32:13 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Fri, 02 Jul 2021 19:32:15 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:acc28506464ab4d21eaffeb562876f3408463a46d298d12ded7ac0e3dd3c1bd6`  
		Last Modified: Wed, 09 Jun 2021 17:25:28 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a8aa554907fcec99de91851053bfbdcc543f546430c0a1c27a0354cf66ab24`  
		Last Modified: Mon, 14 Jun 2021 21:39:04 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:912c2d7b4763a54931ac01e61f4d52cf9bdfbcb35903c8a29acbc422174b5197`  
		Last Modified: Mon, 14 Jun 2021 21:39:04 GMT  
		Size: 1.1 KB (1072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b175b01ffc1eae821eef4878d9ba8edc445669d64945462f128e7caa1a5cbb3`  
		Last Modified: Mon, 14 Jun 2021 21:39:04 GMT  
		Size: 67.8 KB (67770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696d5b17d363cf6c1471c63b7fc24a3d3c36b15d702a96f0f4ce1cdf249db20f`  
		Last Modified: Mon, 14 Jun 2021 21:39:01 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed8dd3dcc108ff06ddb260dc09bdf78f8ed167421033e49bc91cab9c1054763`  
		Last Modified: Fri, 02 Jul 2021 19:42:49 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5694fd7b5fbe73814c914f8d9840357f16c01d6542fd53a0c6974507c29e09ae`  
		Last Modified: Fri, 02 Jul 2021 19:43:07 GMT  
		Size: 182.9 MB (182878088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f252fa9bad1de791207b0c7e2dc44225db9ba9e290ea94d9caeb1313e00354`  
		Last Modified: Fri, 02 Jul 2021 19:42:50 GMT  
		Size: 3.7 MB (3650729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4ee7a1157309cae7c9b4efeaec1d75a3849c975025725606a1af3442bfbb562`  
		Last Modified: Fri, 02 Jul 2021 19:42:48 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
