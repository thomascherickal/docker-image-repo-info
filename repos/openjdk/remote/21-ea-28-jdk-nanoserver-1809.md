## `openjdk:21-ea-28-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:8682af4bea7b19caf93c131d71d93c8289236015247e571dc499d48f7604958e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `openjdk:21-ea-28-jdk-nanoserver-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull openjdk@sha256:82181acf8c7fea9d21949149c8627c16d3284133c3c0ecd66363238935e0811b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.2 MB (306238943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c3cd32f8e6c6d7942352ba0209201f189f4aa4980fc2c5d767c0e0d5caa2876`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 08 Jun 2023 12:28:32 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:41:42 GMT
SHELL [cmd /s /c]
# Wed, 14 Jun 2023 20:32:10 GMT
ENV JAVA_HOME=C:\openjdk-21
# Wed, 14 Jun 2023 20:32:11 GMT
USER ContainerAdministrator
# Wed, 14 Jun 2023 20:32:20 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 14 Jun 2023 20:32:21 GMT
USER ContainerUser
# Fri, 23 Jun 2023 00:39:47 GMT
ENV JAVA_VERSION=21-ea+28
# Fri, 23 Jun 2023 00:40:02 GMT
COPY dir:5e5e1336ec2d60e8b2707494abc1e5b87c4f17d59c6e98aa6bc368a25f065267 in C:\openjdk-21 
# Fri, 23 Jun 2023 00:40:15 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Fri, 23 Jun 2023 00:40:16 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:234d39d9b188e7f36d5a77b0d54990ea826551314b6703c83aef3ef20b1a7050`  
		Last Modified: Tue, 13 Jun 2023 19:06:23 GMT  
		Size: 104.4 MB (104397895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2364e413270ecc5b57d2596b092fb57b828229b59e810d9f345fc0d31ca535d`  
		Last Modified: Wed, 14 Jun 2023 18:26:46 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c86c8f72d5c620385f29493830932257c53d9dad74802ecdf0bdbc03b2494c`  
		Last Modified: Wed, 14 Jun 2023 20:37:08 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30698f58bfeb99d6b9b76177da8956540b4b318293543c1e5c8447403dc97f1`  
		Last Modified: Wed, 14 Jun 2023 20:37:08 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c50e91142bca7a5ff55e1ebc6fd6e7a26cdfc9d0890ad2eb8a5c7b031598294`  
		Last Modified: Wed, 14 Jun 2023 20:37:08 GMT  
		Size: 68.8 KB (68836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a22e7e5b49f87fd9c56f26a1e630fdf989e0f48edc7f35e074d47642e4af389`  
		Last Modified: Wed, 14 Jun 2023 20:37:06 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe118feaacd20bc1c480da04798e0c7ee8d9cf420ea387ad3ba212325a1d698`  
		Last Modified: Fri, 23 Jun 2023 00:44:39 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58c30d2d307952321c32e77fae8a75c49572a318b5b276fa057765097be2f6e`  
		Last Modified: Fri, 23 Jun 2023 00:44:59 GMT  
		Size: 198.0 MB (197954525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e26a243de6eae2cad9d3cfbbb8b70e3e87e4d72dca30d1e246d82094c55919`  
		Last Modified: Fri, 23 Jun 2023 00:44:40 GMT  
		Size: 3.8 MB (3810688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3a6f5785e412ff54de2445547cc49b85d16dff7df91e97348ae093922889627`  
		Last Modified: Fri, 23 Jun 2023 00:44:39 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
