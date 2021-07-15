## `adoptopenjdk:8u292-b10-jdk-openj9-0.26.0-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:b5e0db121bd7e53c229710b4ca63c17281878f805e63ce55d7b17a62150c47ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `adoptopenjdk:8u292-b10-jdk-openj9-0.26.0-windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull adoptopenjdk@sha256:5d91f9f3bb4030a39ebcaaca6e002ce18798856895da462994db01153b58fcca
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2904853209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:260e9fd5f58a069d7ab5a349b330799b7b3f5453c078c18a6c6ea6f12db1c9b4`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 15:59:19 GMT
ENV JAVA_VERSION=jdk8u292-b10_openj9-0.26.0
# Wed, 14 Jul 2021 16:00:55 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10_openj9-0.26.0/OpenJDK8U-jdk_x64_windows_openj9_8u292b10_openj9-0.26.0.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10_openj9-0.26.0/OpenJDK8U-jdk_x64_windows_openj9_8u292b10_openj9-0.26.0.msi ;     Write-Host ('Verifying sha256 (49e59ddbf8d9bcffbfe7c02bc4911ccc44b2426db4f4f02a3c13c3c0dadc28df) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '49e59ddbf8d9bcffbfe7c02bc4911ccc44b2426db4f4f02a3c13c3c0dadc28df') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 14 Jul 2021 16:00:58 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ce6c6f1d83a8e25cef40d46c7cb2160348273672c607c6c3c29623d014324c`  
		Last Modified: Wed, 14 Jul 2021 17:05:35 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d20c8b6a6c64d8d5e243ddc1957cc9ec29107f9320bcd6ec55d607e9092577`  
		Last Modified: Wed, 14 Jul 2021 17:05:54 GMT  
		Size: 219.4 MB (219402135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c78a445498930e64cd0664e3bcf611a98a8cf9680905e30f13abe15f42d349`  
		Last Modified: Wed, 14 Jul 2021 17:05:35 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
