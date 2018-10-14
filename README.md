### Monetize
---

https://github.com/RubyMoney/monetize

```
gem 'monetize'
bundel
gem install monetize

Monetize.parse('OMG 100')
Monetize.parse!('OMG 100')


```

```ruby
Monetize.parse("USD 100") == Money.new(100_00, "USD")
Monetize.parse("EUR 100") == Money.new(100_00, "EUR")
Monetize.parse("GBP 100") == Money.new(100_00, "GBP")
"100".to_money == Money.new(100_00, "USD")

Monetize.parse("€100") == Money.new(100_00, "USD")
Monetize.assume_from_symbol = true
Monetize.parse("€100") == Money.new(100_00, "GBP")
"€100".to_money == Money.new(100_00, "EUR")

Monetize.parse_collection("€80/€100") == [Money.new(80_00, "EUR"), Money.new(100_00, "USD")]
Monetize.parse_collection("€80, $100") == [Money.new(80_00, "EUR"), Money.new(100_00, "USD")]

Monetuze.parse_collection().range? == true
```

```

```

