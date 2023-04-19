# altv-joaat-renamer


This script renames all files in `models` directory with their JOAAT hash as the new file name.

## Why?

i was tired of renaming [700+](https://github.com/altmp/altv-docs-assets/tree/master/altv-docs-gta/images/vehicle/models) Vehicle Models by hand so i made this script to do it for me

You kann convert to: 
> uint32 \
> int32\
> hex

[altv docs](https://docs.altv.mp/gta/articles/references/joaat.html)

# Requirements

- Node.js v18.x or higher


# Installation and Usage

1. Clone this repository
2. Run `npm install` in the repository directory
3. Copy the files that you want to rename from your directory to the `models` directory
4. Run `node rename.js` in the repository directory
5. Copy the files from the `models` directory to your directory

# Configuration
you can caange what you want to convert to in `line 63` in `rename.js`


```js
const newFilename = `${uint32}${extname}`;
const newFilename = `${int32}${extname}`;
const newFilename = `${hex}${extname}`;
```



## Example

### Before

```bash
├── models
│   ├── adder.png
│   ├── airbus.png
│   ├── airtug.png
├── ...
```
### After (hex) 

```bash
├── models
│   ├── 0xB779A091.png
│   ├── 0x4C80EB0E.png
│   ├── 0x5D0AAC8F.png
├── ...
```

# Support

> Support [Discord-Server](https://discord.gg/z8ScRvf)
