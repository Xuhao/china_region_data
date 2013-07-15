China region data
=================

Chinese region data with yaml format. There levels currently: **province**, **city**, **district**.

## Schema

### Province

* `name`: 名称
* `pinyin`: 拼音
* `pinyin_abbr`: 拼音缩写

### City

* `name`: 名称
* `pinyin`: 拼音
* `pinyin_abbr`: 拼音缩写
* `zip_code`: 邮政编码
* `level`: 等级(1:直辖市, 2:省会城市, 3:重要城市, 4:普通城市)

### District

* `name`: 名称
* `pinyin`: 拼音
* `pinyin_abbr`: 拼音缩写

## Usage

### Ruby

```ruby
require 'yaml'
regions = File.open('regions.yml') { |file| YAML.load(file) }
# => {"北京市"=>{"pinyin"=>"beijing", "pinyin_abbr"=>"bj", "cities"=> ...
```

Examples for other languages need your help! :hand:

# Contributing

Any corrections and improvements are welcome!

Need you help to replenish the missing data, improve the data schema and anything that make it useful for other developers.