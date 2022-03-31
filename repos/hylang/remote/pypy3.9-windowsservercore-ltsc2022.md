## `hylang:pypy3.9-windowsservercore-ltsc2022`

```console
$ docker pull hylang@sha256:01d026fded52d3ffe687e0425e8b8f6f24dfd751ac0cd83b8b3a691c0db4eaa4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.587; amd64

### `hylang:pypy3.9-windowsservercore-ltsc2022` - windows version 10.0.20348.587; amd64

```console
$ docker pull hylang@sha256:663cee71a0b491e468c39437c57732da3d63df6c9b00776fcc85485b4e32766a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2271102687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c58a44df9d3c4acf70d7feb9cde586a9718dfaa5c6e35fdde4189647458d182`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Thu, 03 Mar 2022 05:02:11 GMT
RUN Install update ltsc2022-amd64
# Tue, 08 Mar 2022 19:26:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 08 Mar 2022 19:27:44 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Tue, 08 Mar 2022 19:28:39 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x64.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = 'da66717784c192f1004e856bbcf7b3e13b7bf3ea45932c48e4c9b9a50ca80965'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Wed, 30 Mar 2022 17:15:35 GMT
ENV PYPY_VERSION=7.3.9
# Wed, 30 Mar 2022 17:16:36 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.9-v7.3.9-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = 'be48ab42f95c402543a7042c999c9433b17e55477c847612c8733a583ca6dff5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.9-v7.3.9-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy --version") ...'; 	pypy --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 30 Mar 2022 17:16:37 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 30 Mar 2022 17:16:38 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 30 Mar 2022 17:17:46 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$pipVersion = & pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)'; 	$setuptoolsVersion = & pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)'; 		Write-Host ('Installing "pip == {0}", "setuptools == {1}" ...' -f $pipVersion, $setuptoolsVersion); 	pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $pipVersion) 		('setuptools == {0}' -f $setuptoolsVersion) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 30 Mar 2022 17:17:48 GMT
CMD ["pypy"]
# Wed, 30 Mar 2022 18:04:43 GMT
ENV HY_VERSION=1.0a4
# Wed, 30 Mar 2022 18:04:44 GMT
ENV HYRULE_VERSION=0.1
# Wed, 30 Mar 2022 18:05:28 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION) ('hyrule == {0}' -f $env:HYRULE_VERSION)
# Wed, 30 Mar 2022 18:05:29 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:037d5740b40414bc505c21324142a1cd3eab10c176189a9a74d1a90354ac7cd4`  
		Size: 969.5 MB (969547968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d58ba398110c3f761c6307a5621ec218b8593ba8b07b734436bcdd8d07a23e08`  
		Last Modified: Tue, 08 Mar 2022 20:00:31 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05429111ea1a767be23087b3f6fa1981262988c6d2df8593c80c89c9e2a4e861`  
		Last Modified: Tue, 08 Mar 2022 20:00:30 GMT  
		Size: 598.5 KB (598492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698c85ea3e7dd99853bbb9a33f94d396c7d355a5e77c52e258d46f0f0ce810d4`  
		Last Modified: Tue, 08 Mar 2022 20:00:32 GMT  
		Size: 15.7 MB (15701447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f196293e5c782b29357e73f16fd1ab044611d7f5847544619032020da6f79257`  
		Last Modified: Wed, 30 Mar 2022 17:42:32 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0ee775a0b032d042b57e6cc65ebc96a33a8ac82a5a3b21076f829088956053`  
		Last Modified: Wed, 30 Mar 2022 17:42:58 GMT  
		Size: 26.6 MB (26570221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9efb6b63b584fad68627f05dd9f1025f8a72fbf234d89f8f8845d0e5c7c0581f`  
		Last Modified: Wed, 30 Mar 2022 17:42:29 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b928aa0273405d83ad523e6399c60997e1b6ba8520f3dad44736bb16af4953ce`  
		Last Modified: Wed, 30 Mar 2022 17:42:29 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554025c1d199789bc9412a001ad415c45a20f4ff51e5e717ecf943b77a6a00a5`  
		Last Modified: Wed, 30 Mar 2022 17:42:31 GMT  
		Size: 3.2 MB (3181434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e6f0e2bf5a2d4ba98efc9298b6e79d31d737e5c3db16a85a32d9119595c38a`  
		Last Modified: Wed, 30 Mar 2022 17:42:29 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5468dfc6d80ff297b437e12d9f0fc38d71b74acd27125e24e749377b5b0fd392`  
		Last Modified: Wed, 30 Mar 2022 18:12:24 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a098f487ba7e8e5011b46a6f783c6772e72e5063439beccd196ae6f6ef11a2`  
		Last Modified: Wed, 30 Mar 2022 18:12:24 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470eac63e35a3c119bc7c40adaed0cc9d2084ef9edd0f90b3c36d32768124dd8`  
		Last Modified: Wed, 30 Mar 2022 18:12:28 GMT  
		Size: 3.8 MB (3792732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c01541b262c54855d820c1d6157d17a509eaabdd29595628efae4ab29ef873`  
		Last Modified: Wed, 30 Mar 2022 18:12:24 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
