# Run VISUASYL

VISUASYL can be called up via a link without installation or executed locally. 

## Open Link

Run VISUASYL without installation: [https://share.streamlit.io/hannahkruck/visuasyl/app.py](https://share.streamlit.io/hannahkruck/visuasyl/app.py)

Please use Chrome or Firefox browser for best performance.

## Installation

If VISUASYL is to be run locally, the following steps are required:
- Download the [GitHub VISUASYL Repository](https://github.com/hannahkruck/VISUASYL)
- Install all packages from requirements_base.txt and requirements_local.txt via command line: 
```bash
pip install <package that should be installed>
```
- To run VISUASYL you have to run the file --> start.py
- Run VISUASYL with the command via command line:
```bash
streamlit run <path/app.py>
```

## Problem solving if app shows Error 404
Apparently, the problem can occur that the app no longer runs correctly through streamlit sharing.
Then the error code 404 is thrown when the link is called. If the app does not work anymore even after a reboot on the streamlit sharing page, the following workaround should be applied. 

1. Copy the code of start.py (originally app.py) and create a new file, e.g. start_copy.py with the same code.
2. Create a new Streamlit sharing "project" and specify the new file to start the app (in this example: start_copy.py).
3. Start the app on Streamlit sharing.

Now the error should be fixed and the app should run as usual.

There is no official reason for this problem at the moment.
[In this forum post](https://discuss.streamlit.io/t/app-stuck-on-please-wait-app-is-in-the-oven/8395) the problem and the workaround was explained as described here.
