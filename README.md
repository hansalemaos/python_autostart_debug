# python_autostart_debug
Magisk / KernelSU plugin to run a Python script at startup

## Create a Python script and save it as `magiskpythonscript.py`

```py
print("Hello")
```

## Push it to the sdcard

```sh
# The script runs at every startup
adb -s 127.0.0.1:5560 push C:\Users\hansc\Downloads\magiskpythonscript.py /sdcard
```

## Check the ouput after startup / execution of the script

```sh
cat /sdcard/magiskpythonscript_debug.txt
```


