# uFR 

A cli-based **rss** reader written in python
## Installation

### pip 
If your system (Windows, macOS and some Linux distributions) supports **pip**
```bash
pip install unnfr
```

### Arch Linux
on Arch Linux or Arch-based Distributions (EndeavourOS, Manjaro, etc.), you can use the PKGBUILD
```bash
makepkg -si
```

### Other
You can setup a `venv` 
```bash
python -m venv ~/.venv
source ~/.venv/bin/activate
pip install unnfr
```
Or for windows:
```cmd
python -m venv %USERPROFILE%/.venv
%USERPROFILE%/bin/activate.bat
pip install unnfr

```
## Dependencies

- **requests**: if you want to download feeds
- **xmltodict**: required to read feeds
- **inscriptis**: required for descriptions
## License

uFR is licensed with the [MIT](https://choosealicense.com/licenses/mit/) License
