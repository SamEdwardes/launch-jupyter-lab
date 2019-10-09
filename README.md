# Launch Jupyter Lab

Launches Jupyter Lab as in Chrome app mode.

## Setup

**Step 1**

the following option must exist in `jupyter_notebook_config.py`. Note that the file is saved `/Users/samedwardes/.jupyter/jupyter_notebook_config.py`

```python
c.NotebookApp.browser = '/Applications/Google\ Chrome.app/Contents/MacOS/Google\ Chrome --app=%s'
```

**Step 2**

Create an apple script:

```
tell application "Terminal" to do script "~/tools/launch-jupyter-lab/jupyter-lab.command"
```

Then export the script as an application.

**Step 3**

Edit the icon of the application if you wish and drag to dock.


## Reference

[https://mdyzma.github.io/2018/06/24/running-jupyter-lab-in-application-mode/](https://mdyzma.github.io/2018/06/24/running-jupyter-lab-in-application-mode/)