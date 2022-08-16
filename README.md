# General
This container allows to run [markdown-to-pdf](https://github.com/wll8/markdown-to-file) and create pdf files during CI/CD.

# Usage

Assuming that you have *somefile.md* in current directory, the following command will convert it to pdf.

```bash
docker run -it --rm  -v "$(pwd)":/data bladerunner2020/markdown-to-pdf:1.0  sh -c "m2f /data/somefile.md pdf" 
```
