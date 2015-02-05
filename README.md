Compares [Protocol Buffers](https://developers.google.com/protocol-buffers/)
with alternatives.

$ python protobuftest.py
         Read   Write    Size
json     1.00    1.00    1.00
proto   16.29    7.53    0.57
json.gz  4.37    1.08    0.37
csv.gz   5.01    0.47    0.34

So looks like Protobufs are significantly slower than JSON.
The only advantage is file size.
But if you write gzipped JSON files, they're almost as fast, and much smaller.