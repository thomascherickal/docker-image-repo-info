## `adoptopenjdk:8u275-b01-jdk-openj9-0.23.0-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:902b1f3295599bfe1757e044edc5b2da57f771e01308ec1d7ea49cc558e52f79
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `adoptopenjdk:8u275-b01-jdk-openj9-0.23.0-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull adoptopenjdk@sha256:718eb6f18b5d0f9c433fd4360a00b974486b13c92d212f73ad158fa5e17c0cb4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2661405751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a3db2a032bdd29ada00a97e4bd15bdd1520ca17e216755ce9d234eb0c104c2a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 22:25:37 GMT
ENV JAVA_VERSION=jdk8u275-b01_openj9-0.23.0
# Wed, 13 Jan 2021 22:27:34 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jdk_x64_windows_openj9_8u275b01_openj9-0.23.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jdk_x64_windows_openj9_8u275b01_openj9-0.23.0.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (94f90bbde3cee74fb0f7708259186d54c7fa91d0519e9c8f9b363f31ddcfbb55) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '94f90bbde3cee74fb0f7708259186d54c7fa91d0519e9c8f9b363f31ddcfbb55') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 13 Jan 2021 22:27:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21fb211f0cc4413d4089ab88aaf06ccd58b8baca8b25f9c36dd3d9001e3eeffc`  
		Last Modified: Wed, 13 Jan 2021 23:28:54 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7cf519518be61b90985a61ae370884bb08baeee6bf69ebc3f1fd060ef2c409`  
		Last Modified: Wed, 13 Jan 2021 23:29:14 GMT  
		Size: 225.6 MB (225630219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc6dc8706e2ef3d5bc57f3457ea4a99eed7c7df677de5e42ddebf99d8ef07e2`  
		Last Modified: Wed, 13 Jan 2021 23:28:53 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
