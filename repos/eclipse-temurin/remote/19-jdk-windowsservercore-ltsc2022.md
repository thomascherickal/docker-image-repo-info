## `eclipse-temurin:19-jdk-windowsservercore-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:6020bae0c228525c3aac4121045a6ee5a281dacac63f7c97909e4572afd1d407
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1547; amd64

### `eclipse-temurin:19-jdk-windowsservercore-ltsc2022` - windows version 10.0.20348.1547; amd64

```console
$ docker pull eclipse-temurin@sha256:8cf9214ae45b8d65756449d18677f8bcee1704b63bee77f636cc751129e4f67e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2046666815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:219821098b90e750f409bf79b5a9334436a44a446d56087dcb6bc507b387fc2f`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Tue, 07 Feb 2023 11:42:22 GMT
RUN Install update 10.0.20348.1547
# Wed, 15 Feb 2023 22:37:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Feb 2023 23:20:54 GMT
ENV JAVA_VERSION=jdk-19.0.2+7
# Wed, 15 Feb 2023 23:22:27 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.2%2B7/OpenJDK19U-jdk_x64_windows_hotspot_19.0.2_7.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.2%2B7/OpenJDK19U-jdk_x64_windows_hotspot_19.0.2_7.msi ;     Write-Host ('Verifying sha256 (b2372bd728a5a708a4ce5ec6cc8b46489e5292051f4993568ec1d5f395f7e06e) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'b2372bd728a5a708a4ce5ec6cc8b46489e5292051f4993568ec1d5f395f7e06e') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-19' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 15 Feb 2023 23:23:12 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Wed, 15 Feb 2023 23:23:13 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d015a9e7adea898d81486dce8b513b0e9cbeca30904cac18c3ea98ab3be7a6`  
		Last Modified: Thu, 16 Feb 2023 00:28:01 GMT  
		Size: 293.3 MB (293317272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9c63a3d1906c0f8f7ca38587ab5f1c84160f9127cce25fb7f57d8a60dc7008`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ddcbf6bbcb07dff97ccd7f5e5ed5a3400deeae9ea0f2bdcf7cc83bfe386f95`  
		Last Modified: Thu, 16 Feb 2023 07:17:32 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49feba9ed6dc221a63d5555baac9e70d14eadc4e81c9377c8e1aa9c6a96fd795`  
		Last Modified: Thu, 16 Feb 2023 07:18:12 GMT  
		Size: 366.7 MB (366733673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb14f3b578d8fa31df15b2a16a3b318f9b089fae95d1ed2fef01d8786c6e8bd6`  
		Last Modified: Thu, 16 Feb 2023 07:17:33 GMT  
		Size: 582.5 KB (582547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23971dbccd1309568754433b618b72931e96b5e2d37b8f2bba4e2c320edb6421`  
		Last Modified: Thu, 16 Feb 2023 07:17:32 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
