This is an implementation of Sea-Thru. The original paper by Derya Akkaynak and Tali Treibitz can be found [here](http://csms.haifa.ac.il/profiles/tTreibitz/webfiles/sea-thru_cvpr2019.pdf). Data can be found [here](http://csms.haifa.ac.il/profiles/tTreibitz/datasets/sea_thru/index.html).

You will need python3 as well as all the packages in the `requirements.txt` file, as well as tkinter (on Ubuntu, `sudo apt install python3-tk`).

I extended their method to use a CNN-based monocular depth estimation technique called monodepth2, which can be found [here](https://github.com/nianticlabs/monodepth2).
Check out the report for more information!

Example:

```
# install the requirements
pip3 install -r requirements.txt
# download the dataset
wget "https://www.dropbox.com/sh/xtimf7qwfak4wwc/AAAGqn2JMe98II9lYeBTVBE2a/D3?dl=1"
unzip D3.zip
# generate the image
python3 seathru.py --image Raw/T_S04858.ARW --depth-map depthMaps/depthT_S04858.tif
```

Input:
![](input.png?raw=true)


Output:
![](output.png?raw=true)


