## `adoptopenjdk:11-jdk-hotspot-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:e6a99cf2d726c2bbecdbd63be66d1e9acafb045375aa36aec57011192756b078
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `adoptopenjdk:11-jdk-hotspot-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull adoptopenjdk@sha256:120d004032f7c0f2234844a70535258eee217e1581db8605e3793e56cd1f56b1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3050435450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b262d80ccebf678735a62fc9a62a74a6fd892808a79927109aea44b8e0f82949`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Aug 2021 12:16:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 18:54:37 GMT
ENV JAVA_VERSION=jdk-11.0.11+9
# Wed, 11 Aug 2021 18:56:34 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_x64_windows_hotspot_11.0.11_9.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_x64_windows_hotspot_11.0.11_9.msi ;     Write-Host ('Verifying sha256 (de7de70fbd9f3ff49ce34db87c5f331a5c0b72e54c16e9e6d9ba3007d23b361e) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'de7de70fbd9f3ff49ce34db87c5f331a5c0b72e54c16e9e6d9ba3007d23b361e') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 11 Aug 2021 18:56:37 GMT
CMD ["jshell"]
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
	-	`sha256:a771911218e2373e9fb4e1fd731e5b0e16b600b45f6ac384375ded412a3ae225`  
		Last Modified: Wed, 11 Aug 2021 20:00:00 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c2da431d52fca0b5b78a26538688c3a86371e194fa63dc4dd4c0946f6b8203a`  
		Last Modified: Wed, 11 Aug 2021 20:07:10 GMT  
		Size: 364.4 MB (364433281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5540c8f069d8e443ddd1176e0e4e18673799311eb80f3d90f7292a7257891623`  
		Last Modified: Wed, 11 Aug 2021 20:00:00 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
