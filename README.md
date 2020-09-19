# Heartfelt Words

:heart: 心语

> 源自大千世界中芸芸众生

## 分类

- `animation` 动漫
- `film` 影视
- `game` 游戏
- `innovation` 原创
- `literary` 文学
- `philosophy` 哲学
- `verse` 诗词
- `world` 大千世界

> 动漫：动画 + 漫画，仅在华语圈使用
>
> ACG：动画 + 漫画 + 游戏

## 请求示例

```bash
curl -G 'https://cdn.jsdelivr.net/gh/cnguu/heartfelt-words@master/<type>/<page>.json'
```

- `type` 分类
- `page` 当前页

> 默认每页数量：3000

## 返回参数

- `key` 唯一值，生成格式：`data-h-年月日时分秒`
- `heart` 内容
- `type` 分类
- `origin` 来源
- `author` 作者
- `recorded_at` 收录日期

示例：

```json
{
  "key": "data-h-20200101000000",
  "heart": "床前明月光，疑是地上霜，举头望明月，低头思故乡",
  "type": "verse",
  "origin": "《唐诗三百首》",
  "author": "李白",
  "recorded_at": "2020年01月01日"
}
```

## 配置

```bash
# 分类
curl -G 'https://cdn.jsdelivr.net/gh/cnguu/heartfelt-words@master/config/type.json'
```

### 分类

- `key` 唯一值
- `title` 标题
- `total` 收录总数

## License

- [MIT](https://cdn.jsdelivr.net/gh/cnguu/heartfelt-words@master/LICENSE)
