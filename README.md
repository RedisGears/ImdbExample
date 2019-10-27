# ImdbExample
RedisGears Imdb Example

## Run the Example
* Set up you redis server with RedisGears
* run `python UploadImdb.py`
* run `RG.PYEXECUTE "GB('KeysOnlyReader').map(lambda x: execute('hget', x, 'genres')).flatmap(lambda x: x.split(',')).countby().run()"`
