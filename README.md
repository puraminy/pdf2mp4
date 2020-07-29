## Convert pdf to video

A linux bash file to convert a pdf file to a video in mp4 format. It scans the pages of the pdf file using a sliding window and save them as frames in a folder, then it creates a video from the frames.


## Usage

```
./pdftomp4 --input 1column_paper.pdf
```

If you have a paper with two columns you can also use:

```
./pdftomp4 --input 2column_paper.pdf --cols 2
```

It has many options that you can find by checking the code


## Prerequisite

  - FFMpeg
  - ImageMagick
