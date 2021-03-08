# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/codec-browsers/index.test.ts --update-snapshots` to update.

## `combined > full`

### `result`

```javascript
[
	"edge:88"
	"edge:87"
	"firefox:87"
	"firefox:86"
	"chrome:91"
	"chrome:90"
	"safari:14"
	"safari:13.1"
	"opera:73"
	"opera:72"
	"ios_saf:14.4"
	"ios_saf:14"
	"op_mini:1"
	"android:81"
	"android:4.4"
	"op_mob:59"
	"and_chr:88"
	"and_ff:85"
	"and_uc:12.12"
	"samsung:13"
	"samsung:12"
	"and_qq:10.4"
	"baidu:7.12"
	"kaios:2.5"
]
```

### `targets`

```javascript
[
	TargetBrowserPreset {preset: "modern"}
	TargetBrowserCombination {
		and: TargetBrowserRange {browser: "Firefox", to: 85, version: 80}
		target: TargetBrowserUsage {operator: "GT", usage: 5}
	}
	TargetBrowserLast {browser: "Chrome", qty: 2, unit: "versions"}
	TargetBrowserCombination {
		and: TargetBrowserUsage {operator: "GT", region: "BE", usage: 20}
		target: TargetBrowserSince {since: 1_525_132_800_000}
	}
]
```

### `tokens`

```javascript
[
	Modern {
		end: ZeroIndexedNumber<6>
		start: ZeroIndexedNumber<0>
	}
	Or {
		end: ZeroIndexedNumber<7>
		start: ZeroIndexedNumber<6>
	}
	GT {
		end: ZeroIndexedNumber<9>
		start: ZeroIndexedNumber<8>
	}
	Percentage {
		value: 5
		end: ZeroIndexedNumber<12>
		start: ZeroIndexedNumber<10>
	}
	And {
		end: ZeroIndexedNumber<16>
		start: ZeroIndexedNumber<13>
	}
	String {
		value: "Firefox"
		end: ZeroIndexedNumber<24>
		start: ZeroIndexedNumber<17>
	}
	Number {
		value: 80
		end: ZeroIndexedNumber<27>
		start: ZeroIndexedNumber<25>
	}
	Hyphen {
		end: ZeroIndexedNumber<28>
		start: ZeroIndexedNumber<27>
	}
	Number {
		value: 85
		end: ZeroIndexedNumber<30>
		start: ZeroIndexedNumber<28>
	}
	Or {
		end: ZeroIndexedNumber<31>
		start: ZeroIndexedNumber<30>
	}
	Last {
		end: ZeroIndexedNumber<36>
		start: ZeroIndexedNumber<32>
	}
	Number {
		value: 2
		end: ZeroIndexedNumber<38>
		start: ZeroIndexedNumber<37>
	}
	String {
		value: "Chrome"
		end: ZeroIndexedNumber<45>
		start: ZeroIndexedNumber<39>
	}
	Versions {
		end: ZeroIndexedNumber<54>
		start: ZeroIndexedNumber<46>
	}
	Or {
		end: ZeroIndexedNumber<57>
		start: ZeroIndexedNumber<55>
	}
	Since {
		end: ZeroIndexedNumber<63>
		start: ZeroIndexedNumber<58>
	}
	Number {
		value: 2_018
		end: ZeroIndexedNumber<68>
		start: ZeroIndexedNumber<64>
	}
	Hyphen {
		end: ZeroIndexedNumber<69>
		start: ZeroIndexedNumber<68>
	}
	Number {
		value: 5
		end: ZeroIndexedNumber<71>
		start: ZeroIndexedNumber<69>
	}
	And {
		end: ZeroIndexedNumber<75>
		start: ZeroIndexedNumber<72>
	}
	GT {
		end: ZeroIndexedNumber<77>
		start: ZeroIndexedNumber<76>
	}
	Percentage {
		value: 20
		end: ZeroIndexedNumber<81>
		start: ZeroIndexedNumber<78>
	}
	In {
		end: ZeroIndexedNumber<84>
		start: ZeroIndexedNumber<82>
	}
	String {
		value: "BE"
		end: ZeroIndexedNumber<87>
		start: ZeroIndexedNumber<85>
	}
	EOF {
		end: ZeroIndexedNumber<88>
		start: ZeroIndexedNumber<88>
	}
]
```