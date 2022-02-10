## `python:windowsservercore-1809`

```console
$ docker pull python@sha256:2e2f7539418a05680b391cfc0a8414565405f6461e097f611401a4fa6548f15c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `python:windowsservercore-1809` - windows version 10.0.17763.2565; amd64

```console
$ docker pull python@sha256:d9bc15281f70018b32f43e279bbd2d8b651c952d0e3ec8169aa5d63dc7077634
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2766777709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32ee945e41837eb5816919dbebf413aa490d144f2e85aafd584e4db96fbb9664`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 02 Feb 2022 19:28:56 GMT
RUN Install update 1809-amd64
# Wed, 09 Feb 2022 13:09:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Feb 2022 13:19:44 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 09 Feb 2022 20:33:49 GMT
ENV PYTHON_VERSION=3.10.2
# Wed, 09 Feb 2022 20:35:49 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f ($env:PYTHON_VERSION -replace '[a-z]+[0-9]*$', ''), $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Wed, 09 Feb 2022 20:35:51 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 09 Feb 2022 20:35:52 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Wed, 09 Feb 2022 20:35:53 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2caf84b14febcda8077e59e9b8a6ef9a680aa392/public/get-pip.py
# Wed, 09 Feb 2022 20:35:54 GMT
ENV PYTHON_GET_PIP_SHA256=7c5239cea323cadae36083079a5ee6b2b3d56f25762a0c060d2867b89e5e06c5
# Wed, 09 Feb 2022 20:37:15 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 09 Feb 2022 20:37:16 GMT
CMD ["python"]
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
	-	`sha256:42a7c52a40ee1a3e8513436661e94eab0212813dc541bb3fdec3e396a986d673`  
		Last Modified: Wed, 09 Feb 2022 13:27:20 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa304a4f34e2e051cd97fedd65599e9fb5d39a0d18dc01a6937c5206b16c1203`  
		Last Modified: Wed, 09 Feb 2022 20:46:11 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9591bb7b6d98832c1f583580d4270340a2791f6c6e145b1784e1f5d42e20df25`  
		Last Modified: Wed, 09 Feb 2022 20:46:17 GMT  
		Size: 46.5 MB (46544066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d8c1bf45de3997fe38cf3ef27cb91ed40919a7b13c6234f6074e784808be5f`  
		Last Modified: Wed, 09 Feb 2022 20:46:11 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177364207a5e525c7c1f66b8ad4682fd7b1699def51e982b9eb98cc954b10ff8`  
		Last Modified: Wed, 09 Feb 2022 20:46:08 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d68c037a34aebfe254ae2481c6c12c1437b6c8e165ed536f0d8aa9bd0d89d9`  
		Last Modified: Wed, 09 Feb 2022 20:46:09 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77223368de3ceb600b1992ed474ea2e7b33096b1d0d07adf83f6bb9c97c1cd3a`  
		Last Modified: Wed, 09 Feb 2022 20:46:09 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5cd91cbbbf90c452b9901355041801f48da44ab106b3287088a5473ed20fac6`  
		Last Modified: Wed, 09 Feb 2022 20:46:11 GMT  
		Size: 6.5 MB (6507651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:831a1666720a5885b0b9ef3cd7451ebcfa33460a2556fad9e88e51659f257faa`  
		Last Modified: Wed, 09 Feb 2022 20:46:09 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
