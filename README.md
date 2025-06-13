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
		-- stylua: ignore start
		{ '*', function() require('asterisk-remix').normal_search('*') end, mode = 'n', desc = 'Asterisk: *' },
		{ '#', function() require('asterisk-remix').normal_search('#') end, mode = 'n', desc = 'Asterisk: #' },
		{ 'g*', function() require('asterisk-remix').normal_search('g*') end, mode = 'n', desc = 'Asterisk: g*' },
		{ 'g#', function() require('asterisk-remix').normal_search('g#') end, mode = 'n', desc = 'Asterisk: g#' },
		{ '*', function() return require('asterisk-remix').visual_search('*') end, desc = 'Asterisk: *', mode = 'x', { expr = true } },
		{ '#', function() return require('asterisk-remix').visual_search('#') end, desc = 'Asterisk: #', mode = 'x', { expr = true } },
		{ '<Space>*', function() return require('asterisk-remix').operator_search('*') end, mode = 'n', desc = 'Asterisk: Ope *', { expr = true } },
		{ '<Space>#', function() return require('asterisk-remix').operator_search('#') end, mode = 'n', desc = 'Asterisk: Ope #', { expr = true } },
		-- stylua: ignore end
	}
}
```

# Similar projects

- [haya14busa/vim-asterisk](https://github.com/haya14busa/vim-asterisk)
- [rapan931/lasterisk.nvim](https://github.com/rapan931/lasterisk.nvim)
