## `hylang:pypy-windowsservercore-1809`

```console
$ docker pull hylang@sha256:93c129453cace4051afd0f85c90342e66e1021eae202738c6c83fe01b7b4f76d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `hylang:pypy-windowsservercore-1809` - windows version 10.0.17763.2565; amd64

```console
$ docker pull hylang@sha256:255685849b9a0e343ceda9627ad9e8695871a9644c2b0659b76b98a1efe242c3
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2762068109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3763da34df45b36405e1651cec938deddb3ea1d098d1f383478c33bf59a3991`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 02 Feb 2022 19:28:56 GMT
RUN Install update 1809-amd64
# Wed, 09 Feb 2022 13:09:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Feb 2022 13:11:21 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Wed, 09 Feb 2022 13:12:34 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x64.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = 'da66717784c192f1004e856bbcf7b3e13b7bf3ea45932c48e4c9b9a50ca80965'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Wed, 23 Feb 2022 02:14:43 GMT
ENV PYPY_VERSION=7.3.8
# Wed, 23 Feb 2022 02:20:22 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.8-v7.3.8-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = '0894c468e7de758c509a602a28ef0ba4fbf197ccdf946c7853a7283d9bb2a345'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.8-v7.3.8-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy3 --version") ...'; 	pypy3 --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 23 Feb 2022 02:20:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 23 Feb 2022 02:20:25 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 23 Feb 2022 02:22:19 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$pipVersion = & pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)'; 	$setuptoolsVersion = & pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)'; 		Write-Host ('Installing "pip == {0}", "setuptools == {1}" ...' -f $pipVersion, $setuptoolsVersion); 	pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $pipVersion) 		('setuptools == {0}' -f $setuptoolsVersion) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 23 Feb 2022 02:22:20 GMT
CMD ["pypy3"]
# Wed, 23 Feb 2022 02:50:44 GMT
ENV HY_VERSION=1.0a4
# Wed, 23 Feb 2022 02:50:45 GMT
ENV HYRULE_VERSION=0.1
# Wed, 23 Feb 2022 02:52:12 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION) ('hyrule == {0}' -f $env:HYRULE_VERSION)
# Wed, 23 Feb 2022 02:52:13 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1bd78008c728d8f9e56dc2093e6eb55f0f0b1aa96e5d0c7ccc830c5f60876cdf`  
		Size: 995.4 MB (995381853 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f0c1566a9285d9465334dc923e9d6fd93a51b3ef6cb8497efcacbcf64e3b93fc`  
		Last Modified: Wed, 09 Feb 2022 13:26:13 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977ed2cf6839223b96336b95fbc7b18790a8c388e758a4b5f403696804739a5b`  
		Last Modified: Wed, 09 Feb 2022 13:26:12 GMT  
		Size: 356.8 KB (356819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090aceebb35b9bcb96fa341afc3e961eb65c37ed4bc746e7e03249273d754df9`  
		Last Modified: Wed, 09 Feb 2022 13:26:29 GMT  
		Size: 15.5 MB (15490453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c5d1f58c9ccb416475e7fa5abc5710e84a4ac8f6056172d00158c7cae3171c`  
		Last Modified: Wed, 23 Feb 2022 02:31:06 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a565cc760a2d39bed62e2827f303804769e84e5167a5eb8936bd9f1a54602c8`  
		Last Modified: Wed, 23 Feb 2022 02:31:54 GMT  
		Size: 26.0 MB (25950734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84669a85ad56c6d6c7f5697fc3824efce000f437f69085748b048709542aa0e`  
		Last Modified: Wed, 23 Feb 2022 02:31:47 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fdec1b0e3f802f8f9e3601a4ea25ac8f4481b026081cc382dc68af9ee8ef6d`  
		Last Modified: Wed, 23 Feb 2022 02:31:47 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2ea80c5c490b7acf9e148f8524930a187afb4672f36cb0370baea5f5d3f535`  
		Last Modified: Wed, 23 Feb 2022 02:31:48 GMT  
		Size: 3.0 MB (2986217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9654545f7adacf97c10c28e2887ca2bb9dba165a94c85f7bd107b0ae96c6b4`  
		Last Modified: Wed, 23 Feb 2022 02:31:47 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b35f1a69f85e6f6f7d702790a2671caba5152a4b98df794df7e03a5b0c5743`  
		Last Modified: Wed, 23 Feb 2022 02:54:34 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc52a846359e80fcccba7a2ea2e1dacf357899dc9b8b896e2eaa8ad8c67e220`  
		Last Modified: Wed, 23 Feb 2022 02:54:34 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a3553f87cd95a337ac2d93d49102a4c696599ffc885efc251c1af41ceddf12`  
		Last Modified: Wed, 23 Feb 2022 02:54:36 GMT  
		Size: 3.6 MB (3557809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4e2a51a6c7cf1887f71639c8bda44133b6754b2bb7064547163a0af98e9f4b`  
		Last Modified: Wed, 23 Feb 2022 02:54:35 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
