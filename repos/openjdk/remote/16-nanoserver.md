## `openjdk:16-nanoserver`

```console
$ docker pull openjdk@sha256:9a21a31df846c662d4cb7bfd7d54f1875be8e857e371485ac2dd27c7787e6077
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `openjdk:16-nanoserver` - windows version 10.0.17763.1999; amd64

```console
$ docker pull openjdk@sha256:6618fc6173e136c188d1ae736aced44b3bd1f72d342c3d17999f3fa211354a1a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.5 MB (286494571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b016c780080c517e47cd8d887e0ada6864d236da5ef82bed02a5cfa2bd87677`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 16:52:42 GMT
SHELL [cmd /s /c]
# Wed, 09 Jun 2021 16:59:53 GMT
ENV JAVA_HOME=C:\openjdk-16
# Wed, 09 Jun 2021 16:59:55 GMT
USER ContainerAdministrator
# Wed, 09 Jun 2021 17:00:11 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 09 Jun 2021 17:00:13 GMT
USER ContainerUser
# Wed, 09 Jun 2021 17:00:15 GMT
ENV JAVA_VERSION=16.0.1
# Wed, 09 Jun 2021 17:00:34 GMT
COPY dir:ec453f8f02d21eabd8383c9d68e7e854c44e602cce3510b820d8ac55a0745712 in C:\openjdk-16 
# Wed, 09 Jun 2021 17:00:57 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Wed, 09 Jun 2021 17:00:59 GMT
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
	-	`sha256:82c4170444b16e8ecbe8d5c3a4a3ccb3614633ceb5b23f4f92764a6d48f86ff7`  
		Last Modified: Wed, 09 Jun 2021 17:33:40 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04339765859573a45d2b66679d81a72e388592bc708f529587e0948bfbbd9ee0`  
		Last Modified: Wed, 09 Jun 2021 17:33:40 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a004757c4b200af4a6138497ead3bd48fd24c812035ae504393a1e22b3d37b2c`  
		Last Modified: Wed, 09 Jun 2021 17:33:40 GMT  
		Size: 70.7 KB (70697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61025953647318f84ddfedf00f0a6baba26b7e326e129b33b1f1c0f189533c2`  
		Last Modified: Wed, 09 Jun 2021 17:33:37 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de76ca7d333d486e40dff7d8e466abb4f45f8bd77ee6edc19e30ce608bc0c8be`  
		Last Modified: Wed, 09 Jun 2021 17:33:37 GMT  
		Size: 1.1 KB (1105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae05dab41d5aab883331bfcca943a3921e618c5153e9045de25a2bd18a270e4a`  
		Last Modified: Wed, 09 Jun 2021 17:37:06 GMT  
		Size: 180.1 MB (180078935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2f5a8c22e76a5218f09560aef905d13d51873cf0d2aedcc4e2a50f30508af5`  
		Last Modified: Wed, 09 Jun 2021 17:33:38 GMT  
		Size: 3.7 MB (3666583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f509bb13d85ed41baea3f104ae2c384bda40ce65b098d131a70a4c36ecfc47`  
		Last Modified: Wed, 09 Jun 2021 17:33:37 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
