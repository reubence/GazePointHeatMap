# Gaze Heat Plot
Simple Python command line based script to generate a gaze point heat map from a csv file. 👁️

## Usage
Install the required dependencies over the command line.
```bash
pip install -r requirements.text
```

Run the script from the command line.
```bash  
python gazeheatplot.py --input-path gaze-data.csv --display-width 1440 --display-height 900
``` 

### Shortcut and Additional Arguments
```bash
 -i INPUT_PATH        --input-path INPUT_PATH              path to the csv input
 -dw DISPLAY_WIDTH    --display-width DISPLAY_WIDTH        an integer representing the display width
 -dh DISPLAY_HEIGHT   --display-height DISPLAY_HEIGHT      an integer representing the display height
 [-a ALPHA            --alpha ALPHA                        alpha of the gaze overlay                 ]
 [-o OUTPUT_NAME      --output-name OUTPUT_NAME            name of the output file                   ]
 [-b BACKGROUND_IMAGE --background-image BACKGROUND_IMAGE  path to the background image              ]
 ```
**Note:** To add a background image make sure to *provide the whole path* and *only png images without an alpha channel*.

### Data Format
|     X         |        Y      |
| ------------- | ------------- |
|     123       |      654      |
|     121       |      657      |
|     ...       |      ...      |

 ## Appreciation
 The script is based on the heat map plotter of [PyGaze](http://www.pygaze.org).
