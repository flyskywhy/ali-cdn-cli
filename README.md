# ali-cdn-cli
A cli wrapper of [aliyun-cdn-refresh](https://www.npmjs.com/package/aliyun-cdn-refresh) to simplify Refresh and push interface for aliyun cdn api

[CDN缓存概览](https://help.aliyun.com/knowledge_detail/40190.html)

```
npm install -g ali-cdn-cli
```
```
  Usage: ali-cdn-cli [options]

  Options:

    -i, --AccessKeyId <value>      Aliyun AccessKeyId
    -k, --AccessKeySecret <value>  Aliyun AccessKeySecret
    -d, --refreshDir <dir>         refresh dir on CDN Cache to be expired
    -f, --refreshFile <file>       refresh file on CDN Cache to be expired
    -p, --pushFile <file>          push file into CDN L2 Cache
    -h, --help                     output usage information
```
## [刷新缓存](https://help.aliyun.com/document_detail/27200.html) refresh dir or file on CDN Cache to be expired
```
ali-cdn-cli --refreshDir http://yourcdndomain/img/
ali-cdn-cli --refreshFile http://yourcdndomain/img/1.png
```
[使用CDN后，文件与源文件不一致，如何刷新缓存](https://help.aliyun.com/knowledge_detail/40188.html)

## [预热](https://help.aliyun.com/document_detail/27201.html) push file into CDN L2 cache
```
ali-cdn-cli --pushFile http://yourcdndomain/img/1.png
```
[如何判断CDN的预热任务是否执行完成](https://help.aliyun.com/knowledge_detail/40132.html)
