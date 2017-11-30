# ActivityNet-Video-Downloader

This simple script is for downloading videos of ActivityNet dataset by parsing URLs from given .json file. Therefore, it is required to download the related .json file [here](http://activity-net.org/download.html).

## Using activityNetDownloader

1. Install the prerequisites.

	- Python 2.7
	
	- Pafy:

		``` bash
	   sudo pip install pafy
	   ```

2. Clone the repository or download the zip to your working directory.

	```bash
   git clone https://github.com/ozgyal/ActivityNet-Video-Downloader.git
   ```

3. Define a path to download the videos. 
	
    ```python
	directory = '/path/to/your/directory/'
    ```

4. Videos will be downloaded in ".flv" format. If you want to change this, you can modify the following line by considering [Pafy's website](https://pypi.python.org/pypi/pafy):

	```python
	best = video.getbest(preftype="flv")
    ```
    
5. Run the script.

	``` bash
	python activityNetDownloader.py
	```
