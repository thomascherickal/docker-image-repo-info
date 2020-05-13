## `adoptopenjdk:11-jre-openj9-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:1b2f67aebbd69da997e09e1d6a27158c00abffcac5eeff5fb6c2319b4dd7041c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `adoptopenjdk:11-jre-openj9-windowsservercore-1809` - windows version 10.0.17763.1217; amd64

```console
$ docker pull adoptopenjdk@sha256:27c532650c03c90e00620335572032621697b30fc12f53f44924e8fad08bb2cf
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1789381890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a03baf1a4daf5df92e1bbd0f5818b977f495bafa83e3153bcff4cb4553f4ee23`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 12:41:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 May 2020 17:22:22 GMT
ENV JAVA_VERSION=jdk-11.0.7+10.1_openj9-0.20.0
# Wed, 13 May 2020 17:28:01 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.7%2B10.1_openj9-0.20.0/OpenJDK11U-jre_x64_windows_openj9_11.0.7_10_openj9-0.20.0.msi ...');         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         wget https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.7%2B10.1_openj9-0.20.0/OpenJDK11U-jre_x64_windows_openj9_11.0.7_10_openj9-0.20.0.msi -O 'openjdk.msi';         Write-Host ('Verifying sha256 (2d87def1e58a08db4fb7125d510a29f537c39bbb58c637b5b694abf1fff7fbdc) ...');         if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '2d87def1e58a08db4fb7125d510a29f537c39bbb58c637b5b694abf1fff7fbdc') {                 Write-Host 'FAILED!';                 exit 1;         };                 New-Item -ItemType Directory -Path C:\temp | Out-Null;                 Write-Host 'Installing using MSI ...';         Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',         '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;         Write-Host 'Removing openjdk.msi ...';         Remove-Item openjdk.msi -Force;         Remove-Item -Path C:\temp -Recurse | Out-Null;
# Wed, 13 May 2020 17:28:02 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:77613e754ba9d62c0acd4ef271c4ee7d3af091b8c8b310afa404560a9d281f82`  
		Last Modified: Wed, 13 May 2020 13:00:20 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d810ccd15d7c31a36ee65ea8b587f5efb4eec16a8c827e6476ab4036a37f93`  
		Last Modified: Wed, 13 May 2020 18:28:34 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0559f8ecbc5bfb7c0121f80c241e2b3bb35f7e9af8f4388e300eaaa143ff16ed`  
		Last Modified: Wed, 13 May 2020 18:35:47 GMT  
		Size: 71.0 MB (71045561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e6ddcd2ff7a0ef416cf8a9d760f486274bb310b1548d1157369f8405f51ba1`  
		Last Modified: Wed, 13 May 2020 18:35:31 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
