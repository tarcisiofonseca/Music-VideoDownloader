# Music-VideoDownloader
The most simple video or music downloader I could think of for non-technical users. It can download video or music from more than 1,000 websites, since it uses [youtube-dl](https://github.com/ytdl-org/youtube-dl) library to download content. The complete list of supported websites can be found [here](https://ytdl-org.github.io/youtube-dl/supportedsites.html).

## Requirements

Just a Google account. The script uses Google Colab environment to download the files directly to your Google Drive, so you can use it even on smartphones without [Termux](https://termux.dev/en/) or a rooted device.

## First steps

1 - Download the file named "Music_VideoDownloader.ipynb" <br>
2 - Access https://colab.research.google.com/ <br>
3 - Upload the file (Google may call it "notebook") <br>

## How to use

Before running the script, there are three variables that you need to configure:

**output_ext** = Change the value to 0 if you want just the audio (.mp3) or to 1 if you want both audio and video (.mp4) <br><br>
**folder_name** = The name of the folder in your Google Drive account to where the files will be stored (keep it between quotation marks). If the folder doesn't exist yet, it will be created before. <br><br>
**videos_list** = Just follow the example in the code. Put the links between quotation marks and separated by commas (except for the last link). There is virtually no limit for how many files you can download for each time you run the script (probably limited just by Colab's cache), and you **can** download a whole youtube playlist by using its links, instead of downloading each song separately. <br><br>

After setting everything up, just select the option Run All (CTRL + F9 if you are on PC) and give it permission to access Google Drive, so the script can move the files from Colab's environment to your personal account.

