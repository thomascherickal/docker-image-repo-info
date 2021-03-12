## `adoptopenjdk:8-jre-openj9-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:ea01ee10573988b380f91fe94c7b33521d052e2860d1640e2d8b44b0f5ac3ba8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `adoptopenjdk:8-jre-openj9-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull adoptopenjdk@sha256:b4715401ca363bac50989ad2753c107aee9a1392b5e255da9d353ee05af97046
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2559571675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:905ab28e689602da8ebf6469bcb2f4e66c049b7d161b846d04ea01e552722276`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 19:51:31 GMT
ENV JAVA_VERSION=jdk8u282-b08_openj9-0.24.0
# Wed, 10 Mar 2021 19:56:44 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u282-b08_openj9-0.24.0/OpenJDK8U-jre_x64_windows_openj9_8u282b08_openj9-0.24.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u282-b08_openj9-0.24.0/OpenJDK8U-jre_x64_windows_openj9_8u282b08_openj9-0.24.0.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (cb1ba5f2d086ac3fb6a875ac7749837c1b0a7493d988d0b2360a0f2b392255c3) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'cb1ba5f2d086ac3fb6a875ac7749837c1b0a7493d988d0b2360a0f2b392255c3') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 10 Mar 2021 19:56:45 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae4593d8414b46fa4a3504a0dd75db92db4d9e8ac8f5e0bba3e14a72f5e76ba`  
		Last Modified: Wed, 10 Mar 2021 20:57:19 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec9292803154ca32e437e1c17c3022ac5e789294756b6183a8925133fd61162`  
		Last Modified: Wed, 10 Mar 2021 21:02:38 GMT  
		Size: 98.0 MB (98032910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59483a43d76fc521512856a6c178e108c5c3e9bad6ddba777970ae55c24711ce`  
		Last Modified: Wed, 10 Mar 2021 21:02:21 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
