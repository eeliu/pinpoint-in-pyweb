## Blog


## Download pinpoint-py-plugins
[pinpoint-py-plugins](https://github.com/pinpoint-apm/pinpoint-c-agent/releases/download/v0.4.0/pinpoint-py-v0.4.0.zip)

### Steps

* set database

    ``` py
    ## model.py
    db = web.database(dbn="mysql", db="blog", user="root",pw='root',host="dev-mysql")
    ```
* copy pinpoint
* enable pinpoint middleware
    ``` python
    if __name__ == "__main__":
        from pinpoint.pyweb.middleware import PinPointMiddleWare
        app.run(PinPointMiddleWare)
    ```
  
