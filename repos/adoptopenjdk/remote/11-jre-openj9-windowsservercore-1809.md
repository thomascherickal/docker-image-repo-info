## `adoptopenjdk:11-jre-openj9-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:a9422ac729cae68db3bfea87ce055b4bc86c5d6c94dc7ab35301e6dd92c77bac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `adoptopenjdk:11-jre-openj9-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull adoptopenjdk@sha256:fd45da383983ca545e1294aaf509c23e52a306db52c1b4bc128ebd42d69fde9d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2471444006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c9f5394271adb22c711becd8abb334b1b961eeb80337883e198d1c91e0eec2b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 21:09:26 GMT
ENV JAVA_VERSION=jdk-11.0.9+11_openj9-0.23.0
# Wed, 09 Dec 2020 21:18:05 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_x64_windows_openj9_11.0.9_11_openj9-0.23.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jre_x64_windows_openj9_11.0.9_11_openj9-0.23.0.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (780cb9f4aa34493d6ce555983957b04514da630901004242c1d8f70ba46cbcf8) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '780cb9f4aa34493d6ce555983957b04514da630901004242c1d8f70ba46cbcf8') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 09 Dec 2020 21:18:06 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7433b46de6c97734364f747bd0e3df41a54429134f36eb65f1ad26ecfda6a1c`  
		Last Modified: Wed, 09 Dec 2020 22:00:35 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd299a6e3260c63707e91ae488d90934a58f270bf34bafefcc38206af0e315b0`  
		Last Modified: Wed, 09 Dec 2020 22:09:08 GMT  
		Size: 80.6 MB (80566136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43b8836a4194baf85f3080e94ded5ef50a8719e5db8b6b051f422874da04ff4`  
		Last Modified: Wed, 09 Dec 2020 22:08:57 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
