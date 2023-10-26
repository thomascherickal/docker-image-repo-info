## `pypy:3-windowsservercore-ltsc2022`

```console
$ docker pull pypy@sha256:1865fd0c040eb939f73ba4763c7b5460fa591cc97656a1e6fc29725ae7916f7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2031; amd64

### `pypy:3-windowsservercore-ltsc2022` - windows version 10.0.20348.2031; amd64

```console
$ docker pull pypy@sha256:58d161c85727fefbdbe68b0e1bd60f200c73cc8d0daa438bedc08bde504ef43e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1905706400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd2ab1cbd2634a60e10ed747faf8b58a478be596b6520710613a27e8fbc2a203`
-	Default Command: `["pypy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 06 Oct 2023 21:59:31 GMT
RUN Install update 10.0.20348.2031
# Wed, 11 Oct 2023 01:35:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 06:14:40 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Wed, 11 Oct 2023 06:15:05 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x64.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = 'da66717784c192f1004e856bbcf7b3e13b7bf3ea45932c48e4c9b9a50ca80965'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Thu, 26 Oct 2023 01:15:09 GMT
ENV PYPY_VERSION=7.3.13
# Thu, 26 Oct 2023 01:15:57 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.10-v7.3.13-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = '5b99422fb8978b2f4bbf97961bca49963a82dc47c2fa51b7d23c493db3a2e0f0'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.10-v7.3.13-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy --version") ...'; 	pypy --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Thu, 26 Oct 2023 01:15:58 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 26 Oct 2023 01:15:59 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 26 Oct 2023 01:17:06 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$pipVersion = & pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)'; 	$setuptoolsVersion = & pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)'; 		Write-Host ('Installing "pip == {0}", "setuptools == {1}" ...' -f $pipVersion, $setuptoolsVersion); 	pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $pipVersion) 		('setuptools == {0}' -f $setuptoolsVersion) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Thu, 26 Oct 2023 01:17:06 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d2471a50c8ec3ea61c16dd871f7b9167bf779faad2b6e5a6f72a18b88b846b`  
		Last Modified: Tue, 10 Oct 2023 17:55:23 GMT  
		Size: 471.2 MB (471244358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73b90f34f44bbbb354af4f3d4cc6cde597d2f5183641e139f7ca8b76ec3bb9`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd18844d7cd91075829793024df5a5d9d615bf17e860c71d9d1ef6b7cbd0dd0`  
		Last Modified: Wed, 11 Oct 2023 06:37:18 GMT  
		Size: 445.5 KB (445470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f4050e10e1bb82c108d6c64fa6275e021c24161296f4976b50cc7ddd01032a`  
		Last Modified: Wed, 11 Oct 2023 06:37:20 GMT  
		Size: 15.5 MB (15451502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee80caefaddaede3888ab0418aff530483fdd9fd46c5cac248d9b0f6bdc6318`  
		Last Modified: Thu, 26 Oct 2023 01:28:35 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436760db6a19d988fc0303ca8807e1b0f740e6679d4fc53ff84ee6f6ddd7af77`  
		Last Modified: Thu, 26 Oct 2023 01:28:42 GMT  
		Size: 26.1 MB (26113386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e07b985dbf43a3fdf9514dfb22953c434cabb8b8cd6c07dbfd30cf69106f00b`  
		Last Modified: Thu, 26 Oct 2023 01:28:33 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786c1b76f22dbe2e1f4b6142b574e4d72af0549d7e27c43d073687714977a6c5`  
		Last Modified: Thu, 26 Oct 2023 01:28:33 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b88fc23de941248ae48fe0c36b06ea28fb0fedc870e50cbf077be0d3d1bb84c5`  
		Last Modified: Thu, 26 Oct 2023 01:28:35 GMT  
		Size: 3.8 MB (3846396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88668fdb1eb0c4145ec947298644d37c1a4cddc03420a1616b0e3962f99b7fb1`  
		Last Modified: Thu, 26 Oct 2023 01:28:34 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
