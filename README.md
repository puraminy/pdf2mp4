## Convert pdf to video

A linux bash file to convert a pdf file to a video in mp4 format. It scans the pages of the pdf file using a sliding window and save them as frames in a folder, then it creates a video from the frames.


## Usage

```
./pdftomp4 --input 1column_paper.pdf
```

If you have a paper with two columns you can also use the following command. This way, the sliding window moves over columns:

```
./pdftomp4 --input 2column_paper.pdf --cols 2
```

It has many options that you can find by checking the code. Some of them are :

```

start=1  # start page (from)
end=1000  # end page (to)

win_height=400 # the height of sliding window (view port)
stride=32 # the number of pixels to slide

cut_left=100 # left margin to crop
cut_top=100   # top margin to crop

cols=0  # number of paper columns 
```

You can set them in the code or pass them from the command line using this syntax `--option option_value` (for example `--end 10`)


## Prerequisite

  - FFMpeg
  - ImageMagick
