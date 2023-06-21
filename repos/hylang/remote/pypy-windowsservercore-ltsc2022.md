## `hylang:pypy-windowsservercore-ltsc2022`

```console
$ docker pull hylang@sha256:3de0e6ac12b0f615cdf807c6c1485799dee601db42d697a9e5de5eda24bfe132
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `hylang:pypy-windowsservercore-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull hylang@sha256:bbbb57f903d918151046309076ec7477be3fb0fc6ca2996c9fd916abfa7225a1
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1439209594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc2060b9188a7f045606c5b0ec7aacd845356e84a5ffe9a4198f75a18edfa243`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Wed, 14 Jun 2023 17:38:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 22:49:27 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Wed, 14 Jun 2023 22:49:59 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x64.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = 'da66717784c192f1004e856bbcf7b3e13b7bf3ea45932c48e4c9b9a50ca80965'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Wed, 14 Jun 2023 22:50:00 GMT
ENV PYPY_VERSION=7.3.11
# Wed, 14 Jun 2023 22:50:50 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.9-v7.3.11-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = '57faad132d42d3e7a6406fcffafffe0b4f390cf0e2966abb8090d073c6edf405'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.9-v7.3.11-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy --version") ...'; 	pypy --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 14 Jun 2023 22:50:52 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 14 Jun 2023 22:50:52 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 14 Jun 2023 22:52:02 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$pipVersion = & pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)'; 	$setuptoolsVersion = & pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)'; 		Write-Host ('Installing "pip == {0}", "setuptools == {1}" ...' -f $pipVersion, $setuptoolsVersion); 	pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $pipVersion) 		('setuptools == {0}' -f $setuptoolsVersion) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 14 Jun 2023 22:52:02 GMT
CMD ["pypy"]
# Wed, 14 Jun 2023 23:58:58 GMT
ENV HY_VERSION=0.26.0
# Wed, 14 Jun 2023 23:58:59 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 15 Jun 2023 00:01:29 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION) ('hyrule == {0}' -f $env:HYRULE_VERSION)
# Thu, 15 Jun 2023 00:01:30 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0972ddd233121a2afd2cf1a3eaec49d595cfe6b3ebe19ef3dd492d99784c370f`  
		Last Modified: Wed, 14 Jun 2023 18:17:55 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:494928dc22760e844729c73d3630dffe1d8a58b5cb4f07f51aa050220ccbb022`  
		Last Modified: Wed, 14 Jun 2023 23:39:45 GMT  
		Size: 315.4 KB (315438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47cea0a370519618fc87381c6251f61791e86d8479636a8d529614016877f8d`  
		Last Modified: Wed, 14 Jun 2023 23:39:48 GMT  
		Size: 15.5 MB (15452954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb49b84e7d71577b27e21ef90de124e68b909b72f4e03f0a281c84cdf165d0a0`  
		Last Modified: Wed, 14 Jun 2023 23:39:45 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b3c182b43c5921d2ff3437b88a9e02514188a74f397fb025602b005fc9a5026`  
		Last Modified: Wed, 14 Jun 2023 23:39:49 GMT  
		Size: 26.6 MB (26552400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b13f7a514f8b0030a11ef008daa88a292181d619255e9d281fb9030bafc6c8c`  
		Last Modified: Wed, 14 Jun 2023 23:39:43 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22951c8822da1115237b996f794344bb115bdce82f91c7400b5d9824a14891b1`  
		Last Modified: Wed, 14 Jun 2023 23:39:43 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf3419bf96ca065d4875e75a1ee086ffdb60018be7f3a24ad8f0bc686aca3aea`  
		Last Modified: Wed, 14 Jun 2023 23:39:44 GMT  
		Size: 3.5 MB (3504564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a459b1ff6fe48419d4987b434e68214f8e2cbfca1f5cc0ca397f43260b1e3a2`  
		Last Modified: Wed, 14 Jun 2023 23:39:43 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de229f166b0be8658965957d48823da825915a5ed66b1050c7654119e28b7f4`  
		Last Modified: Wed, 21 Jun 2023 01:16:06 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8017a3bf355322e16d31fe6cea33b8e0a581ccbd8aae9927ca666b0f9704b9`  
		Last Modified: Wed, 21 Jun 2023 01:16:06 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037e2803d629a6d03d3538c5cd974d74a78a113cf92c4c64cf2f34f13997bbb1`  
		Last Modified: Wed, 21 Jun 2023 01:16:08 GMT  
		Size: 4.8 MB (4775066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc6153b74bc0fd37bfc798e892b87e4175d2986083d2a1d187fd8107387ebe6`  
		Last Modified: Wed, 21 Jun 2023 01:16:06 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
