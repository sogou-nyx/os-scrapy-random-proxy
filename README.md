# os_scrapy_random_proxy
This project provide a [Downloader Middleware](https://docs.scrapy.org/en/latest/topics/downloader-middleware.html) to add 'proxy' for request.


## Install

```
pip install os-scrapy-random-proxy
```

## Usage

### Settings

* enable downloader middleware in settings.py file:




    ```
    DOWNLOADER_MIDDLEWARES = {
        "os_scrapy_random_proxy.ProxyMiddleware": 543,
    }
    ```

* config useragents:
   
    - by file:

        ```
        PROXIES = "./your-proxies-file"
        ```

    - by string:

        ```
        PROXIES = "Your-Proxy-String"
        ```

    - by list:

        ```
        PROXIES = ["Proxy-01", "Proxy-02"]
        ```

## Unit Tests

```
tox
```

## License

MIT licensed.
