## `adoptopenjdk:14-jdk-openj9-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:4595fb80a139017314e2bf4b8f224343645b3c222433036b2ae9d7bc9bcd066e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `adoptopenjdk:14-jdk-openj9-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull adoptopenjdk@sha256:f80f0ff8484aa781ab7d2d0b6a5c94cc15c39edd2255a62b43f0c2df5411c6c8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2784585203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e10cc439c5716c87d499df031d4517b9168822ab02d53aa864b6043dbb8e4ac6`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 21:20:28 GMT
ENV JAVA_VERSION=jdk-14.0.2+12_openj9-0.21.0
# Wed, 09 Dec 2020 21:23:00 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12_openj9-0.21.0/OpenJDK14U-jdk_x64_windows_openj9_14.0.2_12_openj9-0.21.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12_openj9-0.21.0/OpenJDK14U-jdk_x64_windows_openj9_14.0.2_12_openj9-0.21.0.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (2e496ce7ca02f7a380fd1902e06d55d52121bb2eee29b21b8e54ad3e2fd3466e) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '2e496ce7ca02f7a380fd1902e06d55d52121bb2eee29b21b8e54ad3e2fd3466e') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 09 Dec 2020 21:23:01 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Wed, 09 Dec 2020 21:23:02 GMT
CMD ["jshell"]
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
	-	`sha256:2710c23583982d49f4a83afc02cfbaeeb59cec97189cd15be9ccd96295c07224`  
		Last Modified: Wed, 09 Dec 2020 22:09:44 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc600afed29050971dce14730970c65eafde433417db6356106a97b6a54dfcd6`  
		Last Modified: Wed, 09 Dec 2020 22:17:18 GMT  
		Size: 393.7 MB (393706208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8880d75db1bc5682e0b38f642ce347049f6366ebb9c17b3fbd7e23da19daadcb`  
		Last Modified: Wed, 09 Dec 2020 22:09:44 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2bcac2b9e817be29d10499b9620538a5443f6ebb186f1b0f4443baec067aae`  
		Last Modified: Wed, 09 Dec 2020 22:09:44 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
