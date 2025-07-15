# EasyUse Styles Selectors Prompts Templates

This repository mainly stores custom style selector prompt templates and the preview thumbnails used. You only need to download the JSON files and place them in the styles folder under the easyuse root directory. You can also supplement the needed content based on the current files. Of course, if you are willing, you can submit PRs according to this format to supplement prompt templates.


## List of Prompts

| Preview | Name | File |
|---------|------|------|
|   ![图片](./preview/kontext_presets.jpg)     |  Kontext Presets    |  [⬇️ Download](https://raw.githubusercontent.com/yolain/EasyUse-Styles-Templates/refs/heads/main/templates/kontext_presets.json)    |



## Currently supported formats

```json
[
    {
        "name": string, // Required, the name of the prompt template
        "name_cn": string, // Optional, the Chinese name of the prompt template
        "prompt": string, // Required, the prompt template content
        "negative_prompt": string, // Optional, the negative prompt template content
        "thumbnail": string | array, // Optional, the thumbnail image path or an array of paths
        "thumbnail_variant": ['default', 'compareSlider', 'hoverDissolve'], // Optional, the thumbnail variant type
    }
]
```

## How to set the thumbnail?

### 1. URL Paths

You can set the thumbnail to a URL path, such as:

```json
[
    {
        //... other properties
        "thumbnail": "https://example.com/path/to/thumbnail.jpg"
    }
]
```

### 2. Local Path

You can place the thumbnails in the samples folder under the styles directory, then reference them using relative paths, for example:

```json
[
    {
        //... other properties
        "thumbnail": "kontext_presets/thumbnail.jpg" // the root path is the samples folder
    }
]
```

