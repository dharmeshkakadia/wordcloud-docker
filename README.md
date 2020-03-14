wordcloud-docker
================

Generate word cloud image from text using [Python wordcloud](https://github.com/amueller/word_cloud) package without any manual installation using docker.

To generate word cloud image from text file `README.md` use the following command from the directory of the file.

```
docker run -it --rm --volume="$PWD:/work" --workdir /work dharmeshkakadia/wordcloud wordcloud_cli --text README.md --imagefile wordcloud.png
```

This will generate output like following and save it as `wordcloud.png` in the current directory.

![example generated wordcloud image](https://raw.githubusercontent.com/dharmeshkakadia/wordcloud-docker/master/example-wordcloud.png)

For more options on controlling word cloud output, please see the [package documentation](https://amueller.github.io/word_cloud/cli.html)