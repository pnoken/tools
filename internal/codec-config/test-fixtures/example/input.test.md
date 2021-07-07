# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/codec-config/index.test.ts --update-snapshots` to update.

## `example`

### `parse .toml`

```javascript
{
	products: [{name: "Hammer", sku: 738_594_937}, {name: "Nail", color: "gray", sku: 284_758_393}]
	title: "TOML Example"
	clients: {data: [["gamma", "delta"], [1, 2]], hosts: ["alpha", "omega"]}
	database: {connection_max: 5_000, enabled: true, ports: [8_001, 8_001, 8_002], server: "192.168.1.1"}
	owner: {
		name: "Tom Preston-Werner"
		bio: "GitHub Cofounder & CEO\nLikes tater tots and beer."
		organization: "GitHub"
		dob: 1979-05-27T07:32:00.000Z
	}
	servers: {
		alpha: {dc: "eqdc10", ip: "10.0.0.1"}
		beta: {country: "\u4e2d\u56fd", dc: "eqdc10", ip: "10.0.0.2"}
	}
}
```

### `stringify .toml`

```toml
title = "TOML Example"
[owner]
name = "Tom Preston-Werner"
organization = "GitHub"
bio = """
GitHub Cofounder & CEO
Likes tater tots and beer."""
[owner.dob]



# First class dates? Why not?
[database]
server = "192.168.1.1"
ports = [
	8_001,
	8_001,
	8_002,
]
connection_max = 5_000
enabled = true

[servers]
# You can indent as you please. Tabs or spaces. TOML don't care.
[servers.alpha]
ip = "10.0.0.1"
dc = "eqdc10"

[servers.beta]
ip = "10.0.0.2"
dc = "eqdc10"
country = "\u4e2d\u56fd"


# This should be parsed as UTF-8
[clients]
data = [
	[
		"gamma",
		"delta",
	],
	[
		1,
		2,
	],
]
hosts = [
	"alpha",
	"omega",
]

# Products
[[products]]
name = "Hammer"
sku = 738_594_937

[[products]]
name = "Nail"
sku = 284_758_393
color = "gray"


```