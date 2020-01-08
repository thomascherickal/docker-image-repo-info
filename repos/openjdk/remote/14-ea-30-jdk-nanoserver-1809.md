## `openjdk:14-ea-30-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:c11e33cfd41b7a13ba4c0cabfaf25bc8ddc54cf7356f4f83a01de43918b4924a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.914; amd64

### `openjdk:14-ea-30-jdk-nanoserver-1809` - windows version 10.0.17763.914; amd64

```console
$ docker pull openjdk@sha256:df4cee819700fe5090a8273d92bff1b425957d9a9ad8f2eb956c047d1900ae4b
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.5 MB (298482439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e0eda6f34071c71ded66879f31b8cc3ea686ae902cded9d140f35167d22bb05`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 28 Nov 2019 13:16:41 GMT
RUN Apply image 1809-amd64
# Wed, 11 Dec 2019 18:49:48 GMT
SHELL [cmd /s /c]
# Wed, 11 Dec 2019 18:49:50 GMT
ENV JAVA_HOME=C:\openjdk-14
# Wed, 11 Dec 2019 18:49:51 GMT
USER ContainerAdministrator
# Wed, 11 Dec 2019 18:50:06 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Wed, 11 Dec 2019 18:50:07 GMT
USER ContainerUser
# Tue, 07 Jan 2020 23:38:42 GMT
ENV JAVA_VERSION=14-ea+30
# Tue, 07 Jan 2020 23:39:42 GMT
COPY dir:4b0191a72f8e091ffdd613e34bd9beb628e72ed6906ece0f0d1de856f1353379 in C:\openjdk-14 
# Tue, 07 Jan 2020 23:40:03 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Tue, 07 Jan 2020 23:40:05 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:1951f408509ba9ddcf240ef5d838c72c5596f97a05b063446508f2ba15d510f2`  
		Size: 101.1 MB (101106116 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:163d55b77f49371136083ba8066ddbec4afad6e1f4fbba77fa4ffebc99a8098a`  
		Last Modified: Wed, 11 Dec 2019 20:01:21 GMT  
		Size: 945.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9326e4caa8f459874d77c281820948a0fa2e558568f484250684f714e368c0bc`  
		Last Modified: Wed, 11 Dec 2019 20:01:19 GMT  
		Size: 953.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07bbc07ec7d9f59279b56946327222e61b8d576bc34eb8b70be4aa88b484d87`  
		Last Modified: Wed, 11 Dec 2019 20:01:19 GMT  
		Size: 944.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c25567424a9bb0685aa9d0cc78a53b800a3447fff914466146890e6bf40dcdd`  
		Last Modified: Wed, 11 Dec 2019 20:01:19 GMT  
		Size: 63.9 KB (63920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6607ef629cd6ba3de9b2b3f57cdc6172ca483c4f285428321d4b04ce9b321db8`  
		Last Modified: Wed, 11 Dec 2019 20:01:16 GMT  
		Size: 949.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c5aa8ba58a2f83813250dec95ae7b4a71a72d0caee06843050b6ef4f6841da`  
		Last Modified: Tue, 07 Jan 2020 23:54:42 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8022b410b6866ae34e23f2f7a9784a55676f19587b77011335f2aa8d2db257fd`  
		Last Modified: Tue, 07 Jan 2020 23:55:10 GMT  
		Size: 193.8 MB (193829948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bac42a1eb1f6b8f1be51eb17196b9d42f599437d98e736885038215e317a3a4`  
		Last Modified: Tue, 07 Jan 2020 23:54:44 GMT  
		Size: 3.5 MB (3476792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843625de8072458777dfd7189e7dc24ac52adbb0b52f363b7de498c9722ff227`  
		Last Modified: Tue, 07 Jan 2020 23:54:42 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
