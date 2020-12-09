## `adoptopenjdk:14-jre-openj9-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:37da4556bdfbbeb900cf5a8bb2fe26c50b38e0c149bf70ae793474d453b9d616
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `adoptopenjdk:14-jre-openj9-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull adoptopenjdk@sha256:44330ab78c352532cac2bbb6c5633e67241d5a3f58d7fccfe6fc75454d299cba
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2486743817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5e6ef9d05e1e30e39ecec6dbd79621674be42b17944796783573d74196d2f5d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
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
# Wed, 09 Dec 2020 21:29:44 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12_openj9-0.21.0/OpenJDK14U-jre_x64_windows_openj9_14.0.2_12_openj9-0.21.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12_openj9-0.21.0/OpenJDK14U-jre_x64_windows_openj9_14.0.2_12_openj9-0.21.0.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (12c883da9337470094993384c68f85effdd1752575fc2316459b50d541e35060) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '12c883da9337470094993384c68f85effdd1752575fc2316459b50d541e35060') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 09 Dec 2020 21:29:45 GMT
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
	-	`sha256:2710c23583982d49f4a83afc02cfbaeeb59cec97189cd15be9ccd96295c07224`  
		Last Modified: Wed, 09 Dec 2020 22:09:44 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8cd7f404a404b2a891baa9ab2c4122581ab289d57a29680f0d388c9cb61a95`  
		Last Modified: Wed, 09 Dec 2020 22:27:39 GMT  
		Size: 95.9 MB (95865943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eac8c2ccf7b904166eaba40eb2e86b3a8776c4fe58a56e9052b1f58b654a851`  
		Last Modified: Wed, 09 Dec 2020 22:25:29 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
