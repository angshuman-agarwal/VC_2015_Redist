# VC++ 2015 Update 3 Redistributable DLLs

It is very hard to get hold of VC++ 2015 DLLs, so I thought I will put them here. When you download & install VC++ 2015 x64 DLLs from [here](https://www.microsoft.com/en-us/download/details.aspx?id=53587), a log file will be created under __%temp%__. 
The name of the logfile will be like `dd_vcredist_amd64_20190402210618_000_vcRuntimeMinimum_x64`.

Open the log file and navigate to this line (search for _SOURCEDIR_) - `Property(S): SOURCEDIR = C:\ProgramData\Package Cache\{0D3E9E15-DE7A-300B-96F1-B4AF12B96488}v14.0.23026\packages\vcRuntimeMinimum_amd64\`. This is where the package is present. For you the GUID in the package cache path might be different. You can search for `vc_runtimeMinimum_x64.msi` in the directory.

- Go to that path
- You will see a `cab1.cab` file. It is nothing but a zip archive.
- Use a standard .zip utility to unpackage wherever you want to

I have uploaded that cab file here under `x64` folder
