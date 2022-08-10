## `openjdk:18-nanoserver-1809`

```console
$ docker pull openjdk@sha256:5973a553e8d1915fcdfb3700618798dac8396d1cf50f5734d311e26c023b7048
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `openjdk:18-nanoserver-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull openjdk@sha256:0c6c0dd3d9ae115465ef1be3f359c0d09c40edf61d0be482be62101a0f2b74c1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.0 MB (291022808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:932dfc452d6d20a910762eb8080fedf07b9bacc0140d27d3586f9f40f45602e1`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 06 Aug 2022 18:08:38 GMT
RUN Apply image 10.0.17763.3287
# Wed, 10 Aug 2022 15:57:07 GMT
SHELL [cmd /s /c]
# Wed, 10 Aug 2022 17:09:37 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 10 Aug 2022 17:09:38 GMT
USER ContainerAdministrator
# Wed, 10 Aug 2022 17:09:48 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 10 Aug 2022 17:09:48 GMT
USER ContainerUser
# Wed, 10 Aug 2022 17:09:49 GMT
ENV JAVA_VERSION=18.0.2
# Wed, 10 Aug 2022 17:10:06 GMT
COPY dir:1a22cafd1c3a73c07e75460ef8cc20669902f9a162797035a29e2b4c98b82396 in C:\openjdk-18 
# Wed, 10 Aug 2022 17:10:21 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Wed, 10 Aug 2022 17:10:21 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5c9d6483dab113d2d9b50fdf3156622aa2ec3d6faaed5664d15a5568032d1714`  
		Size: 103.2 MB (103204200 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0f4438539876006761cb687527bd8cb94cc7a273cf8bb47563981044f2e1771e`  
		Last Modified: Wed, 10 Aug 2022 16:38:40 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a91856336cfdacf547b1d0d94d065d6b3bdd9edb62351e0df92549cd0a65a49`  
		Last Modified: Wed, 10 Aug 2022 17:33:00 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc63044ec1c6da15a3f6d6135965b6e55b7e7899fb0eaae529fe3626ba69d6e`  
		Last Modified: Wed, 10 Aug 2022 17:33:00 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a832c9a3c0d67e44835cf87df912846f421402e83a20f3e94bd283062f92f8a9`  
		Last Modified: Wed, 10 Aug 2022 17:33:00 GMT  
		Size: 72.0 KB (72007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b73642ce805331d7b7c6476923129ea292e1631d34fd0966df74206628d2f2`  
		Last Modified: Wed, 10 Aug 2022 17:32:57 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8848a68fe0c06bdec8b9d045dc17dde80cbf68a8271740a3f5d37eba0e4683`  
		Last Modified: Wed, 10 Aug 2022 17:32:57 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2800e34e92da5c7f17819d954e6231da297424f205255654d1c5260b43714d5`  
		Last Modified: Wed, 10 Aug 2022 17:33:17 GMT  
		Size: 184.2 MB (184209822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12afdbdd4e49e3bbb98e27bb05b00923bad1d92eade208e722a9d1c0e247cc9`  
		Last Modified: Wed, 10 Aug 2022 17:32:58 GMT  
		Size: 3.5 MB (3529920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db36956e33bf103ca85c22d9398fca4899c0827e8862ce14f57df93bd16b2135`  
		Last Modified: Wed, 10 Aug 2022 17:32:57 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
