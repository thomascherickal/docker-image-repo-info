## `openjdk:17-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:93ad8bf45a821865dae23f3a97146a072c39be572090379a978d64aeb0884206
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `openjdk:17-jdk-nanoserver` - windows version 10.0.17763.1817; amd64

```console
$ docker pull openjdk@sha256:ab0adc795952cd0e6482d0222cbd9259f696e8a508d1b035df0acb8202346e6f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.1 MB (286127987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e322eb55dae470fc162913368e6142aa94e0183008416e8326d93f6b92b6cfa5`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 17:50:47 GMT
SHELL [cmd /s /c]
# Wed, 10 Mar 2021 17:50:48 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 10 Mar 2021 17:50:49 GMT
USER ContainerAdministrator
# Wed, 10 Mar 2021 17:51:08 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 10 Mar 2021 17:51:08 GMT
USER ContainerUser
# Fri, 09 Apr 2021 18:21:59 GMT
ENV JAVA_VERSION=17-ea+17
# Fri, 09 Apr 2021 18:22:18 GMT
COPY dir:9945bfade0f5f62abb3138c090a680fb415eb2c55b5c62ad68275ad248e75a0e in C:\openjdk-17 
# Fri, 09 Apr 2021 18:22:54 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Fri, 09 Apr 2021 18:22:55 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b1146273d9b624ee892dfcbb3c753523f09f79536a16d63b711cb0027825374a`  
		Last Modified: Wed, 10 Mar 2021 18:33:51 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c1ac1e6f2d0594fe7e8e0395310c60461fc8ce5183f6a15db964a07b66176e`  
		Last Modified: Wed, 10 Mar 2021 18:33:51 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050de60c3748a5bfc798f599cadba652e52a162ca31f36b8c783664c11ed224b`  
		Last Modified: Wed, 10 Mar 2021 18:33:54 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e309359702f2d5c4fa7bc854144ad320712050892d017cdfcb58acff4fea2609`  
		Last Modified: Wed, 10 Mar 2021 18:33:50 GMT  
		Size: 66.6 KB (66576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97ecf2dccedb4699a8caf6c19a7a80768c90efb0af5959f1465b00abe8faa12`  
		Last Modified: Wed, 10 Mar 2021 18:33:48 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae35a9fbeabf09b60974b6819a9bc70d2e4e7b17e32f957f3222ae9c14355d7`  
		Last Modified: Fri, 09 Apr 2021 19:27:26 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4a703af259325c5db574fca2c90c5cf3f733c492315608e6e1dc5a6fcc50e5`  
		Last Modified: Fri, 09 Apr 2021 19:27:47 GMT  
		Size: 181.0 MB (181029223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44caed6ed25def153fbd786323b5f81cfffa2bbe241e7e14e88039b5e7f45a72`  
		Last Modified: Fri, 09 Apr 2021 19:27:30 GMT  
		Size: 3.6 MB (3635232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed261db13c0dbd5ea76c065ecf1be0ef075af2b66f463ae9df14db0ba2cc709b`  
		Last Modified: Fri, 09 Apr 2021 19:27:26 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
