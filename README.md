# Asterisk-remix: Yet another * -Improved

**This plugin is in WIP state**

---

- TODO: add DEMO
	- Use `nvim-keycastr`?

# Installation

## Lazy.nvim

```lua
{
	'https://github.com/kjuq/asterisk-remix.nvim',
	keys = {
		{ '*', function() require('asterisk-remix').normal_search('*') end, mode = 'n' },
		{ '#', function() require('asterisk-remix').normal_search('#') end, mode = 'n' },
		{ 'g*', function() require('asterisk-remix').normal_search('g*') end, mode = 'n' },
		{ 'g#', function() require('asterisk-remix').normal_search('g#') end, mode = 'n' },
		{ '*', function() return require('asterisk-remix').visual_search('*') end, mode = 'x', { expr = true } },
		{ '#', function() return require('asterisk-remix').visual_search('#') end, mode = 'x', { expr = true } },
		{ '<Space>*', function() return require('asterisk-remix').operator_search('*') end, mode = 'n', { expr = true } },
		{ '<Space>#', function() return require('asterisk-remix').operator_search('#') end, mode = 'n', { expr = true } },
	}
}
```

# Similar projects

- [haya14busa/vim-asterisk](https://github.com/haya14busa/vim-asterisk)
- [rapan931/lasterisk.nvim](https://github.com/rapan931/lasterisk.nvim)
