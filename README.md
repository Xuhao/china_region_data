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

First of all, download the latest yaml file from: [https://github.com/Xuhao/china_region_data/raw/master/regions.yml](https://github.com/Xuhao/china_region_data/raw/master/regions.yml)

### Ruby

```ruby
require 'yaml'
regions = File.open('regions.yml') { |file| YAML.load(file) }
# => {"北京市"=>{"pinyin"=>"beijing", "pinyin_abbr"=>"bj", "cities"=> ...
```

### Ruby on Rails

put 'gem china_region_fu' to your Gemfile:

    gem 'china_region_fu'

Check out [ChainRegionFu](https://github.com/Xuhao/china_region_fu) gem for more details

:two_men_holding_hands: Examples for other languages need your help! :hand:

# Contributing

Any corrections and improvements are welcome!

Need you help to replenish the missing data, improve the data schema and anything that make it useful for other developers.