## `adoptopenjdk:8u292-b10-jre-openj9-0.26.0-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:63afc76e27a3f9a822cdec221a99cb30ebb9570009de060f8a826a7f86eb9878
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `adoptopenjdk:8u292-b10-jre-openj9-0.26.0-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull adoptopenjdk@sha256:13a0e3c20d99bcdca5a6b8d71bba7406af3dfa1f1b352884a731d50643996ea9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2777267505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f45b3541010f9f4168847d1da43e4de49ba77a6a46bc49a424a4740a97c78db`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Aug 2021 12:16:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 19:21:08 GMT
ENV JAVA_VERSION=jdk8u292-b10_openj9-0.26.0
# Wed, 11 Aug 2021 19:27:00 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10_openj9-0.26.0/OpenJDK8U-jre_x64_windows_openj9_8u292b10_openj9-0.26.0.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10_openj9-0.26.0/OpenJDK8U-jre_x64_windows_openj9_8u292b10_openj9-0.26.0.msi ;     Write-Host ('Verifying sha256 (8decae9e065946cfc9a4b7f3c0ed61cfc6fe3076cdcbbbece33ef39c9ccef6e3) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '8decae9e065946cfc9a4b7f3c0ed61cfc6fe3076cdcbbbece33ef39c9ccef6e3') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 11 Aug 2021 19:27:03 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f5be68d5dab08a1dcc52a6ee52dd4901e4d6a384f0df3a12cba3d53649f7c602`  
		Last Modified: Wed, 11 Aug 2021 13:29:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4084bd76e8f9657fa0af0e0c819c10064a701b1f5c84252d91f9fdcd54b71e9b`  
		Last Modified: Wed, 11 Aug 2021 20:30:35 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e6f583c0530dc2e2b138cb5428422792c0eed69b5f25664303736208b81655`  
		Last Modified: Wed, 11 Aug 2021 20:39:52 GMT  
		Size: 91.3 MB (91265282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230f9212e119e4144babf359bdc57721ea96ca68c7e36c6b5adf40e4a22ae915`  
		Last Modified: Wed, 11 Aug 2021 20:39:42 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
