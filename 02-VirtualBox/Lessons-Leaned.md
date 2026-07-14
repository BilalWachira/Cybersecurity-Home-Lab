# VirtualBox Lessons Learned

## ISO File Association

Windows displayed the downloaded ISO files as `WinRAR archive (.iso)`.

I initially questioned whether the files needed to be extracted. After checking the extension, I confirmed that the files were already ISO images and that WinRAR was only the default program associated with the file type.

## Key Lesson

The application icon or associated program does not determine the actual file format. The file extension should be verified before extracting or modifying a file.

## VirtualBox Navigation

VirtualBox initially opened in the Network Manager view rather than the main machine view.

I learned that a new virtual machine can still be created through:

```text
Machine → New
