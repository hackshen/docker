# verdaccio

```bash
# 直接运行
V_PATH=/path/for/verdaccio; docker run -it --rm --name verdaccio \
  -p 4873:4873 \
  -v $V_PATH/conf:/verdaccio/conf \
  -v $V_PATH/storage:/verdaccio/storage \
  -v $V_PATH/plugins:/verdaccio/plugins \
  -e 'VERDACCIO_PORT=8080' \
  verdaccio/verdaccio
  
# 设置目录拥有者(否则没权限读取映射的文件夹)
sudo chown -R 10001:65533 /path/for/verdaccio
```