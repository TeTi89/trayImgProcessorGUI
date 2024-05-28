# create a virtual environment
>>python -m venv .venv
# activate the virtual environment
>>.venv\Scripts\activate
# deactivate the virtual environment
>>deactivate
# delete the virtual environment
>>rmdir /s .venv

# to download the libraries, run the following commands in the terminal
>>pip install -r requirements.txt
# check the installed libraries
>>pip list

# change GUI layout

``` python
'''
%%%%%%%%% GUI %%%%%%%%%
'''


# create the main window
window = tk.Tk()
# set the window size
window.geometry("800x950")
# set the window size to be fixed
window.resizable(False, False)
# set the window title
window.title("Tray Image Processor")

'''
%%%%%%%%% LAYOUT %%%%%%%%%

Legend:
ent -> entry
btn -> button
lbl -> label
frm -> frame
txt -> text
radio button -> radio
check button -> checkbnt
scale -> scl

+-----------------------------------+
## frame_A: file path ##
| ent(filePath) | btn(browse) | btn(load) |
-------------------------------------
## frame_B: tray image ##
| lbl(trayImg) | lbl(para) |
| btn(rotCW) | btn(rotCCW) | btn(zoomIn) | btn(zoomOut) | btn(MovUp) | btn(MovDn) | btn(MovL) | btn(MovR) |
-------------------------------------
## frame_C: pot images ##
| lbl(Img) | lbl(Img) | lbl(Img) | lbl | radio(showPot) |
-------------------------------------
## frame_D: parameters ##
| checkbnt(useChannelA) | lbl(min) | scl(min) | lbl(max) | scl(max) |
-------------------------------------
## frame_E: parameters ##
| checkbnt(useChannelH) | lbl(min) | scl(min) | lbl(max) | scl(max) |
-------------------------------------
## frame_F: parameters ##
| checkbnt(useChannelV) | lbl(min) | scl(min) | lbl(max) | scl(max) |
-------------------------------------
## frame_G: parameters ##
| radio(kernelSize) | btn(analyze) |
+-----------------------------------+

```