# Tar files in Linux

有很多办法可以在linux中压缩一个文件夹

Run the following to find out:

```bash
tar czvf name-of-archive.tar.gz /path/to/directory

```
If you want exclude some big file use --exclude 

```bash
tar czvf name-of-archive.tar.gz --exclude ='/path/to/directory/exclude_dir' /path/to/directory

```