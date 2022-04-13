## `eclipse-temurin:18-jdk-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:7876a2888bde3464aacc7dbf93e766ca99538ad80ecc507b9fcfaad5fe87ec6e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `eclipse-temurin:18-jdk-nanoserver-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull eclipse-temurin@sha256:954845c955201ab0f3628e2cd3f76601085a353ddcf8cae89a6277ea5bb32669
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.1 MB (293059900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:848dd61169ff7c08aab2c0cadd6d292e64c9d381b2e9559da27422c4010661ba`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 15:16:11 GMT
SHELL [cmd /s /c]
# Wed, 13 Apr 2022 15:47:14 GMT
ENV JAVA_VERSION=jdk-18+36
# Wed, 13 Apr 2022 15:47:15 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 13 Apr 2022 15:47:16 GMT
USER ContainerAdministrator
# Wed, 13 Apr 2022 15:47:22 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 13 Apr 2022 15:47:23 GMT
USER ContainerUser
# Wed, 13 Apr 2022 15:47:38 GMT
COPY dir:2e742036aad301ef262998624b1ad05a0be865b4697e1fe99b4c522724f72462 in C:\openjdk-18 
# Wed, 13 Apr 2022 15:47:48 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 13 Apr 2022 15:47:49 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ea4009814dceb50337c66614a6008cfc2fb73ce53e62162bce071ef6ea1adf2d`  
		Last Modified: Wed, 13 Apr 2022 15:58:06 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08aaf12cedc1817ed98e2b881a790b03ccd6a520c728338bbe763cb9a6601a5e`  
		Last Modified: Wed, 13 Apr 2022 16:38:00 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874ba82981bcf34adf712063ea1eae0fefc88f604a0fbbbf26fffccbdd53db1f`  
		Last Modified: Wed, 13 Apr 2022 16:37:59 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16a36ab9150af19bed162b78a51b572a3a7e50c0ce2f40bcc918ded3ede543d`  
		Last Modified: Wed, 13 Apr 2022 16:37:59 GMT  
		Size: 1.1 KB (1087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b28e0d32a47b4f7dc44af6a29d1a219b475df7c24090ca39b961f4b27aa518`  
		Last Modified: Wed, 13 Apr 2022 16:37:57 GMT  
		Size: 80.0 KB (80015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a725f5aa3ef591009507a47f76df82a47c636c79bf878c1ccb2190a758bf7bf`  
		Last Modified: Wed, 13 Apr 2022 16:37:57 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b2da3dfc2555008b5bab023577767f951cd86ec23299019b40aeb22ddb580d5`  
		Last Modified: Wed, 13 Apr 2022 16:38:15 GMT  
		Size: 186.3 MB (186345307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e159809587b5e48582afc13a2adf554778995f9b288fc49c7ccaa58ef407f2c`  
		Last Modified: Wed, 13 Apr 2022 16:38:01 GMT  
		Size: 3.5 MB (3532077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1e8c1d86a0970e67d1e87439d336eb7a57e83d7a88794ec916b299d0da35ee`  
		Last Modified: Wed, 13 Apr 2022 16:37:57 GMT  
		Size: 1.0 KB (1045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
